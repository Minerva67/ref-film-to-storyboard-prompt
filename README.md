# ref-film-to-storyboard-prompt：客户指着一支视频说「要这种」，怎么做出来

客户发来一支参考视频和自己的官网或 brief，说想要这种感觉的宣传片。这个 skill 把这两样东西变成可以直接开工的故事板和一整段生成提示词。

## 适合什么时候用

- 要做一支像某个参考片那样的片子，手上有参考视频和品牌资料
- 要给动效师出故事板
- 想知道每个镜头该用视频模型生成还是用代码做
- 要批量出素材，测试哪个卖点效果更好

只想分析参考片、不打算制作的话，用 [video-lapian](https://github.com/Minerva67/video-lapian)。

## 你会拿到什么

1. **故事板**：一个 HTML 文件，可以直接发给动效师或制作方。每个镜头写明时间、对应的卖点、参考截图、旁白、画面描述、动效描述、制作方式（视频模型 / 代码 / AE 手做 / 现成素材）和成功率（稳 / 中 / 险）。用视频模型的镜头附完整英文提示词。
2. **一整段英文生成提示词**：可以整段复制，适用于同时支持精确图形和实拍质感的混合生成工具。

## 它怎么做

- 从参考片里提炼 3–6 个可以迁移的手法，而不是逐镜照抄。客户要的是那支片的感觉，不是那支片本身。
- 品牌文案、参数、网址、数字全部来自官网或 brief 原文。找不到来源的内容会删掉，或标为待确认。
- 目标受众按资料里的证据判断，例如 FAQ 在对谁说话、主图里是谁在使用产品。
- 默认采用「固定图形骨架 + 可替换的卖点位」，8–10 个镜头、15–30 秒。真人镜头只用生成模型比较稳定的景别（背影、侧面、俯拍、局部特写），每个镜头都可以单独替换。同一套骨架可以换卖点批量出片，某个镜头生成失败也不用整支重做。

## 需要准备

- 参考视频（链接或文件）
- 官网链接或 brief
- 已安装 [video-lapian](https://github.com/Minerva67/video-lapian)（拉片部分复用它的下载和抽帧脚本），以及 Python 3、yt-dlp、opencv

## 怎么用

- 「这是对标片和我们的官网，帮我出故事板和 prompt」
- 「哪些镜头用 diffusion，哪些用 codegen」

## 包含的文件

- `SKILL.md`
- `scripts/scrape_site.py`：抓取官网文案、色板和素材地址（包括打包在 JS 里的单页应用文案）
- `scripts/build_storyboard.py`：生成故事板 HTML
- `references/`：参考片与品牌的合并方法、逐镜制作方式的判断规则、故事板格式、提示词模板

## 安装

```bash
git clone https://github.com/Minerva67/ref-film-to-storyboard-prompt.git ~/.claude/skills/ref-film-to-storyboard-prompt
```

重启 Claude Code 后，直接描述你的任务就会触发。也可以输入 `/ref-film-to-storyboard-prompt` 手动调用。

更多 skill 见 [claude-skills](https://github.com/Minerva67/claude-skills)。
