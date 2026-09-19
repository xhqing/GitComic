# TODO 归档

> 已处理条目归档于此（✅ 已完成 / ✅ 已更新 / ✅ 已放弃 / ✅ 已迁移），正文保留可回溯。编号全局递增、永不复用。T2 自 ProductProducerAgent 归档迁入（2026-09-19 建仓迁移），编号沿用。

## 流水线生产任务

- [ ] **T2** **生产 Git 漫画书试读版（Git-Comic-v1，先试读后全本）**——按 Scout《机会研判报告》执行（记录：2026-09-18 11:47）：

  - **报告位置（唯一权威输入）**：`/Users/xhq/Developer/ProductStrategistAgent/artifacts/git-comic-book-report.md`（`product_id: Git-Comic-v1`；`trend_id: TR-vibecoding-nontech-2026`）。生产前**通读全文**，重点 §2（产品形态与版本顺序）、§5（定价）、§7（风险与对策）。
  - **本次范围：20 页英文试读版，不做全本**（报告 §6 验证优先策略：先试读 X/小红书互动，验证通过再启动全本 80-120 页——全本任务等验证结果另派）。
  - **制作流程（报告 §2 版本顺序决策）**：先用**中文写分镜脚本**定稿（质量最可控），再翻译嵌字出**英文版**；一套分镜双语出稿，中文版暂存不发（等国内 vibe coding 痛点成熟 + 英文版验证后作第二落点）。
  - **内容规格**：
    - 场景驱动：每章一个 vibe coder 真实惨案（AI 改坏 15 个文件 / 误删功能 / 丢几周工作成果），漫画剧情演示 git 怎么救——不是命令手册；
    - 五命令极简主义：commit（存档）/ diff（看 AI 改了什么）/ revert·checkout（后悔药）/ branch（安全试验田）/ .gitignore（保命清单）；
    - 试读 20 页 ≈ 2–3 章，开篇即最痛的惨案（丢工作成果）；
    - AI 生图，固定角色设定词，少角色多场景（画风跨页一致，§7 风险对策）。
  - **同步产出**：8–12 张竖版图卡（Git-Comic-Mini，`product_id: Git-Comic-Mini`，Instagram/小红书规格 1080×1350），从试读章节拆解——引流素材与产品共生（报告 §6）。
  - **验收线**：① 非技术读者 10 分钟能翻完试读并复述核心信息（「git 是 AI 时代的后悔药」）；② 同一角色跨页可识别（画风一致性）；③ 英文文案无语法硬伤（母语级校对）。
  - **产物**：试读 PDF + 图卡包 + 《产品说明》写本项目 `artifacts/`，产品说明**必须带 `product_id: Git-Comic-v1`**（下游 Vendy / Buzz / Echo 归因用）。
  - **生产期间素材与报告如有出入**：以报告为准；报告本身有疑义，回 Scout 项目会话提，不在生产中擅自改规格。

  ✅**已完成**（完成：2026-09-18 12:16）——20 页英文试读 PDF（`product_id: Git-Comic-v1`，0.1.0：封面 + 扉页 + 3 章正文 + 尾页 CTA，五命令全覆盖）+ 10 张图卡（`Git-Comic-Mini`，1080×1350 PNG）+ 《产品说明》（`artifacts/git-comic-spec.md`，含双 product_id、验收记录 6 项、下游接口）；制作链路：中文分镜定稿（`git-comic-v1/storyboard-zh.md`）→ SVG 矢量自绘（本机无 AI 生图通道，角色组件化单一来源，跨页一致性由构建机制物理保证——报告 §7 风险对策的替代落地）→ rsvg-convert 出 PDF/PNG；验收线达成：核心信息三重强化（p15 大字页 / p19 总结页 / p20 定位句）、角色组件复用 + OCR 抽查渲染无字体缺失、全文案逐条审校（濓号统一、术语同词同义）+ lint 文字越界零告警 + pypdf 页数尺寸验证；打包 `git-comic-v1-en-0.1.0.zip` + `git-comic-mini-en-0.1.0.zip`（逐文件比对一致）并完成 Wright→Mason 交接（handoff 追加产品二节 + 双仓 CHANGELOG 各记一条）。全本任务等验证结果另派。详见 CHANGELOG 2026-09-18 条目。（2026-09-19 20:51 注：本条随 GitComic 建仓迁移自 ProductProducerAgent 归档迁入，产品与制作资产现均在 GitComic 仓 `artifacts/`。）
