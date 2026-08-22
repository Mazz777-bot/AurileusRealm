# Aurileous's Realm

This repository is Aurileous's Realm: the complete, validated Goldsmiths lion pet project for Codex.

The install-ready Codex v2 package is in `package/`. Its `spritesheet.webp` is an 8-by-11 atlas with 192-by-208 cells, and `pet.json` declares `spriteVersionNumber: 2`.

Project sources and evidence are retained alongside the package:

- `decoded/` contains selected generated source strips and look-direction anchors.
- `frames/` contains extracted animation frames and their manifest.
- `final/` contains assembled standard and extended atlases plus validation results.
- `prompts/` and `references/` preserve generation inputs and layout guides.
- `qa/` contains contact sheets, animated previews, direction checks, and the run summary.

The authoritative completion record is `qa/run-summary.json`. The final v2 atlas validation is `final/validation-extended.json` and should retain `"ok": true` with no errors or warnings.
