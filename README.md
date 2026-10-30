# ref-film-to-storyboard-prompt

- Turn "客户指着一支对标视频说要这个" into two deliverables — (1) a production-ready storyboard (逐镜表 + 参考截图 + 动效描述 + 每镜标 diffusion / code-gen / AE 一次性 / 素材 + 复现稳定性 + 可直接用的 diffusion 提示词) and (2) one complete, copy-as-a-whole hybrid video-generation prompt (TapVid 类混合模型：程序化图形 + 扩散实拍质感) with rendering-rule routing and hard constraints. The method: 拉片对标视频提机制（不是抄镜头） → 抓官网/brief 提炼品牌内容槽并逐条事实核对 → 定性 + 受众核对 → 坑位/填法 merge → 复现优先的"图形骨架 × 卖点插槽"设计 → 故事板 → 最终 prompt。Use this WHENEVER the user gives a reference/对标/benchmark video (URL 或文件) plus a brand, website, or brief and wants a 宣传片 / 品牌片 / 曝光素材 / 参考样片 / storyboard / 故事板 / 分镜 / video prompt out of it — including "帮我拉片然后写 prompt", "做一个像 X 那样的片子", "给动效师出故事板", "哪些用 diffusion 哪些用 codegen", "批量出素材测卖点" — even if they only ask for one of the two deliverables or don't say "拉片". Do not use for pure teardown with no production intent (that is video-lapian) or for article→explainer prompts with no reference film (that is explainer-video-prompt).

一个 Claude Code skill。来自合集 [claude-skills](https://github.com/Minerva67/claude-skills)。

## 安装

```bash
git clone https://github.com/Minerva67/ref-film-to-storyboard-prompt.git ~/.claude/skills/ref-film-to-storyboard-prompt
```

装好后在 Claude Code 里输入 `/ref-film-to-storyboard-prompt`，或者直接描述任务，符合条件时会自动触发。

## 文件

```
SKILL.md
references/merge-method.md
references/prompt-template.md
references/routing-rules.md
references/storyboard-spec.md
scripts/build_storyboard.py
scripts/scrape_site.py
```
