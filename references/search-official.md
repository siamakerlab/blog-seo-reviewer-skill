# Search Official Reference

Use this reference for crawl/index, search-result display, and search-engine policy questions.

## Primary Sources

- Google Search Central documentation:
  - SEO Starter Guide
  - Search Essentials
  - Spam policies
  - How Google Search works
  - URL inspection and Search Console help
  - Image SEO and title/snippet documentation
- Bing Webmaster Guidelines and Bing Webmaster Tools documentation.

## Crawl and Index Basics

- A page generally needs to be discoverable, crawlable, indexable, and useful to appear in search results.
- `robots.txt` controls crawling, not indexing by itself.
- `noindex` is the appropriate signal for excluding a page from search results, but the crawler must be able to see it.
- Canonical links are signals, not absolute directives.
- Sitemaps help discovery and update signaling; they do not guarantee indexing.

## Search Result Presentation

- Search engines may choose their own title links and snippets.
- Title and description should accurately describe the page; they are display aids and relevance signals, not guarantees.
- Avoid boilerplate duplicate titles/descriptions across many posts.

## Policy Checks

Flag issues when evidence exists:

- keyword stuffing
- hidden text or hidden links
- cloaking
- doorway pages
- scraped or mass-generated content without added value
- misleading structured data
- link spam
- affiliate or promotional content without independent value

## Verification Guidance

Use official tools when available:

- Google Search Console URL Inspection for indexing and canonical observations.
- Rich Results Test for eligible structured data.
- PageSpeed Insights / Lighthouse for performance evidence.
- Bing Webmaster Tools for Bing-specific crawl/index observations.

Do not infer penalties, ranking drops, traffic gains, or indexing state without tool evidence.
