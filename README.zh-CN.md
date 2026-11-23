# riscv-isa-manual-cn-data

[English](README.md) | 简体中文

官方 [RISC-V 指令集手册](https://github.com/riscv/riscv-isa-manual) 的中文翻译数据仓库，配合引擎仓库 `riscv-isa-manual-cn` 进行同步、校验与站点发布。

## 目录说明

- `GLOSSARY.md`：中英术语对照表。
- `manifests/`：已同步的上游提交索引（`index.json`）、提交快照（`snapshots/`）与章节结构（`chapters/`）。
- `units/<prefix>/<unit_id>.toml`：各翻译单元文件（状态流转：`untranslated` → `machine` → `approved`）。

## 审校与贡献

1. 直接编辑 `units/<prefix>/<unit_id>.toml`（校对 `zh` 后将 `status` 改为 `"approved"`）或完善 `GLOSSARY.md`。
2. 向 `main` 发起 Pull Request，GitHub Actions 会自动执行数据校验与站点构建检查。
3. 合并至 `main` 后，GitHub Actions 会自动构建并部署更新后的双语阅读器到 GitHub Pages。

如需在审校时本地实时预览页面，请使用 `riscv-isa-manual-cn` 仓库并将 `DATA_DIR` 指向本仓库目录后运行 `bun run dev`。

## 许可协议与署名

本仓库中的中文译文与结构化元数据改编自 RISC-V International 及其贡献者维护的 [RISC-V Instruction Set Manual](https://github.com/riscv/riscv-isa-manual)，依据 [知识共享署名 4.0 国际许可协议（CC BY 4.0）](LICENSE) 发布。
