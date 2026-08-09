---
name: official-blog-seo
description: Lightweight blog post SEO review and improvement workflow grounded only in official or high-authority sources. Use when Codex needs to assess or improve blog/article SEO, titles, meta descriptions, headings, image alt text, internal/external links, structured data, crawl/index basics, Core Web Vitals, accessibility-relevant HTML, or search-result presentation without relying on third-party SEO folklore, plugin scores, keyword-density rules, or ranking guarantees.
---

# Official Blog SEO

Use this skill to improve blog posts with source-grounded SEO guidance. Treat search engines' official documentation and web standards as the baseline, and treat SEO plugin scores, third-party checklists, and industry heuristics as optional implementation aids only when they do not conflict with official guidance.

## Source Policy

Rely on these source classes, in this order:

1. **Search engine official guidance**: Google Search Central first, Bing Webmaster Guidelines when broad search-engine compatibility matters.
2. **Official search tools**: Google Search Console, Rich Results Test, PageSpeed Insights, Lighthouse, Bing Webmaster Tools.
3. **Web standards and platform references**: Schema.org, WHATWG HTML, W3C WAI/WCAG, MDN, web.dev.
4. **CMS or plugin documentation**: Use only for implementation details inside that CMS/plugin. Do not treat plugin scores as search-engine rules.

Do not claim that a practice is "official SEO" unless it is supported by one of the source classes above. When a claim is common SEO practice but not official, label it as a heuristic.

When current facts matter, verify against the official page before making a firm claim. This especially applies to rich result eligibility, structured data deprecations, Core Web Vitals metrics, spam policies, AI search features, and search tool behavior.

## Reference Routing

Read only the relevant reference file:

- Blog content, title, description, headings, links, images: [references/blog-content.md](references/blog-content.md)
- Crawl/index basics, snippets, canonical, sitemaps, robots, spam policy: [references/search-official.md](references/search-official.md)
- Structured data for articles, breadcrumbs, FAQ/HowTo cautions: [references/structured-data.md](references/structured-data.md)
- Performance and Core Web Vitals: [references/performance.md](references/performance.md)
- HTML semantics, accessibility, alt text, links: [references/web-standards.md](references/web-standards.md)

## Workflow

1. Identify the post goal, audience, search intent, and primary topic. If the user already provides a target query or focus keyword, treat it as a working hypothesis, not proof of demand.
2. Inspect the article body and metadata. Check title, meta description, slug/URL, headings, first paragraph, internal links, external citations, images, alt text, captions, and structured data.
3. Separate findings into:
   - `Confirmed`: directly visible in the provided content, HTML, metadata, or official tool output.
   - `Needs official verification`: depends on current policy/tool behavior or a referenced official page not yet checked.
   - `Heuristic`: common editorial or SEO practice, not an official rule.
4. Prefer people-first improvements: make the post clearer, more complete for its intent, easier to scan, better sourced, and more useful. Do not add keywords just to satisfy density.
5. Preserve the author's voice and factual scope. Do not invent experience, credentials, dates, data, traffic numbers, rankings, or source claims.
6. Recommend concrete edits: replacement title/meta text, heading changes, paragraph improvements, image alt/caption suggestions, internal link opportunities, or schema changes.
7. If asked to edit files, make the smallest content changes needed and keep CMS-specific requirements separate from official SEO requirements.

## Output Contract

For a review, return:

```text
Scope:
Official sources used or needing verification:
Confirmed issues:
Recommended edits:
Heuristics / optional improvements:
Do not do:
```

For direct content improvement, return the revised content plus a short note of official-source-sensitive assumptions that should be verified.

## Guardrails

- Do not promise ranking, indexing, traffic, CTR, Discover, AI Overview, or rich result outcomes.
- Do not use keyword density targets as a quality gate.
- Do not force exact title or meta description lengths. Use concise, descriptive text and mention truncation risk only as a display consideration.
- Do not recommend FAQ or HowTo structured data for rich results without checking current Google eligibility.
- Do not mark up content that is not visible to users.
- Do not treat decorative images as needing keyword-rich alt text.
- Do not cite unofficial SEO blogs as proof when official sources are available.
