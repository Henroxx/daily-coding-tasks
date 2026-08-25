# History

Chronology, ascending: **date | what was done | why.**

**Scope in this repo: changes to the repo itself** — scaffold, structure,
rules, curriculum decisions. Not the training record: which task was solved
when lives in `tasks/` and `solutions/`, and duplicating it here would create a
second place to maintain.

Purpose: nobody should have to reconstruct in which order decisions fell and
what triggered them — it is already written here.

More informative than a git log — git shows *what* changed, this file holds
*why* and *what was learned* — but not longer per entry: **at most 3 lines per
entry.** An entry is a pointer into the past, not a report. The detail belongs
in DETAILS.

This file is **not** read at session start — only when a question about the
past comes up, or when writing something that needs the project's history. It
therefore grows in number of entries over the years, never in entry size.

---

## 2026-08-25

- Repo scaffolded with the agentic-coding methodology (6815a2e) — so a fresh
  task chat can start immediately with full context and none has to be rebuilt.
- Coaching constraint fixed: Claude writes no solution code, tasks and
  solutions live in parallel dated folders. Reason: reading a finished
  solution destroys the skill this repo exists to build.
