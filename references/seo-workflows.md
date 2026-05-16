# SEO Workflows

## `seo-audit`

Full website SEO audit. Crawl up to 500 pages where feasible, respect robots.txt, and delegate to specialist workflows: technical, content, schema, sitemap, images, and GEO. Produce a scored SEO health report and prioritized action plan.

Core areas:

- Fetch and inspect homepage signals.
- Detect business type and likely conversion goals.
- Crawl internal links up to the agreed page limit.
- Review crawlability, indexability, Core Web Vitals, security, content quality, structured data, sitemap quality, image SEO, and AI search readiness.
- Aggregate into a 0-100 SEO Health Score.

Outputs:

- `FULL-AUDIT-REPORT.md`: comprehensive findings.
- `ACTION-PLAN.md`: recommendations prioritized Critical, High, Medium, Low.

Suggested scoring weights:

- Technical SEO: 25%.
- On-page SEO: 20%.
- Content quality: 25%.
- Schema/structured data: 10%.
- Performance/Core Web Vitals: 10%.
- Images: 5%.
- AI search readiness: 5%.

## `seo-competitor-pages`

Generate SEO-optimized competitor comparison and alternatives pages.

Use for:

- "X vs Y" pages.
- "Alternatives to X" pages.
- "Best [category] tools" roundup pages.
- Comparison table pages.

Include:

- Balanced feature-by-feature comparison.
- Clear verdict or recommendation with justification.
- Feature matrix.
- Current pricing with "as of [date]" note.
- Public sources for competitor claims.
- Schema markup: Product, SoftwareApplication, ItemList as appropriate.
- Keyword targeting patterns and title/H1 formulas.
- Conversion layout: above-fold CTA, CTA after comparison table, bottom recommendation CTA.
- Trust signals: last updated date, author expertise, methodology, disclosure of own product affiliation.

Fairness rules:

- Verify competitor information from public sources.
- Do not make false or misleading claims.
- Acknowledge competitor strengths honestly.
- Review when competitors ship major changes.

## `seo-content`

Content quality and E-E-A-T analysis with AI citation readiness.

Assess:

- Experience: original research, case studies, process documentation, unique data, photos/videos from direct experience.
- Expertise: author credentials, professional background, technical depth, accurate sourcing.
- Authoritativeness: external citations, backlinks, brand mentions, recognized outlets, expert citations.
- Trustworthiness: contact info, policies, reviews, date stamps, transparent corrections, HTTPS.
- Word count as topical coverage floors, not direct ranking targets.
- Readability: Flesch Reading Ease, grade level, sentence length, paragraph length, scannability.
- Keyword optimization: primary keyword, semantic terms, headings, alt text, title/meta alignment.
- Content structure: H1/H2/H3 flow, answer-first sections, tables, lists, FAQs.
- AI content quality: human oversight, specificity, original insight, factual accuracy.
- Freshness: dates, updates, current examples, stale claims.
- AI citation readiness: clear quotable claims, data points, source citations, answer-first formatting.

Important note:

- Google word count and readability are not direct ranking factors. Treat them as proxies for topical coverage and accessibility.

## `seo-geo`

Generative Engine Optimization and AI search visibility.

Assess:

- Whether pages are easy for AI answer engines to cite.
- Clear definitions, answer-first paragraphs, and extractable facts.
- Authority signals: citations, author bios, publisher credibility, original data.
- Structural readability: concise headings, lists, tables, FAQs.
- AI crawler access: robots.txt handling for GPTBot, ChatGPT-User, ClaudeBot, PerplexityBot, Bytespider, Google-Extended, CCBot.
- `llms.txt` or similar AI-readable site guidance when relevant.

Use for visibility in:

- ChatGPT.
- Perplexity.
- Google AI Overviews and AI Mode.
- Other answer engines.

## `seo-hreflang`

International SEO audit, validation, and generation.

Check:

- Correct language and region codes.
- Self-referencing hreflang.
- Reciprocal links between alternates.
- `x-default` where appropriate.
- Canonical and hreflang consistency.
- Matching URLs for translated or localized pages.
- No broken, redirected, noindexed, or canonicalized-away hreflang targets.

Output:

- Hreflang issue table.
- Corrected hreflang snippets.
- International targeting recommendations.

## `seo-images`

Image optimization analysis.

Check:

