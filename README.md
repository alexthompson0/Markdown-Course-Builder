# Markdown Course Builder

A solo project to scaffold and organize Markdown-based course content into a clean folder structure with simple metadata, TOC generation, and export helpers.

This is a personal, nights-and-weekends build. No runtime required — it focuses on structure, scripts, and docs to outline how a course would be authored and shipped.

## Features
- Course manifest (`course.yaml`) with title, description, and module ordering
- Lightweight CLI (`mcb`) to scaffold modules/lessons and generate a `TOC.md`
- Export helpers to bundle selected lessons into a single `export.md`
- Lint rules for front‑matter and filename conventions

## Quick Start
```sh
# list commands
./scripts/mcb help

# scaffold a module and a lesson
./scripts/mcb add-module "Foundations"
./scripts/mcb add-lesson foundations "What is Markdown?"

# regen TOC
./scripts/mcb gen-toc

# export a subset
./scripts/mcb export foundations getting-started > export.md
```

No build required. Scripts are POSIX shell and safe to read.

