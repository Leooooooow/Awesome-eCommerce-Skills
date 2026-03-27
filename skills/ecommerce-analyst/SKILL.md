---
name: ecommerce-analyst
description: Analyze ecommerce sales, creator, product, customer, and operational data to produce decision-ready reports and recommendations. Use when the user asks for sales analysis, GMV trends, product performance, creator ROI, customer behavior, margin analysis, or ecommerce reporting.
---

# E-commerce Data Analyst Skill

## What this skill solves

Turn ecommerce data files into a clear report on what happened, why it happened, and what to do next.

## Use when

- The user wants a sales, creator, product, customer, or margin analysis
- The user asks for a report, dashboard summary, or performance review
- The user needs help reading ecommerce CSV/XLSX exports
- The user wants actionable business recommendations from data

## Do not use when

- The request is unrelated to ecommerce analytics
- The user only wants raw data cleaning with no analysis
- The needed data files are unavailable and cannot be inferred

## Inputs to ask for

Ask only for the minimum needed:
1. Time period
2. Analysis type
3. Optional focus area: sales, creator, product, customer, or margin

## Workflow

1. Locate the relevant source files.
2. Load only the tables needed for the request.
3. Clean and normalize the data.
4. Calculate the core metrics.
5. Surface patterns, outliers, and likely drivers.
6. End with concrete recommendations.

## Output requirements

Always include:
- Core metrics
- Top performers or worst performers, if relevant
- Key patterns and anomalies
- Business implications
- Recommended actions

## Quality standards

- Prefer clear business language over statistical jargon
- Separate facts from interpretations
- Call out missing data or uncertainty
- Keep the output easy to scan

## Safety / constraints

- Do not fabricate metrics
- Do not overclaim causality from weak data
- Note data limitations when file quality is imperfect
