# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repo status: empty scaffold

As of this writing the repository contains only a `.gitignore` and a single `Initial commit`. There is **no source code, no build system, no documentation, and no tests yet**. Do not infer architecture that is not actually here — when the first real files land, this file should be rewritten to describe them.

## What the .gitignore tells us

The `.gitignore` is the **Adventure Game Studio (AGS)** template. Ignored paths include `_Debug/`, `Compiled/`, `AudioCache/`, `_OpenInEditor.lock`, `Game.agf.user`, `*.crm.user`, `Game.agf.bak`, `backup_acsprset.spr`, `~aclzw.tmp`, `game28.dta`, `*.exe`, and `warnings.log`.

This strongly implies the repo will host an **AGS adventure game project** ("Bank"). Expect future contents along these lines:

- `Game.agf` — the AGS project file (XML; the canonical project manifest).
- `*.asc` / `*.ash` — AGS Script source / header pairs (one per room or module).
- `*.crm` — compiled room files (binary; check in alongside their script).
- `acsprset.spr` — sprite set (binary).
- `AudioCache/` — derived; ignored.
- `Compiled/` and `_Debug/` — build outputs; ignored.

AGS games are normally built and edited inside the AGS Editor (Windows GUI). There is no command-line build in the standard AGS toolchain, so until someone adds custom tooling, expect that "build" means opening `Game.agf` in the AGS Editor and pressing F5 / F7. If the user asks you to compile from the CLI, ask them which toolchain they want — there is no convention to fall back on.

## When real content lands

When the first source files appear, replace this file's body with a real overview: the room/module layout, where the dialog scripts live, any custom Python/JS tooling for asset pipelines, and the actual build/run commands. Until then there is nothing project-specific to follow.
