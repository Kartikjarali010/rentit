---
name: bye-bye
description: "Triggers when the user says bye, goodbye, bye bye, see you, see ya, cya, done for today, wrapping up, that's it for now, ending the session, good night, talk later, /bye-bye, or any other sign-off. Performs the full end-of-session ritual: writes the session log to the brain wiki, updates Claude memory files, captures any decisions or learnings, and gives a clean summary of what was saved. Always run this before the session closes — it is the last thing that happens every time."
---

# Bye-Bye — End of Session Ritual

When the user says bye (in any form), run this ritual completely before responding. Do not skip steps. Do not summarize and stop early. Every step is required.

## Step 1 — Write the session log

Write to `/Users/kartik/Documents/projects/brain/wiki/sessions/YYYY-MM-DD-<slug>.md`

Use today's date. Slug = 2-3 words describing the main topic (e.g. `founder-validation`, `auth-bug-fix`, `marketing-plan`).

```markdown
---
title: <Topic> — YYYY-MM-DD
type: session-log
date: YYYY-MM-DD
tags: [relevant, tags]
---

## What we worked on
One paragraph. What was the main task or discussion this session?

## What was built / changed
Bullet list — be specific:
- Files created or modified (with paths)
- Code written or changed
- Decisions implemented
- Skills invoked and what they produced

## Decisions made
| Decision | Why |
|----------|-----|
| ... | ... |
Only include non-obvious decisions worth remembering in a future session.

## Skills invoked
Which skills triggered and what they contributed.

## Brain wiki updates
Which wiki pages were created or updated this session.

## Memory updates
Which memory files were updated and what was added.

## Continue next time
Numbered list. Specific enough to act on immediately without re-reading the whole session:
1. ...
2. ...
```

## Step 2 — Update brain/index.md

Add or update the row in the Sessions table:
```
| [[sessions/YYYY-MM-DD-<slug>]] | <one-line summary> | YYYY-MM-DD |
```

Also update the "Last session" line at the top of index.md.

## Step 3 — Update brain/log.md

Append:
```
## [YYYY-MM-DD] session | <slug>
- Brief bullet list of the 3-5 most important things that happened
```

## Step 4 — Update Claude memory files

Memory lives at `/Users/kartik/.claude/projects/-Users-kartik/memory/`.
Read `MEMORY.md` to see what exists. Then:

**Update existing memories if anything changed:**
- Did the user's goals change? → update `user_kartik.md`
- Did a new rule or preference emerge? → update or create a `feedback_*.md`
- Did the project state change? → update `project_skills_setup.md` or create new `project_*.md`
- Did the user reference an external resource? → create `reference_*.md`

**Create new memories if something genuinely new and durable was learned:**
- A new preference or rule → `feedback_<topic>.md`
- New project context → `project_<topic>.md`
- New resource → `reference_<topic>.md`

Memory format:
```markdown
---
name: <name>
description: <one-line, used to judge relevance in future sessions>
type: user | feedback | project | reference
---
<content>

**Why:** <reason>
**How to apply:** <when this matters>
```

Always update `MEMORY.md` index if a new memory file was created.

## Step 5 — Update any stale brain wiki pages

If anything discussed this session makes an existing wiki page outdated:
- Update the page
- Mark stale claims with `> 🕐 POSSIBLY STALE:`
- Update `index.md` and `log.md`

## Step 6 — Confirm and say bye

Output a brief, clean summary:

```
Session saved ✓

📓 Log: wiki/sessions/YYYY-MM-DD-<slug>.md
🧠 Memory: <list what was updated, or "no changes">
📚 Wiki: <list pages updated, or "no changes">

Continue next time:
1. ...
2. ...

See you! 👋
```

Keep it short. The user is leaving — don't make them read a wall of text.
