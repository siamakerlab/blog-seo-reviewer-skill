# Web Standards and Accessibility Reference

Use this reference for HTML semantics, accessibility-adjacent SEO, image alt text, and link behavior.

## Primary Sources

- WHATWG HTML standard for HTML semantics.
- MDN Web Docs for practical HTML element guidance.
- W3C WAI/WCAG for accessibility guidance.
- Schema.org for vocabulary definitions.

## Official URLs

- WHATWG HTML: https://html.spec.whatwg.org/
- MDN HTML elements reference: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements
- MDN image alt text guidance: https://developer.mozilla.org/en-US/docs/Web/API/HTMLImageElement/alt
- W3C WAI images tutorial: https://www.w3.org/WAI/tutorials/images/
- WCAG 2 overview: https://www.w3.org/WAI/standards-guidelines/wcag/
- Schema.org: https://schema.org/

## HTML Semantics

- Use headings to represent document structure.
- Use lists, tables, figures, captions, and code blocks when they reflect the content.
- Avoid using headings or tables purely for visual styling.
- Use meaningful link text that works out of context when possible.

## Alt Text

- Informative images need alt text that describes the image and its role in context.
- Decorative images should have empty alt text or be hidden from assistive technology.
- Do not stuff keywords into alt text.
- If a nearby caption fully describes the image, alt text can be concise but should still serve non-visual users.

## Links

- Anchor text should describe the destination or action.
- External links to official/reference sources are useful when they support factual claims.
- `target="_blank"` is a UX choice; when used, include `rel="noopener"` for security.

## Tables and Code

- Use tables for comparison data, not layout.
- Code blocks should be syntactically clear and relevant to the article.
- Avoid screenshots of code when text code blocks would be more accessible and searchable.

## What to Flag

- missing alt on informative images
- meaningless anchors
- heading order that obscures article structure
- inaccessible image-only explanations
- unsupported claims without citations
