# Blog SEO Reviewer Skill

A very lightweight skill for reviewing blog posts from a conservative SEO perspective.

This skill is not designed to be a feature-rich SEO automation suite. Its main purpose is to help an agent review blog content by checking reliable baseline guidance from official or high-authority sources, then present cautious, source-grounded suggestions.

In short: it is a small review aid for blog posts, not a ranking tool.

## Purpose

Blog SEO Reviewer exists to help with practical blog post reviews:

- title and SEO title clarity;
- meta description quality;
- heading structure;
- topic and focus keyword alignment;
- internal and external links;
- image alt text and captions;
- structured data basics;
- crawl/index signals visible from the page;
- Core Web Vitals or performance evidence when tool output is available;
- accessibility-relevant HTML checks.

The skill intentionally stays conservative. It prefers official search engine documentation, official search tools, and web standards over third-party SEO folklore or aggressive scoring formulas.

## Source Position

The skill is written around these source classes:

1. Search engine official guidance, especially Google Search Central and Bing Webmaster Guidelines.
2. Official search tools such as Google Search Console, Rich Results Test, PageSpeed Insights, Lighthouse, and Bing Webmaster Tools.
3. Web standards and platform references such as Schema.org, WHATWG HTML, W3C WAI/WCAG, MDN, and web.dev.
4. CMS or plugin documentation only for implementation details, not as search-engine rules.

When current policy or tool behavior matters, the agent should verify against the current official page before making firm claims.

## What This Skill Is

- A compact blog SEO review workflow.
- A source-grounded checklist for common blog post SEO review tasks.
- A conservative reference layer for agents reviewing blog content.
- A small scorecard system for before/after review summaries.
- A reusable skill that is not tied to one specific blog platform, CMS, theme, or SEO plugin.

## What This Skill Is Not

- It is not an official product from Google, Bing, OpenAI, Anthropic, Schema.org, W3C, WHATWG, MDN, or web.dev.
- It is not a full SEO suite.
- It is not a keyword research tool.
- It is not a ranking predictor.
- It is not a traffic or CTR estimator.
- It does not guarantee indexing, ranking, rich results, Discover visibility, or AI search visibility.
- It should not override user instructions, repository guidance, editorial rules, brand style guides, CMS rules, legal requirements, or project management documents.

## Scorecard

Reviews include itemized scores from `0` to `5`, with `N/A` for items that are not applicable or not inspectable from the available evidence.

The scorecard is only a diagnostic checklist. It does not predict rankings.

Default review areas:

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

## Quick Install

The easiest way is to ask your coding agent in plain language:

```text
Install siamakerlab/blog-seo-reviewer-skill from GitHub.
```

You can also phrase it like this:

```text
Install the Codex/Claude skill from https://github.com/siamakerlab/blog-seo-reviewer-skill.git.
```

SSH also works if your environment has GitHub SSH access:

```text
Install the Codex/Claude skill from git@github.com:siamakerlab/blog-seo-reviewer-skill.git.
```

If your agent supports skill installation from GitHub, it should fetch the repository and place the skill in the correct local skills directory.

## Codex Installation

Ask Codex:

```text
Install siamakerlab/blog-seo-reviewer-skill from GitHub.
```

After installation, use:

```text
Use $blog-seo-reviewer to review this blog post.
```

Manual installation is also possible by cloning or copying this repository's contents into a folder named `blog-seo-reviewer` under your Codex skills directory:

```text
~/.codex/skills/blog-seo-reviewer/
```

## Claude Installation

Ask Claude Code or another Claude-based coding agent that supports skills:

```text
Install siamakerlab/blog-seo-reviewer-skill from GitHub.
```

Then use:

```text
Use the blog-seo-reviewer skill to review this blog post.
```

If you install manually, place the repository contents in a folder named `blog-seo-reviewer` inside the skills directory used by your Claude environment. The exact directory may depend on your Claude setup, so prefer the natural-language install request when available.

## Removal

The simplest removal request is:

```text
Remove the blog-seo-reviewer skill.
```

For Codex manual removal, delete the local skill directory:

```text
~/.codex/skills/blog-seo-reviewer/
```

For Claude manual removal, delete the `blog-seo-reviewer` skill folder from the skills directory used by your Claude environment.

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

## License

MIT License. See [LICENSE](LICENSE).
