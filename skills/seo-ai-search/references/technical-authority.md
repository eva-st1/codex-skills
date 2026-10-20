# Technical health and authority

## Access, indexing, and URL relationships

Inspect status/redirect behavior, robots.txt, meta/X-Robots-Tag directives, canonical targets, rendered main content, sitemap membership, and internal discovery. Public inspection establishes technical eligibility; actual indexing and Google's selected canonical require Search Console evidence. Site-search results are not a complete index report.

Cross-check redirect, canonical, sitemap, and hreflang signals. Canonicals should represent intended equivalent content; localized alternatives need appropriate reciprocal relationships. Identify conflicts from actual responses/page data. Similar text alone does not prove two pages should canonicalize together.

Distinguish crawl from index controls: robots.txt can prevent a crawler from seeing noindex; canonicals are consolidation signals, not guaranteed directives. Before restrictions, redirects, or removals, map affected patterns, valuable URLs, dependencies, and verification/rollback. Do not apply broad rules merely because URLs have parameters or pagination.

Investigate crawl budget when scale, server load, discovery delays, or logs justify it. Crawl exports describe a crawler's traversal, not Google's crawl frequency. Search Console crawl stats and verified server logs support bot-behavior findings. Explain wasted patterns with evidence; avoid universal monthly crawl targets.

## Structured data

Compare structured data with visible facts, then check syntax and current feature requirements. Schema.org validity, Google feature eligibility, and actual rich-result appearance are separate checks.

Choose types that describe the real entity/page. Never fabricate offers, prices, ratings, reviews, or author identities. Multiple nodes can be valid; duplication matters when facts or entity identifiers conflict. Validate generated JSON-LD and use an available structured-data/rich-result validator for the intended consumer.

Check current documentation before promising FAQ, HowTo, review, or other search treatments. Useful question/answer content does not imply rich-result eligibility. There is no special Google AI schema requirement.

## Performance

Use field data for Core Web Vitals assessment and lab data/traces for diagnosis. State source, date/window, device, and URL-level versus origin-level scope. Evaluate available field LCP, INP, and CLS at the 75th percentile, not the median of unrelated pages.

Baseline good thresholds checked on 2026-10-05: LCP <= 2.5 s, INP <= 200 ms, CLS <= 0.1. Recheck [the primary reference](https://web.dev/articles/defining-core-web-vitals-thresholds) when applying them. Missing field data means unavailable, not passing or failing. Lab TBT is a diagnostic, not field INP.

Identify the actual slow resource, interaction, or shift from traces. Label unsupported causes as hypotheses. Group shared bottlenecks by template and prioritize affected important pages. Estimate gains only from measured evidence; verify under comparable conditions and allow time for field data to reflect changes.

## Internal links

Inspect crawlable links, descriptive anchors, click depth, destination status, and relevant context. Reconcile a crawl with sitemap, analytics, or known URL inventories before claiming orphan pages; a crawler alone may never discover them.

Recommend concrete source URL/section -> target URL/anchor additions helping readers discover important material. Explain importance through business value and navigability. Avoid fixed minimum link counts and claims that useful legal/contact links automatically drain rankings. Base consolidation on page purpose and evidence.

## External authority and anchors

Examine referring-page relevance, editorial context, placement, link attributes, destination health, verified referral outcomes, and signs of link schemes. Label provider authority/traffic estimates as third-party metrics. Low DR, unfamiliar publishers, or unusual anchors alone do not establish harm.

Calculate anchor distributions with explicit denominators and counting units (links, pages, or referring domains). Use niche/context comparisons to investigate patterns; avoid universal safe percentages. Prioritize broken valuable backlinks and legitimate relationship/content opportunities.

Disavow is exceptional. Follow [Google's current criteria](https://support.google.com/webmasters/answer/2648487): substantial artificial/spammy links plus a manual action or likely manual action. A toxicity score is insufficient. If evidence and authorization support it, prepare a reviewable list and account for replacement of an existing submission; never submit as routine cleanup.

Recommend earned coverage based on audience fit, expertise, and observable citation/referral value. Publication prestige does not prove inclusion in training data or a predictable AI-citation weight.