- Alt text quality and relevance.
- Decorative versus informative image handling.
- File size and compression.
- Modern formats: WebP, AVIF where supported.
- Responsive images: `srcset`, sizes, correct dimensions.
- Lazy loading for below-the-fold images.
- CLS prevention through width/height or aspect ratio.
- CDN and caching usage.
- Image sitemap or image metadata where relevant.

## `seo-page`

Deep single-page SEO analysis.

Review:

- Title tag.
- Meta description.
- H1/H2 structure.
- URL slug.
- Search intent fit.
- Content quality and E-E-A-T.
- Internal links and anchor text.
- External citations.
- Schema opportunities.
- Image SEO.
- Mobile UX signals.
- Performance indicators.
- Conversion relevance.

Use for landing pages, blog posts, product pages, campaign pages, and mobile app landing pages.

## `seo-plan`

Strategic SEO planning for a new or existing website.

Include:

- Current-state summary.
- Business goals and target audience.
- Competitor landscape.
- Keyword and topic strategy.
- Content pillars and page types.
- Technical foundation work.
- Schema and AI search readiness.
- Link/internal linking strategy.
- 3, 6, and 12-month roadmap.
- KPI framework.

## `seo-programmatic`

Programmatic SEO planning and audit for pages generated at scale from structured data.

Use for:

- Location pages.
- Category pages.
- Comparison pages.
- Template-driven directories.
- Pages generated from product, market, city, or topic datasets.

Quality gates:

- Each page must have unique user value.
- Avoid city-name-only or keyword-swap pages.
- Avoid competitor alternative pages without real comparison data.
- Avoid index bloat from low-value pages.
- Require human review and unique data where possible.
- Control sitemap inclusion, canonicals, noindex rules, and crawl budget.

## `seo-schema`

Detect, validate, and generate Schema.org structured data, JSON-LD preferred.

Common schema types:

- Organization.
- LocalBusiness.
- WebSite.
- WebPage.
- Article.
- FAQPage where eligible.
- Product.
- SoftwareApplication.
- AggregateRating when valid and sourced.
- BreadcrumbList.
- ItemList for roundup pages.

Output:

- `SCHEMA-REPORT.md`: detection and validation results.
- `generated-schema.json`: ready-to-use JSON-LD snippets.
- Recommendation table for missing schema and fixes.

## `seo-sitemap`

Analyze existing XML sitemaps or generate new ones.

Validation checks:

- Valid XML.
- Fewer than 50,000 URLs per sitemap file.
- URLs return HTTP 200.
- Accurate `lastmod` values.
- No deprecated reliance on `priority` or `changefreq`.
- Sitemap referenced in robots.txt.
- Sitemap index used for large sites.
- Split by content type when helpful.
- No non-canonical, noindexed, redirected, or HTTP URLs.
- Compare crawled pages versus sitemap and flag missing pages.

Generate:

- `sitemap.xml` or sitemap index plus split sitemap files.
- `STRUCTURE.md` with site architecture notes.
- URL count and organization summary.

## `seo-technical`

Technical SEO audit across crawlability, indexability, security, URL structure, mobile, Core Web Vitals, structured data, JavaScript rendering, AI crawler management, and IndexNow.

Check:

- robots.txt exists, is valid, and does not block important resources.
- XML sitemap exists, is valid, and is referenced in robots.txt.
- Noindex tags are intentional.
- Important pages are within roughly 3 clicks of homepage.
- Critical content does not require fragile JavaScript rendering.
- Canonical tags are self-referencing where appropriate and do not conflict with noindex.
- Duplicate content, parameter URLs, www/non-www, and trailing slash handling.
- HTTPS, SSL, mixed content, and security headers.
- Clean, descriptive URLs with no unnecessary query parameters.
- Mobile viewport, responsive CSS, touch targets, font size, and horizontal scroll.
- Core Web Vitals: LCP under 2.5s, INP under 200ms, CLS under 0.1, using 75th percentile real-user data where available.
- Structured data format and validation.
- Server-rendered critical SEO elements for JavaScript sites.
- IndexNow support for Bing, Yandex, and Naver where relevant.

AI crawler guidance:

- Blocking `Google-Extended` prevents Gemini training use but does not affect Google Search indexing or AI Overviews.
- Blocking `GPTBot` prevents OpenAI training but does not necessarily prevent ChatGPT browsing via `ChatGPT-User`.
- Consider the AI visibility strategy before blocking AI crawlers.
