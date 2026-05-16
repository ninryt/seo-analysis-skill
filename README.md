# SEO Analysis Skill

A Claude Code skill for SEO and web/mobile audit workflows. Covers full-site audits, single-page reviews, technical SEO, content quality and E-E-A-T, AI search / GEO readiness, schema, XML sitemaps, image optimization, hreflang, competitor comparison pages, programmatic SEO, and SEO strategy.

**Author:** Nina Ryttel ([@ninryt](https://github.com/ninryt))
**License:** [MIT](LICENSE) : reuse is welcome, please keep the copyright notice.

## Files

- `SKILL.md`: main skill instructions and trigger description.
- `references/seo-workflows.md`: detailed workflow definitions (12 sub-workflows).

## Install

Copy this folder to your Claude Code skills directory:

```bash
cp -r seo-analysis-skill ~/.claude/skills/seo-analysis
```

Claude Code picks it up automatically on next session start.

## Workflows

The skill bundles 12 sub-workflows. The full list and detail lives in [references/seo-workflows.md](references/seo-workflows.md):

- `seo-audit`: full-site SEO health check + prioritized action plan
- `seo-page`: single-page deep review
- `seo-content`: E-E-A-T, helpfulness, readability, AI citation readiness
- `seo-technical`: crawlability, indexability, Core Web Vitals, security, JS rendering
- `seo-schema`: Schema.org detection, validation, JSON-LD generation
- `seo-sitemap`: XML sitemap validation and generation
- `seo-images`: alt text, formats, responsive images, CLS prevention
- `seo-hreflang`: international SEO targeting
- `seo-competitor-pages`: "X vs Y", "alternatives to X", comparison pages
- `seo-programmatic`: pages generated at scale, with thin-content gates
- `seo-geo`: AI search / Generative Engine Optimization
- `seo-plan`: roadmaps, content strategy, implementation sequencing

## Scope

In scope: SEO audits, technical SEO, content/E-E-A-T review, schema, sitemaps, image SEO, hreflang, competitor pages, programmatic SEO, GEO, SEO planning. Also: ASO-adjacent web work (app landing pages, App Store / Play Store copy review, schema on app webpages).

Out of scope: UX/UI heuristic evaluation, usability testing, in-product user-flow audits, in-app funnel/retention/revenue analysis.

## Example prompt

```text
Use the SEO Analysis skill to audit this website: [URL].
Give me an executive summary, technical issues, content issues,
schema opportunities, sitemap issues, AI search readiness, and
a prioritized action plan.
```
