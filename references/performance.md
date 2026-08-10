# Performance Reference

Use this reference for performance and Core Web Vitals checks.

## Primary Sources

- web.dev Core Web Vitals documentation.
- PageSpeed Insights.
- Lighthouse documentation.
- Google Search Console Core Web Vitals report.

## Official URLs

- web.dev Web Vitals: https://web.dev/articles/vitals
- web.dev Core Web Vitals collection: https://web.dev/explore/learn-core-web-vitals
- web.dev Core Web Vitals thresholds: https://web.dev/articles/defining-core-web-vitals-thresholds
- PageSpeed Insights: https://pagespeed.web.dev/
- Lighthouse documentation: https://developer.chrome.com/docs/lighthouse
- Google Search Console Core Web Vitals report: https://support.google.com/webmasters/answer/9205520

## Core Web Vitals

Use current web.dev definitions and thresholds. As of recent guidance, the primary Core Web Vitals are:

- LCP: loading experience
- INP: interaction responsiveness
- CLS: visual stability

Verify current metric names and thresholds before making strong claims, especially if the user asks for latest SEO/performance guidance.

## Blog-Relevant Checks

- Featured/hero image should be appropriately sized and not unnecessarily delayed if it is the likely LCP element.
- Below-the-fold images can use lazy loading.
- Images and embeds should reserve dimensions or aspect ratio to reduce layout shift.
- Avoid excessive third-party scripts that slow interaction or load.
- Use caching, compression, and modern image formats where the platform supports them.

## Evidence Rules

- Do not claim PageSpeed, CrUX, or Core Web Vitals values without measured output.
- Lighthouse lab data is useful for diagnosis, but field data is preferred for user-experience assessment when available.
- Treat performance as user experience and discoverability support, not a guaranteed ranking lever.

## Output Guidance

For each performance recommendation include:

- measured evidence or visible code evidence
- likely user impact
- implementation path
- verification command/tool
