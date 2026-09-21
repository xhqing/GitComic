<div align="center">

<img src="assets/logo.svg" width="640" alt="GitComic logo" />

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Version](https://img.shields.io/badge/Version-0.2.1-blue)
![Type: Digital Product](https://img.shields.io/badge/Type-Digital%20Product-F05032)
![Languages: EN + ZH](https://img.shields.io/badge/Languages-EN%20%2B%20ZH-2A9D8F)

</div>

# GitComic — 用漫画讲明白 Git

> **面向 AI 时代非技术人群的漫画式 Git 入门数字产品线。**
> 由 [Wright](https://github.com/xhqing/ProductProducerAgent)（[xhqing AI agent 团队](https://github.com/xhqing)的数字产品制作人 agent）生产；本仓库是 ProductProducerAgent 的子项目。

[English](README.md)

---

## 产品线

**Git: The Comic — Your Undo Button for the AI Era**（英文版名）/《Git 漫画书：AI 时代的后悔药》（中文版名）——面向 vibe coding 非技术用户（让 AI 写代码但不懂版本控制的创业者、独立工作者、产品 / 设计 / 运营岗）的漫画式图文电子书。当前交付物（0.2.1，试读验证阶段）：

| 产品 | product_id | 形态 |
|---|---|---|
| Git: The Comic（试读） | `Git-Comic-v1` | 20 页试读 PDF，英文版与中文版各一套 |
| Git-Comic-Mini（图卡包） | `Git-Comic-Mini` | 10 张竖版图卡（1080×1350，Instagram / 小红书规格），英文版与中文版各一套 |

策略：验证优先——先发 20 页试读测互动，验证通过再启动全本（80–120 页，等验证结果另派任务）。

## 获取试读版（GitHub Releases）

试读版成图以 zip 附件形式发布在 [GitHub Releases](https://github.com/xhqing/GitComic/releases)——图片裸文件不进 git 仓库，保持仓库轻量。**中文版与英文版各自独立演进版本号**：Release tag 用分语言前缀（`zh-v*` / `en-v*`），中文版发新版不强制英文版跟随。当前：中文版 v0.2.1；英文版正在更新中，将在自己的 tag 上发布。

## 为什么仓库里几乎看不到产品文件

产品本身（制作资产、成品 PDF、图卡、交付 zip、《产品说明》）都在本仓库的 **`artifacts/` 目录下，该目录被 .gitignore 有意忽略**：付费产品不进公开仓库，免费的试读图片也不以裸文件形式进 git 历史——公开分发改走 GitHub Release 附件（见「获取试读版」）。《产品说明》（`artifacts/git-comic-spec.md`，仅存本机）里有 product_id、定价、交付方式、验收记录与流水线接口。git 跟踪的是产品线的文档与记录。

## 制作方式

先写中文分镜定稿 → 一套分镜出两个语言版本（英文 / 中文结构同构、语义对齐）。插画管线：**Agnes AI** 底图（角色基准图多图合成锁定跨页一致性）+ SVG 矢量排版嵌字层（对话气泡 / 旁白 / 终端框）→ Chrome headless 打印 PDF（单语言约 5.5MB）、rsvg-convert 出图卡 PNG。完整细节见本机《产品说明》。

## 流水线位置

① Scout 研判 → ② **Wright 生产（本仓库）** → ③ Mason 建阵地与支付 → ④ Buzz 引流 → ⑤ Vendy 上架成交 → ⑥ Echo 归因（`product_id`）

## License 与署名

- 项目地址：https://github.com/xhqing/GitComic
- Copyright (c) 2026 All Contributors. 仓库文档以 [MIT](LICENSE.md) 许可。
- 产品内容本身（PDF、图卡、分镜与源资产）**不在**该开源许可范围内——它们是商业交付物；试读版图片包经 GitHub Release 分发，但许可范围不变（不开源）。
- 引用本项目时请保留版权声明并注明出处。
