# TikTok Creator & Ecommerce Demand Research — 2026-03-11

## Method

Demand signals were collected from:
1. Reddit community titles (TikTokShop / UGCcreators / shopify / ecommerce / Tiktokmarketing)
2. ClawHub search landscape snapshots (queries: `tiktok creator`, `tiktok shop`, `ecommerce`)
3. Existing internal execution signals (creator outreach + automation workflows)

Artifacts:
- `artifacts/demand-research/tiktok_ecom_sources_2026-03-11.json`
- `artifacts/demand-research/tiktok_ecom_summary_2026-03-11.json`

## High-signal demand clusters

1. **Creator discovery + matching**
   - recurring questions on finding the right creators and collaboration fit
2. **Hook/retention pressure**
   - repeated concerns about low views and weak opening performance
3. **Sales conversion + profit visibility**
   - repeated requests about sales lift and real profit after ad spend
4. **Operational bottlenecks**
   - fulfillment, order-to-label, and logistics friction concerns
5. **Risk/compliance and trust**
   - DMCA/misrepresentation/policy anxiety in ecommerce operations
6. **Review/refund insight extraction**
   - need to convert review/refund text into actionable fixes

## Selected 10 new skills (next build batch)

Priority 11-20 were selected to maximize:
- immediate install value,
- repeat usage for demand validation,
- productization potential for Creatop.

1. `tiktok-shop-creator-fit-scorer`
2. `review-defect-miner`
3. `listing-gap-audit`
4. `shopify-tracking-auditor`
5. `price-gap-monitor`
6. `refund-reason-cluster`
7. `ugc-hook-analyzer`
8. `checkout-friction-audit`
9. `promo-calendar-optimizer`
10. `creator-outreach-sequence-lab`

## Release strategy

Because ClawHub enforces new-skill publish rate limits, release in two waves:
- Wave 1 (first 5): priorities 11-15
- Wave 2 (next 5): priorities 16-20

Each wave should include:
- GitHub sync (README/index/manifest + skill folders)
- ClawHub publish/sync
- post-release usage feedback collection via issue templates.
