# Codex Skills

Reusable skills for practical product, design, and engineering work with Codex.

## Available skills

### Design Heuristics

An evidence-based workflow for reviewing websites, dashboards, mobile apps, forms, screenshots, and prototypes. It turns subjective design feedback into prioritized findings connected to user impact.

The review covers:

- core usability heuristics;
- visual hierarchy and content quality;
- responsive behavior;
- accessibility;
- data-heavy workflows;
- trust, privacy, and safety.

Find it in [`skills/design-heuristics`](skills/design-heuristics).

### SEO & AI Search

A workflow for auditing and improving website SEO and visibility in AI search answers (AEO/GEO). It covers query and content research, technical health, local discovery, authority, and measured AI citations, with recommendations grounded in observed evidence.

Find it in [`skills/seo-ai-search`](skills/seo-ai-search).

### Write LinkedIn Articles

A research-led workflow for professional articles and newsletter editions in the author's demonstrated voice. It combines evidence, a clear point of view, and a useful reader journey without forcing a formula or generic AI phrasing.

Find it in [`skills/write-linkedin-articles`](skills/write-linkedin-articles).

### Website Copywriting

Write, revise, and localize website copy around the visitor's decision, verified business facts, and brand voice. Includes focused guidance for Polish, English, and Norwegian Bokmål, plus review of copy in its rendered context.

Find it in [`skills/website-copywriting`](skills/website-copywriting).

### Create CV

Create and tailor truthful professional CVs and resumes from supplied career evidence. Covers role alignment, market conventions, evidence selection, relevant proof links, text extraction, and rendered-document review.

Find it in [`skills/create-cv`](skills/create-cv).

These skills work from supplied text, files, or accessible sources. They do not require a particular business application, database, or paid account. File rendering, live inspection, and account access depend on the tools available in your environment.

## Install with Codex

Ask Codex:

```text
Install the skill from https://github.com/eva-st1/codex-skills/tree/main/skills/design-heuristics
```

For SEO & AI Search:

```text
Install the skill from https://github.com/eva-st1/codex-skills/tree/main/skills/seo-ai-search
```

For the writing and CV skills, choose the corresponding request:

```text
Install the skill from https://github.com/eva-st1/codex-skills/tree/main/skills/write-linkedin-articles
Install the skill from https://github.com/eva-st1/codex-skills/tree/main/skills/website-copywriting
Install the skill from https://github.com/eva-st1/codex-skills/tree/main/skills/create-cv
```

Or clone the repository and copy the skill into your personal skills directory:

```bash
git clone https://github.com/eva-st1/codex-skills.git
cp -R codex-skills/skills/design-heuristics ~/.codex/skills/
```

Replace `design-heuristics` with another skill's directory name to copy that skill instead.

Then invoke it with:

```text
$design-heuristics review this interface and prioritize actionable improvements
```

Or for SEO & AI Search:

```text
$seo-ai-search audit my website and prioritize SEO and AI search improvements
```

Example requests for the writing and CV skills:

```text
$write-linkedin-articles turn these notes into an article in my established voice
$website-copywriting revise this service page for Polish customers using the supplied business facts
$create-cv tailor my CV to this vacancy without adding unsupported claims
```

## Structure

Each skill is self-contained under `skills/<skill-name>` and includes its own `SKILL.md`, interface metadata, and any supporting references.

## License

MIT
