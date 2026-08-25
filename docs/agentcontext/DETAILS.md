# DETAILS

Detail knowledge per concept. **Every section is a jump target** — the index
and all references live in `PROJECT.md`. This file is never read fully; it is
opened at the matching section.

Therefore: sections are readable on their own, carry an as-of date, and
contain the **reasoning** behind a decision — not just the result.

**A section is the current state, not a chronology.** A new insight *replaces*
the outdated statement and the as-of date moves with it.

**Gotchas:** write the compact fact that keeps the mistake from happening
again, not the story of how it was found.

Rule of thumb for "does this belong here?": Would a new collaborator need
this information to continue working at this one spot? Then here. Do they
need it to know where they are at all? Then PROJECT.

---

## Task protocol

*(as of 2026-08-25)*

One task = one file, one clear outcome, one solution folder.

```
tasks/2026-08-25-fizzbuzz.md          written by Claude, before the task starts
solutions/2026-08-25-fizzbuzz/        written by Henry, files as he likes
```

Same date-slug on both sides, so a task without a solution is visible as a
gap and a solution without a task cannot happen. Multiple tasks a day are fine
— the slug separates them.

A task file holds: what the code must do, how Henry can tell it worked, and
nothing about how to build it. After Henry submits, the reviewing session
appends its review to the **same task file** under a `## Review` heading —
not a new file, so a task and its verdict never drift apart.

Why folders instead of a log file: the record is a byproduct of doing the
work, not a second thing to maintain. A file that must be updated after every
task is a file that stops being updated.

`HISTORY.md` deliberately does not mirror this: it logs changes to the repo
itself. The dated task files already *are* the training chronology, and a
second copy of it would be a second thing to keep in sync.

---

## Learning target

*(as of 2026-08-25)*

The destination is being able to write, by hand, the kind of backend service
Henry works on professionally: FastAPI endpoints, Pydantic models and
validation, service-layer functions with clean boundaries.

Path is deliberately not planned upfront. Starting point is generic, easy
Python — plain functions, data structures, control flow — because the gap to
close first is *writing at all*, not framework knowledge. The concrete
curriculum gets derived once a handful of solutions have shown where the real
weak spots are, and is written to `docs/agentcontext/plans/` when it exists.

Explicitly out of scope: frontend, deployment, and building any working
product in this repo.

---

## Weak spots

*(as of 2026-08-25)*

Empty on purpose — the landing zone for what reviews reveal: concepts Henry
reaches for and misses, idioms he doesn't use yet, mistakes that repeat.
This section drives task selection once it has content.

---

## Glossary

Terms that carry a more precise meaning in this project than in everyday use.

| Term | Meaning here |
|------|--------------|
| Task session | A short, often fresh chat that poses one task, waits, reviews. Distinct from the repo session that maintains this scaffold. |
| Model solution | Code written by Claude, allowed only after Henry submitted his own attempt and explicitly asked. Never replaces his file. |
