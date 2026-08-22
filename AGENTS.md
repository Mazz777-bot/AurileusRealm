# Repository Guidelines

## Project Structure & Module Organization

This repository is an artifact-complete Codex v2 pet project rather than an application source tree. Preserve provenance and QA files with the finished package. `decoded/` holds approved generated strips and cardinal anchors. `frames/` holds the extracted per-state animation cells and `frames-manifest.json`. `final/` contains assembled atlases and deterministic validation output. `package/` is the install-ready deliverable. Generation prompts live in `prompts/`, source art and layout guides in `references/`, and visual plus machine-readable review evidence in `qa/`.

Treat `package/pet.json` and `package/spritesheet.webp` as an inseparable release pair. The extended atlas in `final/spritesheet-extended.webp` is the source of that packaged spritesheet. Do not remove intermediate images merely because the package exists; they are required to reproduce and audit the result.

## Validation Guidelines

Before accepting a changed package, inspect `qa/run-summary.json` and `final/validation-extended.json`. Both must report `ok: true`. The extended validation must describe an RGBA WebP measuring 1536 by 2288, arranged as 8 columns and 11 rows with `sprite_version_number` 2, no validation errors, and no warnings. Review `qa/contact-sheet-extended.png` and the GIFs under `qa/previews/` after any visual change. Directional changes also require reviewing `qa/look-directions.png`, `qa/direction-semantics.json`, `qa/direction-blind-validation.json`, and `qa/look-continuity.json`.

No build or test command is stored in this repository. Do not invent one or hand-edit an atlas to simulate a validated generation run.

## Commit Guidelines

Keep commits focused on one regenerated state, QA correction, packaging update, or documentation change. Include updated validation and review artifacts in the same commit as any spritesheet or frame changes so the repository never records an unverified package state.
