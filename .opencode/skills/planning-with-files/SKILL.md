---
name: planning-with-files
description: Use for multi-step builds or edits (5+ steps). Keep a short plan and notes in markdown files in the working directory so progress survives long work. Text-only adaptation, no scripts or hooks.
---

# Planning with files

Adapted (condensed, text-only, no scripts/hooks) from OthmanAdi/planning-with-files, MIT License, Copyright (c) 2026 Ahmad Adi.

Context is volatile. Write important things to disk.

1. Before a task with 5+ steps, create `task_plan.md` in the working directory: goal, phases (`### Phase N: name` with one `**Status:** pending | in_progress | complete` line each), and decisions.
2. Put discoveries in `findings.md`. Put what you did and test results in `progress.md`.
3. Re-read `task_plan.md` before each major decision. Update status after each phase.
4. If a file already exists, read and continue it. Do not overwrite it.
5. Never write secrets or API keys in these files.
6. Finish only when every phase is complete and the result was checked (see verification-before-completion). Delete the three planning files before finishing if the task asks for a clean deliverable.
