# Blog SEO Reviewer Skill

A lightweight Codex skill for reviewing and improving blog SEO with conservative, source-grounded guidance.

This skill helps Codex review blog posts against reliable baseline references such as search engine documentation, official search tools, Schema.org, web.dev, MDN, WHATWG HTML, and W3C accessibility guidance. It is intentionally conservative and designed to avoid overstating what SEO guidance can prove.

The skill is advisory by design. It reviews and suggests; it should not override a user's instructions, repository guidance, AGENTS.md, CLAUDE.md, CMS/editorial rules, brand style guides, legal requirements, or other project management documents. If there is a conflict, the user's or project's own instructions take priority, and the SEO point should be presented only as an optional recommendation or tradeoff.

## Quick Start

Use the skill by name:

```text
Use $blog-seo-reviewer to review this blog post against source-grounded SEO, structured data, performance, and accessibility guidance.
```

Typical uses:

- review a draft blog post before publishing;
- check an already published article's title, meta description, headings, links, images, and structured data;
- compare before/after SEO checklist scores after edits;
- separate official guidance from optional SEO heuristics.

## What This Skill Is

- A compact review workflow for blog and article SEO.
- A source-grounded checklist for titles, meta descriptions, headings, links, images, alt text, structured data, crawl/index basics, snippets, Core Web Vitals, and HTML semantics.
- A conservative guardrail against unsupported SEO claims, keyword-density rules, plugin-score chasing, and ranking guarantees.
- A reusable skill that is not tied to one blog platform, CMS, theme, or plugin.
- An advisory reference layer that respects user and project-specific management documents.
- An itemized before/after scorecard for reviews and edits, used only as a diagnostic checklist.

## What This Skill Is Not

- It is not an official product from Google, Bing, OpenAI, Schema.org, W3C, WHATWG, MDN, or web.dev.
- It is not a guarantee of ranking, indexing, traffic, click-through rate, rich results, Discover visibility, or AI search visibility.
- It is not a replacement for Google Search Console, Bing Webmaster Tools, PageSpeed Insights, Lighthouse, or the Rich Results Test.
- It is not a third-party SEO framework with aggressive scoring rules or proprietary ranking formulas.
- It is not an instruction hierarchy override for user-provided or project-provided rules.
- Its scores are not ranking predictions; they only summarize visible evidence against the skill's checklist.

## Scorecard

Reviews include itemized scores from `0` to `5`, with `N/A` for items that are not applicable or not inspectable from the provided evidence.

The default scorecard covers:

- people-first usefulness;
- search intent fit;
- title and SEO title;
- meta description and snippet support;
- URL, slug, and canonical;
- heading structure;
- keyword/topic alignment;
- internal links;
- external citations;
- images, alt text, and captions;
- structured data;
- crawl/index signals;
- performance and Core Web Vitals evidence;
- accessibility-relevant HTML;
- project guidance compliance.

The total score excludes `N/A` items. Scores are diagnostic summaries only; they do not predict ranking, indexing, traffic, CTR, rich results, Discover, or AI search inclusion.

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
- show current and post-edit scores when reviewing or modifying content;
- respect the user's management documents and existing editorial requirements;
- avoid inventing claims, credentials, dates, rankings, or performance data.

## Repository Structure

```text
blog-seo-reviewer-skill/
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

Install it as a Codex skill from this GitHub repository:

```text
git@github.com:siamakerlab/blog-seo-reviewer-skill.git
```

Or place the skill folder under your local Codex skills directory.

The skill name is:

```text
blog-seo-reviewer
```

## License

MIT License. See [LICENSE](LICENSE).
