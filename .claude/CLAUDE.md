# RentIt — Claude Code Context

## What we're building
RentIt: hyperlocal P2P rental marketplace. Owners list idle items, renters rent per day, platform earns 15–20% commission.

**Stage:** Validation → build. No product exists yet.

## Repo structure
```
rentit/
├── src/              ← app code lives here
├── smtg/             ← founder docs and board assessment
├── startup-brain/    ← living knowledge base (ideas, decisions, validation)
└── skills/           ← Claude Code skills
```

## Skills (auto-trigger — don't wait to be asked)
Skills are in `skills/`. Key ones:

### Business validation
- `founder-board` — board of advisors on the idea
- `founder-competitors` — competitive landscape
- `founder-consumer` — user research simulation
- `founder-cfo` — unit economics and financial model
- `founder-plan` — full verdict

### Dev workflow
- `brainstorming` → `writing-plans` → `subagent-driven-development`
- `ponytail` — minimum code, YAGNI
- `test-driven-development` — RED-GREEN-REFACTOR
- `systematic-debugging` — structured bug investigation
- `impeccable` — UI/design quality

### Meta
- `task-observer` — logs observations, improves skills over time

## Brain
Startup knowledge base at `startup-brain/`. Read `startup-brain/index.md` first each session.

## Rules
- Use `ponytail` on all code — minimum code that fully works
- Use founder skills when discussing ideas, strategy, validation
- Use `impeccable` on any UI work
- Write session logs to `startup-brain/wiki/sessions/` at session end
