# Official Blog SEO Skill

A lightweight Codex skill for reviewing and improving blog SEO by referring to official and high-authority documentation.

This skill is intentionally conservative. It does not provide a full SEO suite, keyword research system, ranking predictor, traffic estimator, or automated audit platform. Its purpose is much narrower: help Codex check blog/article SEO decisions against reliable baseline references such as search engine documentation, official search tools, Schema.org, web.dev, MDN, WHATWG HTML, and W3C accessibility guidance.

The skill is advisory by design. It reviews and suggests; it should not override a user's instructions, repository guidance, AGENTS.md, CLAUDE.md, CMS/editorial rules, brand style guides, legal requirements, or other project management documents. If there is a conflict, the user's or project's own instructions take priority, and the SEO point should be presented only as an optional recommendation or tradeoff.

## What This Skill Is

- A compact reference workflow for blog and article SEO.
- A source-grounded checklist for titles, meta descriptions, headings, links, images, alt text, structured data, crawl/index basics, snippets, Core Web Vitals, and HTML semantics.
- A conservative guardrail against common unsupported SEO claims, keyword-density rules, plugin-score chasing, and ranking guarantees.
- A reusable skill that is not tied to one blog platform, CMS, theme, or plugin.
- An advisory reference layer that respects user and project-specific management documents.

## What This Skill Is Not

- It is not an official product from Google, Bing, OpenAI, Schema.org, W3C, WHATWG, MDN, or web.dev.
- It is not a guarantee of ranking, indexing, traffic, click-through rate, rich results, Discover visibility, or AI search visibility.
- It is not a replacement for Google Search Console, Bing Webmaster Tools, PageSpeed Insights, Lighthouse, or the Rich Results Test.
- It is not a third-party SEO framework with aggressive scoring rules or proprietary ranking formulas.
- It is not an instruction hierarchy override for user-provided or project-provided rules.

## Source Position

The skill is written to prefer these source classes:

1. Search engine official guidance, especially Google Search Central and Bing Webmaster Guidelines.
2. Official search tools such as Google Search Console, Rich Results Test, PageSpeed Insights, Lighthouse, and Bing Webmaster Tools.
3. Web standards and platform references such as Schema.org, WHATWG HTML, W3C WAI/WCAG, MDN, and web.dev.
4. CMS or plugin documentation only for implementation details, not as search-engine rules.

When current facts matter, the skill instructs Codex to verify against official pages before making firm claims. This is especially important for structured data eligibility, rich results, spam policies, Core Web Vitals metrics, and search feature behavior.

## Design Philosophy

This skill exists as reference material, not as a flashy automation layer. Every recommendation should be traceable to official or high-authority guidance, or clearly labeled as a heuristic when it is not an official rule.

The intended behavior is:

- prefer people-first content improvements;
- avoid keyword stuffing and artificial density targets;
- keep recommendations accurate, specific, and verifiable;
- separate confirmed issues from assumptions and optional heuristics;
- respect the user's management documents and existing editorial requirements;
- avoid inventing claims, credentials, dates, rankings, or performance data.

## Repository Structure

```text
official-blog-seo-skill/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── blog-content.md
    ├── performance.md
    ├── search-official.md
    ├── structured-data.md
    └── web-standards.md
```

## Installation

Install it as a Codex skill from this GitHub repository, or place the folder under your local Codex skills directory.

The skill name is:

```text
official-blog-seo
```

Example prompt:

```text
Use $official-blog-seo to review this blog post against official SEO, structured data, performance, and accessibility guidance.
```

## License

MIT License. See [LICENSE](LICENSE).
