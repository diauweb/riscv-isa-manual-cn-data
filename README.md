# riscv-isa-manual-cn-data

English | [简体中文](README.zh-CN.md)

Chinese translation data for the official [RISC-V Instruction Set Manual](https://github.com/riscv/riscv-isa-manual), built and published with the engine repository `riscv-isa-manual-cn`.

## Contents

- `GLOSSARY.md`: authoritative English–Chinese terminology glossary.
- `manifests/`: synced upstream commits (`index.json`), per-commit snapshots (`snapshots/`), and chapter structures (`chapters/`).
- `units/<prefix>/<unit_id>.toml`: translation units (`untranslated` → `machine` → `approved`).

## Reviewing & Contributing

1. Edit any translation unit under `units/<prefix>/<unit_id>.toml` (update `zh` and set `status = "approved"` after review) or refine terms in `GLOSSARY.md`.
2. Open a pull request against `main`—GitHub Actions runs validation and verifies the static site build automatically.
3. Merging to `main` builds and deploys the updated bilingual viewer to GitHub Pages.

For local live-reload preview while reviewing, clone the engine repository `riscv-isa-manual-cn` and run `bun run dev` with `DATA_DIR` pointing to this repository.

## License & Attribution

This repository contains Chinese translations and structural metadata adapted from the [RISC-V Instruction Set Manual](https://github.com/riscv/riscv-isa-manual) by RISC-V International and contributors, and is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](LICENSE).
