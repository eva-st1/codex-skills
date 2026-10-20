---
name: seo-ai-search
description: Audit and improve website SEO and AI search visibility (AEO/GEO), including content, technical health, authority, local discovery, and measured answer-engine citations. Use for search audits, keyword or content planning, on-page optimization, and search performance reports. General copywriting without a search objective is outside this skill.
---

# SEO & AI Search for Codex

Help the right audience discover useful pages through search and grounded AI answers. Tie recommendations to a specific URL, query, audience need, and observable problem. Optimize for qualified visits, useful brand visibility, and business outcomes.

## Scope and intake

Choose the smallest useful mode: audit, research, rewrite, implementation, measurement, or roadmap. An audit request authorizes inspection and recommendations; implement changes when requested. Follow the site's existing product, publishing, and hosting workflow.

Establish the site, business goal, audience, country/language, important pages, and relevant competitors from available context. Ask only for missing details that materially change the work. For AI visibility, identify the engine and search mode being evaluated; ordinary chat and web-grounded search are different surfaces.

Start with public pages or supplied files. Search Console, analytics, crawl, rank, backlink, and performance exports improve coverage but are not prerequisites for a useful public-page review. Request only the data needed for the chosen task. Keep private exports and customer details out of public artifacts and Git.

## Codex execution

- In a repository, inspect the working directory and dirty state, read applicable AGENTS.md instructions, and identify the owning app/template before editing. Preserve unrelated changes. Use existing commands, libraries, components, and test conventions.
- Inspect public pages with available web/browser tools, and local sources with file/search/terminal tools. Discover connectors when the task needs account data; do not assume Ahrefs, Search Console, or another integration is installed. Accept exports as a fallback without requiring a subscription.
- Use browser inspection for rendered content and interactions when they matter. A source-only check cannot establish what users or crawlers receive after JavaScript rendering.
- For implementation, edit the owning source and validate through its normal workflow. Producing a recommendation alone does not finish an implementation request. Publishing, hosting, account writes, or outreach must stay within the user's authorized scope.
- A request for a weekly report is not permission to create a recurring automation. Schedule only when asked, using Codex's available automation tool.
- This is one discoverable skill with selectively loaded references. It needs no Claude Project, uploaded prompt bundle, external coordinator, or separate agent per specialty.

## Evidence discipline

- Label material findings as observed, calculated, hypothesis, or unavailable. Attach a URL, export/date range, response capture, or code location.
- Use live observations or supplied datasets for rankings, search features, competitor coverage, backlinks, traffic, and citations. Missing access is an evidence gap, not proof of absence.
- Never present an imagined answer-engine response as a measured citation. Report engines you cannot inspect as unmeasured.
- Separate vendor metrics (KD, DR, DA, traffic estimates) from first-party analytics. Name the provider and date. Do not invent difficulty scores, ranking probabilities, traffic forecasts, or Google E-E-A-T scores.
- Use supported impact ranges only when inputs and assumptions are explicit. Otherwise prioritize qualitatively by business importance, reach, evidence strength, and effort.
- Recheck current official documentation when feature support, crawler controls, metric definitions, or eligibility matters. Reference links are starting points, not frozen specifications.

## Focused guidance

Load only the relevant reference and section. Combine modes when the request crosses boundaries.

| Task | Reference | Typical deliverable |
| --- | --- | --- |
| Keyword intent, SERP formats, competitor gaps, snippets, content trust, topical clusters, local discovery | [Research and content](references/research-content.md) | Query-to-page map, rewrite, brief, or local fix list |
| Indexability, schema, performance, crawl, canonicals/hreflang, internal links, backlinks and anchors | [Technical health and authority](references/technical-authority.md) | Reproducible issue cards and focused fixes |
| AI citations, low-CTR diagnosis, ranking changes, executive reporting, annual planning | [AI visibility and measurement](references/ai-measurement.md) | Observation matrix, comparable deltas, or roadmap |

Read [Origins and source policy](references/sources.md) when explaining the article adaptation or validating a contested claim.

## Work and delivery

1. Define the decision the work should support and the inspection scope. Sample shared templates plus business-critical pages; disclose coverage rather than claiming a full-site audit from a few URLs.
2. Inspect evidence with available tools or files. If access is unavailable, finish the accessible portion and give the exact next evidence request.
3. Identify the cause or a testable hypothesis. Separate technical access issues, content mismatch, authority gaps, and visibility/measurement gaps.
4. Recommend or implement the smallest useful change. Specify the affected URL/template, section/file, proposed change, and success check. Preserve brand voice and verified business facts.
5. Verify requested edits: rendered output, metadata, links, relevant structured data, and focused repository checks. Distinguish a shipped fix from later indexing or ranking outcomes.

For an audit, lead with the main finding and top three actions. Add a compact prioritized table:

`Priority | URL/query | Evidence | Fix | Expected benefit | Effort | Verification`

Use P0 for observed critical failures blocking important pages, P1 for material business opportunities, P2 for useful improvements, and P3 for experiments. These are task priorities, not search-engine scores. Include confidence where the cause is uncertain. Give a practical 30-day sequence when useful; disclose evidence and coverage limits. A narrow rewrite or fix needs only the relevant output and verification. Link edited files and report the checks actually run.

## Decision guardrails

Make content clearer, more accurate, easier to access, and more useful. Add original evidence and appropriate attribution; never invent credentials, reviews, case studies, test results, or citations.

Treat AI citation improvements as experiments, not guarantees. Special files, schema saturation, arbitrary word counts, fixed anchor percentages, and prestigious publication names are not universal ranking formulas. Recommend a placement partner only when an observed need and the user's context justify it.

Avoid thin location pages, deceptive comparisons, paid-link schemes, or bulk content merely to manipulate rankings. Preserve useful contact and legal navigation. URL removals, crawl/index restrictions, disavow submissions, publishing, and third-party contact must follow existing authorization and the owning workflow.
