---
name: technical-seo-checker
description: Audit technical SEO issues such as crawlability, indexability, page speed, Core Web Vitals, redirects, canonical tags, hreflang, robots.txt, sitemaps, and structured data. Use when the user asks for a technical SEO audit, site health check, crawl/index diagnosis, speed review, or migration checklist.
---

# Technical SEO Checker

## What this skill solves

Find the technical issues that stop search engines from crawling, indexing, or ranking a site properly.

## Use when

- The user wants a technical SEO audit or site health check
- The site has crawl, index, speed, mobile, or rendering issues
- The user needs a pre-migration SEO checklist
- The user wants Core Web Vitals or redirect/canonical review

## Do not use when

- The issue is mainly page copy, headers, or content quality
- The user wants keyword strategy or content planning
- The task is a general web performance debug unrelated to SEO

## Inputs to ask for

Ask only for the minimum needed:
1. URL or domain
2. Specific problem, if known
3. Optional: PageSpeed, Search Console, robots.txt, sitemap, or crawl data

## Workflow

1. Identify the pages or sections in scope.
2. Check crawlability and indexability first.
3. Review performance, mobile, redirects, canonicals, and structured data.
4. Separate critical blockers from lower-priority issues.
5. Return a prioritized fix list.

## Output requirements

Always include:
- Overall technical health score, if possible
- Critical issues
- High-priority issues
- Medium-priority issues
- Recommended fixes
- Migration or remediation notes, if relevant

## Quality standards

- Be specific about impact, not just symptoms
- Prioritize blockers before nice-to-haves
- Keep recommendations actionable
- Avoid mixing content issues into technical checks

## Safety / constraints

- Do not assume access to Search Console or crawl tools unless provided
- Do not invent metrics
- Clearly label manual vs. tool-based findings
