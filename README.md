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

## Install with Codex

Ask Codex:

```text
Install the skill from https://github.com/eva-st1/codex-skills/tree/main/skills/design-heuristics
```

For SEO & AI Search:

```text
Install the skill from https://github.com/eva-st1/codex-skills/tree/main/skills/seo-ai-search
```

Or clone the repository and copy the skill into your personal skills directory:

```bash
git clone https://github.com/eva-st1/codex-skills.git
cp -R codex-skills/skills/design-heuristics ~/.codex/skills/
```

Then invoke it with:

```text
$design-heuristics review this interface and prioritize actionable improvements
```

Or for SEO & AI Search:

```text
$seo-ai-search audit my website and prioritize SEO and AI search improvements
```

## Structure

Each skill is self-contained under `skills/<skill-name>` and includes its own `SKILL.md`, interface metadata, and any supporting references.

## License

MIT
