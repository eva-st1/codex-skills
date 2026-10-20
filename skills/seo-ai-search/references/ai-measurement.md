# AI visibility, measurement, and planning

## Observe answer engines

Build a small prompt set from real discovery, comparison, and decision questions. Include non-branded prompts; brand-only prompts distort discovery visibility. Establish engines and locales from task context. Choose repeat count and coverage appropriate to the decision and tools; one response does not represent an engine's overall behavior.

Use actual responses from the named surface or supplied captures. A generic search tool cannot prove how ChatGPT, Claude, Gemini, Perplexity, AI Overviews, or AI Mode answered. If the surface is inaccessible, deliver a prompt/test plan and mark results unmeasured.

Record each observation:

`Timestamp/timezone | Engine/surface/model if known | Search mode | Country/language | Exact prompt | Run ID | Brand mentioned | Owned URL cited | Third-party brand citation | Competitor mentions | Cited URLs | Capture/source | Error/limitation`

Retain raw responses locally when allowed. Distinguish plain mentions, citations to owned pages, third-party pages mentioning the brand, and recommendations. Confirm citations are present and relevant; mark ambiguity separately. Separate queries where no AI Overview appeared from triggered overviews without the brand.

Calculate sample metrics explicitly:

- Mention rate = valid observed responses mentioning the brand / valid observed responses.
- Owned citation rate = valid observed responses citing an owned URL / valid observed responses.
- For triggered features, also report citations / observed triggered responses and trigger count.
- For share of voice, define competitors and whether the unit is responses, mentions, or citations; keep the definition stable.

Exclude failed/unavailable runs from denominators and report their count. Break out engines and intent; avoid averaging incompatible surfaces. Keep prompts, locale, search settings, and sampling comparable across periods. Sample frequency is descriptive, not a causal estimate or guaranteed population rate.

## Optimize for useful retrieval

Inspect cited pages and missing information before drafting. Improve direct answers, accurate entity/business facts, clear comparisons/limitations, primary evidence, accessible text, relevant internal links, and supported structured data. Treat format and source additions as testable hypotheses.

Google AI features use ordinary search eligibility and useful-content practices. No special AI file or schema is required; inclusion is not guaranteed. Search Console aggregates these features into Web performance; do not fabricate separate AI Overview traffic from an ordinary export. See [Google's AI guidance](https://developers.google.com/search/docs/appearance/ai-features).

Check search-crawler access independently of training permission. [OpenAI documents](https://developers.openai.com/api/docs/bots) independent OAI-SearchBot and GPTBot controls. Read current engine documentation and inspect robots/CDN responses before proposing changes. Preserve chosen training permissions. Crawler access does not promise citations.

Treat llms.txt and experimental formats as optional consumer-specific experiments when justified. Never require them for an ordinary audit or promise ranking gains. Keep useful information available to users and crawlers.

## Search and business performance

Align periods, timezone, country/device filters, URLs, and keyword sets. Preserve missing rows and tracking limits; absence from a top-N export is not an exact rank of N+1. Search Console average position differs from an instantaneous tracked rank.

Compute CTR from total clicks / total impressions; don't average row CTRs. Do not sum page and query reports as independent traffic. Report anonymization, export limits, or sampling where material. Separate branded/non-branded demand and segment templates/journeys when useful.

Low CTR at strong average positions is a diagnostic lead. Check actual features, intent, title/snippet fit, device mix, seasonality, and position distribution before attributing it to zero-click behavior. Search Console alone does not prove which feature absorbed clicks.

For volatility, compare equivalent snapshots, count affected queries, and inspect site changes and tracking anomalies. Verify alleged updates against [Google's Search status history](https://status.search.google.com/products/rGHU1u87FJnkP6W2GwMi/history). Coincidence is not proof of cause. Explain investigation steps instead of prescribing blanket rewrites.

Track conversions and qualified leads/revenue with available analytics definitions. AI referrals may be incomplete or unattributed; mentions are not conversions. Avoid attributing gains to a change without appropriate comparison and explicit limitations.

## Reports and roadmaps

Summarize business outcomes, comparable movement, strongest evidence, top actions, and decisions needed. Keep raw tables separate when they obscure the decision. Use healthy / needs work / critical / unmeasured for technical eligibility, content fit, authority evidence, and AI visibility, with reasons; these are internal assessments, not engine scores.

A 30-day plan sequences prerequisites, fixes, useful content, and comparable remeasurement. Derive quarterly deliverables/capacity from goals and resources. Give each an owner role, dependency, success measure, and review date. Use scenarios where forecasts need assumptions; avoid compulsory placement/publishing quotas.

For requested recurring analyses, reuse definitions and baselines. Possible cadence: weekly meaningful ranking/citation changes, monthly outcomes/fixes, quarterly strategy review. Creating an automation or contacting a publisher requires a user request; an audit does not implicitly schedule or send anything.
