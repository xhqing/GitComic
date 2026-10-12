<div align="center">

<img src="assets/logo.svg" width="640" alt="GitComic logo" />

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Version](https://img.shields.io/badge/Version-0.2.2-blue)
![Type: Digital Product](https://img.shields.io/badge/Type-Digital%20Product-F05032)
![Languages: EN + ZH](https://img.shields.io/badge/Languages-EN%20%2B%20ZH-2A9D8F)

</div>

# GitComic — Git, Explained in Comics

> **A comic-book product line that teaches Git to non-technical builders in the AI era.**
> Produced by [Wright](https://github.com/xhqing/ProductProducerAgent) (the digital-product producer agent of the [xhqing AI agent team](https://github.com/xhqing)); this repo is a sub-project of ProductProducerAgent.

[简体中文](README_cn.md)

---

## The Product Line

**Git: The Comic — Your Undo Button for the AI Era** (中文版《Git 漫画书：AI 时代的后悔药》) — a comic-style illustrated ebook for *vibe-coding* non-technical users (founders, indie workers, product/design/ops folks who let AI write their code but have no version control). Current deliverables (v0.2.2, preview stage):

| Product | product_id | Form |
|---|---|---|
| Git: The Comic (preview) | `Git-Comic-v1` | 20-page preview artwork (PNG pack), EN & ZH editions |

Strategy: preview-first validation — ship the 20-page preview, measure engagement, then greenlight the full 80–120 page book (a separate task, pending validation results).

## Get the Preview (GitHub Releases)

The preview artwork ships as zip attachments on [GitHub Releases](https://github.com/xhqing/GitComic/releases) — raw image files are deliberately kept out of the git repo to keep it lightweight. The **ZH and EN editions version independently**: release tags use per-language prefixes (`zh-v*` / `en-v*`), so a Chinese-edition release never forces an English one. Current: ZH v0.2.2; EN v0.2.2.

## Why This Repo Tracks So Little

The product itself (source assets, finished PDFs, delivery zips, and the Product Spec) is kept out of git — it lives in this repo's **`artifacts/` directory, which is git-ignored on purpose**: paid products never enter a public repository, and even the free preview images are distributed as Release attachments rather than loose files in git history (see "Get the Preview"). Note: the production source assets that once lived here were removed from this machine on 2026-09-22 by decision — the full book will be produced with a rebuilt pipeline, and those old paths no longer exist. What git tracks here is the product line's documentation and history.

## How It's Made

Chinese storyboard finalized first → one storyboard, two language editions (EN/ZH structurally identical, semantically aligned). Art pipeline: **Agnes AI** base illustrations (character reference images locked via multi-image composition for cross-page consistency) + an SVG typesetting layer for speech bubbles / narration / terminal boxes → Chrome headless prints the PDF (~5.5 MB per language), rsvg-convert renders the PNG page images. Production rule: the book must not depict real brand trademarks (including hand-drawn renditions) — the 0.2.2 pass removed the Apple logo from 9 pages (see the changelog).

## Pipeline Position

① Scout (research) → ② **Wright** (produce, this repo) → ③ Mason (landing + payment) → ④ Buzz (traffic) → ⑤ Vendy (sell & fulfill) → ⑥ Echo (attribution via `product_id`)

## License & Attribution

- Project URL: https://github.com/xhqing/GitComic
- Copyright (c) 2026 All Contributors. Repo documentation is licensed under [MIT](LICENSE.md).
- The product contents themselves (PDFs, card images, source/storyboard assets) are **not** covered by this open license — they are commercial deliverables. The preview image packs are distributed via GitHub Releases, but their license terms stay unchanged (not open-sourced).
- When referencing this project, please keep the copyright notice and cite the source.
