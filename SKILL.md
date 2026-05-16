---
name: seo-analysis
description: SEO and web/mobile audit workflows : website audits, single-page audits, technical SEO, content quality, E-E-A-T, AI search/GEO readiness, schema, XML sitemaps, image optimization, hreflang, competitor comparison pages, programmatic SEO, and SEO strategy. Foundation skill : Nina will build on top of it as audits come up. Trigger when Nina mentions auditing a website, landing page, app landing page, app store listing, or competitor site; planning SEO work; reviewing content for search or AI-citation readiness; generating schema or sitemaps; or asking for a "web audit", "mobile audit", "competitor audit", or "SEO audit". Does NOT cover UX/UI heuristic evaluation, usability testing, or in-product user-flow audits : those are a separate discipline.
---

# SEO Analysis

## Quick Start

Select the narrowest workflow that matches the request. If the user asks for a full audit, start with `seo-audit`, then deepen with specialist workflows where issues appear.

Read [references/seo-workflows.md](references/seo-workflows.md) when you need the detailed workflow list, scoring areas, outputs, or quality checks.

## Workflow Picker

- Use `seo-audit` for full-site SEO health checks and prioritized action plans.
- Use `seo-page` for one landing page, article, product page, campaign page, or app landing page.
- Use `seo-content` for E-E-A-T, helpfulness, readability, thin content, intent coverage, and AI citation readiness.
- Use `seo-technical` for crawlability, indexability, robots.txt, Core Web Vitals, mobile, JavaScript rendering, security, structured data presence, AI crawler management, and IndexNow.
- Use `seo-schema` for Schema.org detection, validation, and JSON-LD generation.
- Use `seo-sitemap` for XML sitemap validation or generation.
- Use `seo-images` for alt text, file size, formats, responsive images, lazy loading, CLS prevention, and CDN usage.
- Use `seo-hreflang` for international SEO and language/region targeting.
- Use `seo-competitor-pages` for "X vs Y", "alternatives to X", comparison tables, and "best tools" pages.
- Use `seo-programmatic` for pages generated at scale from structured data, including quality gates against thin content and index bloat.
- Use `seo-geo` for AI search visibility in ChatGPT, Perplexity, Google AI Overviews, and similar answer engines.
- Use `seo-plan` for SEO roadmaps, content strategy, competitor research, and implementation sequencing.

## Standard Output

For most SEO tasks, produce:

1. Executive summary.
2. Priority table: issue, severity, affected area, evidence, recommendation, expected impact.
3. Detailed findings grouped by workflow area.
4. Quick wins versus deeper work.
5. Measurement plan: rankings, impressions, CTR, indexed pages, conversions, revenue, or ASO/web landing-page metrics as relevant.
6. Next actions with owner-friendly wording.

## Project Fit

When working inside a marketing-analysis project, keep SEO artifacts organized under an `seo/` folder:

```text
seo/
  audits/
  notes/
  reports/
  templates/
  scripts/
```

For mobile app work, use this skill for ASO-adjacent and web discoverability tasks: app landing pages, App Store or Play Store copy review, competitor positioning, review-mined messaging, schema on app webpages, AI search visibility, and SEO/ASO roadmap planning. For in-app funnels, retention, push performance, revenue cohorts, or crash/performance analytics, use a separate app growth analysis workflow.
