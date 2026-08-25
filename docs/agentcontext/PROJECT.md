# PROJECT — Index & State

Entry point for every session: high-level state with references into
`DETAILS.md`, where every concept has its own section. This file stays
scannable; detail knowledge belongs in DETAILS.

This file is read fully every session — that's why it stays short.
Guideline: under 200 lines.

---
# Goal & Scope

Henry writes at least one line of Python by hand every day, to keep and grow
the ability to produce backend code without an agent. The repo is the training
ground and the record: tasks in, solutions out, progress visible over time.
The long-term target is being able to write the kind of backend codebase he
works with professionally — FastAPI and Pydantic services — from scratch,
himself. → DETAILS "Learning target", "Task protocol"

- **Delimitation:** no frontend. No product is built here — nothing in this
  repo needs to keep working, be deployed, or serve anyone. Other languages
  are possible later, but Python is the whole scope for now.
- **Claude writes no solution code** (see `CLAUDE.md` → Core). This is the
  defining constraint of the project, not a preference.
- **Constraints:** daily, and small enough to actually happen. A task that
  takes an hour breaks the habit; the habit is the point.

---
# Status

- Repo scaffolded with the methodology (2026-08-25). Nothing else exists yet:
  no tasks, no solutions, no Python environment.
- Working environment: `~/dev/private_repos/daily-coding-tasks`, branch `main`,
  git is the only backup.
- Henry's current level: working as a developer, writes almost no code by hand
  day to day. Starting point is deliberately easy, generic tasks — not
  FastAPI yet.

> **ASSUMPTION:** Python 3.14 via a project-local venv managed with `uv`, set
> up by Henry himself as his first hands-on exercise. Nothing global.

> **ASSUMPTION:** Solutions stay in the repo permanently and get committed —
> they are the record, so a later session can see what he already solved and
> how. They are never edited by Claude.

---
# To-dos & open decisions

Done items stay as `[x]` with date and **reasoning** — that is the later
answer to "why this way, again?".

- [ ] Henry: set up the venv with `uv` by hand (first exercise).
- [ ] First task from a fresh task chat — generic and easy.
- [ ] Source a pool of exercises (curate or scrape existing sets) so a task
      session doesn't have to invent one from nothing each time.
      → open: which sources, and whether a pool is even needed.
- [ ] Curriculum from "generic Python" toward "FastAPI/Pydantic service" —
      only once a few tasks have shown where the real gaps are. Deliberately
      not planned upfront.
- [ ] Henry will hand over example codebases he works on; they become the
      target shape for later tasks.
- [x] **Claude never writes solution code** (2026-08-25).
      Reason: reading a finished solution destroys the exact skill this repo
      exists to build. → `CLAUDE.md` → Core
- [x] **Two kinds of session: repo chat and task chat** (2026-08-25).
      Reason: task chats stay short and disposable, so the context of the
      maintaining chat is never spent on posing exercises.
      → `CLAUDE.md` → "Two kinds of session"
- [x] **No TESTING.md; HISTORY.md only for repo changes** (2026-08-25).
      Reason: nothing here can regress, so no TESTING. HISTORY logs changes to
      the scaffold and the rules — the training chronology already exists as
      dated task files. → DETAILS "Task protocol"
- [x] **`tasks/` and `solutions/` as parallel folders** (2026-08-25).
      Reason: the pairing and the gaps are visible at a glance, and a task
      file can be written before a solution exists. → DETAILS "Task protocol"

---
# References

- `docs/agentcontext/DETAILS.md` — detail knowledge, jump targets per concept
- `docs/agentcontext/HISTORY.md` — chronology of repo changes, write-only at session end
- `tasks/`, `solutions/` — the training record itself (not agent context)
