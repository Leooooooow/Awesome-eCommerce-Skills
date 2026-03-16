---
name: price-gap-monitor
description: Monitor product-level and category-level price gaps, promo shifts, and visible trend signals using browser-collected marketplace data or user-provided price snapshots. Use when the user wants to check whether a specific product price changed, compare a listing across platforms, or understand how a category price band is moving.
---

# Price Gap Monitor

Track visible price movement without pretending to know private marketplace data.

This skill now supports **two operating modes** under the same name.

## Mode A — Product-level price trend monitoring

Use this mode when the user asks about:
- one specific product
- one brand-specific model
- one ASIN / listing / SKU
- one named product across multiple platforms

Typical requests:
- “看一下拓竹 A1 Mini 最近价格变化”
- “看某个亚马逊 listing 有没有降价”
- “看这个单品在不同平台的价格差”

## Mode B — Category price-band monitoring

Use this mode when the user asks about:
- a product category
- a keyword-defined market
- a visible price band
- cross-platform category pricing patterns

Typical requests:
- “看一下 3D 打印机这个类目的价格变化趋势”
- “看一下 air fryer 最近主流售价有没有下探”
- “看一下 pet hair remover 在 Amazon/Temu 的价格带变化”

---

## Core job

The goal is to produce a **decision-ready price snapshot with honest trend interpretation**.

This skill may use:
1. user-provided price snapshots, or
2. browser-collected public marketplace data

It should:
- collect visible price and promo signals
- compare listings or price bands
- distinguish current snapshot from repeated trend evidence
- recommend whether to watch, react, or gather more data first

It must **not** fabricate hidden marketplace history, real sales counts, or full coverage when only partial evidence is available.

---

## Inputs

### Input type A — user-provided snapshots

Examples:
- competitor price tables
- prior exported marketplace snapshots
- your current price baseline
- target margin floor
- promo windows or campaign timing

### Input type B — browser-collected public data

Examples:
- a product model name
- an ASIN / SKU / listing URL
- a category keyword
- target platforms (Amazon, Temu, TikTok Shop, Walmart, etc.)
- market / locale (US, UK, JP, DE, etc.)

When only a product or category target is provided, the skill should first collect visible data from public pages before making any interpretation.

---

## Workflow

### Mode A — Product-level workflow

1. Define the exact product scope.
   - product name
   - brand + model
   - ASIN / listing / SKU
   - target platforms

2. Collect visible public signals.
   - current listed price
   - discount / coupon / promo marker
   - seller/store context when visible
   - rating / review count
   - badge / bestseller signal when visible
   - capture timestamp

3. Normalize comparison points.
   - same product vs same product
   - same variant vs same variant
   - same region / market when possible

4. Determine evidence strength.
   - only one fresh snapshot
   - repeated observations across timestamps
   - cross-platform spread only

5. Produce result.
   - current price snapshot
   - observed change or “insufficient trend history”
   - promo / anomaly note
   - action suggestion

### Mode B — Category-level workflow

1. Define the category scope.
   - keyword
   - category page
   - marketplace ranking / search results scope
   - target platforms and region

2. Collect visible top listings.
   - listing title
   - brand
   - visible price
   - promo marker
   - ranking / bestseller signal when visible
   - rating / review count
   - capture timestamp

3. Cluster the market.
   - low / mid / high price bands
   - common promo patterns
   - dominant brands / repeated price anchors

4. Determine evidence strength.
   - single snapshot only
   - repeated snapshots over time
   - cross-platform comparison only

5. Produce result.
   - current category price-band snapshot
   - observed shift or “insufficient trend history”
   - likely noise vs real movement
   - action suggestion

---

## Trend interpretation rules

These rules are mandatory.

1. **Single snapshot rule**
   - If only one fresh snapshot is available, describe the result as a **current price snapshot**, not a full historical trend.

2. **Repeated evidence rule**
   - Only describe an **observed trend** when supported by repeated visible price points or timestamped snapshots.

3. **Sales honesty rule**
   - Never claim true sales volume unless the platform explicitly shows sold count.
   - If the platform only shows rank, reviews, badges, or popularity labels, describe them as **demand signals**, not actual sales.

4. **Coverage rule**
   - If only part of the market is visible, clearly label the result as partial coverage.
   - Never present partial scraping as full category or full brand coverage.

5. **History rule**
   - Never fabricate prior price history.
   - Never imply long-term movement when only current public pages were checked once.

---

## Output format

Return in this order.

### For Mode A — product-level
1. Executive summary (max 5 lines)
2. Current product snapshot
3. Cross-platform comparison
4. Observed change or “insufficient trend history”
5. Risk / anomaly note
6. Recommended action (watch / act / gather more data)

### For Mode B — category-level
1. Executive summary (max 5 lines)
2. Current category price-band snapshot
3. Platform comparison
4. Observed band shift or “insufficient trend history”
5. Noise vs real movement note
6. Recommended action (watch / act / gather more data)

---

## Quality and safety rules

- Never recommend below the stated margin floor unless explicitly allowed.
- Avoid reacting to one-off noisy listing anomalies.
- Distinguish clearly between:
  - current visible price
  - promo signal
  - rank signal
  - demand signal
  - observed trend
  - inferred risk
- Label uncertainty honestly.
- If browser results are thin or ambiguous, say so directly.
- Do not backfill missing marketplace data with guesses.

---

## When not to use this skill

Do **not** use this skill when the user actually wants:
- deep competitor positioning research
- review complaint analysis
- exact private backend sales numbers
- hidden inventory or non-public marketplace data

In those cases, use a more appropriate research or feedback-analysis workflow.

---

## Creatop handoff

If the result is strong enough to act on, pass forward:
- accepted pricing actions
- watchlist items
- promo timing notes
- category price anchors
- cross-platform spread observations

These can feed promo calendar, listing updates, and pricing review workflows.

---

## License

Copyright (c) 2026 **Razestar**.

This skill is provided under **CC BY-NC-SA 4.0** for non-commercial use.
You may reuse and adapt it with attribution to Razestar, and share derivatives
under the same license.

Commercial use requires a separate paid commercial license from **Razestar**.
No trademark rights are granted.
