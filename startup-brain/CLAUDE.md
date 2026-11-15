# Startup Brain — Schema
> This is Kartik's dedicated second brain for startup ideas, validation, and company building. It is a satellite of the central brain (`~/Documents/projects/brain/`). Cross-domain decisions and people go in central; deep startup work lives here.

---

## Who this brain belongs to
**Kartik** — building a product/company (early stage, validating)
- Current project: smtg (`~/Documents/projects/smtg/`)
- Central brain: `~/Documents/projects/brain/`

---

## Directory Layout

```
startup-brain/
├── CLAUDE.md          ← this file: schema + rules
├── index.md           ← master catalog — READ THIS FIRST
├── log.md             ← append-only history
├── raw/               ← original docs, screenshots, notes — immutable
│   └── assets/
└── wiki/
    ├── ideas/         ← one page per startup idea (any stage)
    ├── validation/    ← experiments, user interviews, results
    ├── decisions/     ← key decisions with context and rationale
    ├── competitors/   ← competitor research, one page per competitor
    ├── goals/         ← startup goals — OKRs, milestones, targets
    ├── people/        ← cofounders, advisors, investors, potential hires
    └── sessions/      ← one log per Claude session touching startup work
```

---

## Page Format

```yaml
---
title: Page Title
type: idea | validation | decision | competitor | goal | person | session
tags: [tag1, tag2]
status: active | parked | killed | done
created: YYYY-MM-DD
updated: YYYY-MM-DD
---
```

Then: one-paragraph summary → `## Details` → `## Connections` → `## Open Questions`

---

## Idea Page Format

```yaml
---
title: Idea Name
type: idea
status: exploring | validating | building | killed | pivoted
tags: [market, problem]
created: YYYY-MM-DD
updated: YYYY-MM-DD
---
```

Body:
- **Problem:** what problem does this solve
- **Who:** target user/customer
- **Solution:** core mechanism
- **Why now:** why this is relevant today
- **Risks:** biggest unknowns
- **Next step:** one concrete action

---

## Workflows

### NEW IDEA
1. Create `wiki/ideas/<slug>.md`
2. Update `index.md` Ideas table
3. Append to `log.md`: `## [YYYY-MM-DD] idea | <name>`

### VALIDATION EXPERIMENT
1. Create `wiki/validation/<slug>.md` — hypothesis, method, results, conclusion
2. Link to relevant idea page
3. Update idea page status if changed
4. Append to `log.md`: `## [YYYY-MM-DD] validation | <slug>`

### DECISION
1. Create `wiki/decisions/<slug>.md` — context, options, chosen, why
2. Link to relevant idea/goal
3. Append to `log.md`: `## [YYYY-MM-DD] decision | <slug>`

### SESSION (end of every Claude session touching startup work)
1. Write `wiki/sessions/YYYY-MM-DD-<slug>.md`
2. Update `index.md` Sessions table
3. Append to `log.md`: `## [YYYY-MM-DD] session | <slug>`
4. Update central brain's area portal: `brain/wiki/areas/startup.md`

---

## Conventions
- **Status is mandatory** on every idea page — never leave it blank
- **Kill fast** — a killed idea is a valuable record, not a failure
- **Link aggressively** — `[[ideas/slug]]`, `[[decisions/slug]]`
- **Contradict explicitly** — `> ⚠️ CONTRADICTION:` when two pages conflict

---

## Schema Version
v1.0 — 2026-11-15
