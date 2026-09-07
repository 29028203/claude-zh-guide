# Claude 中文指南

## 仓库介绍

本仓库为「Claude 中文指南」的中文资料镜像，收录 Claude中文站 官网相关文章 15 篇（教程与指南 7 篇、版本动态 8 篇），统一整理为 Markdown。每篇文章都保留官网原文链接，可在线阅读，也可 `git clone` 到本地，用于检索、离线阅读或交给 AI 工具做学习总结；内容持续跟随官网更新。

## Claude Code介绍

Claude Code 是 Anthropic 推出的 AI 编程智能体，包含终端命令行工具、桌面应用和 IDE 插件等形态，并支持 Web 与 iOS 端远程委派任务。它直接在本地终端运行，能够理解你的代码库，通过自然语言完成代码生成与修改、执行测试、运行命令、处理 Git 工作流等任务。基于 Sonnet 和 Opus 系列模型驱动，专为真实软件工程任务优化，支持在 VS Code、JetBrains 等 IDE 中以可视化 diff 呈现修改。Claude Code 可调用全部 CLI 工具，从理解百万行级代码库到一键提交 PR，让开发者在终端完成从构思到上线的完整闭环。

## Claude Code特点

- 终端原生运行，轻量高效，零配置开箱即用。
- Sonnet/Opus 模型驱动，专为编程任务深度优化。
- 支持搭建项目、重构、测试、提交 PR 全流程。
- 多模态输入，支持文本、截图、图表理解。
- 深度集成 GitHub，终端/IDE/Web/iOS 多端协作。

## Claude Code教程与指南

- [GitHub 上那个画架构图的技能 Archify，收藏到 19.5K 了](https://www.b2cc.com.cn/chajian/2611) · [📄 仓库内阅读](docs/2611-GitHub上那个画架构图的技能Archify，收藏到19.5K了.md)
- [想给 Claude Code 装官方技能，注册一个市场再装两个包就够](https://www.b2cc.com.cn/jiaocheng/2613) · [📄 仓库内阅读](docs/2613-想给ClaudeCode装官方技能，注册一个市场再装两个包就够.md)
- [Claude Code v2.1.260：看改动有了全屏面板，账单变贵了它会告诉你为什么](https://www.b2cc.com.cn/jiaocheng/2609) · [📄 仓库内阅读](docs/2609-ClaudeCodev2.1.260：看改动有了全屏面板，账单变贵了它会告诉你为.md)
- [Claude Code安装教程2026最新版：npm已弃用，官方推荐这四种方式](https://www.b2cc.com.cn/jiaocheng/2554) · [📄 仓库内阅读](docs/2554-ClaudeCode安装教程2026最新版：npm已弃用，官方推荐这四种方式.md)
- [Anthropic官方技能库全解：Word、PPT、Excel、PDF文档技能免费用](https://www.b2cc.com.cn/chajian/2557) · [📄 仓库内阅读](docs/2557-Anthropic官方技能库全解：Word、PPT、Excel、PDF文档技能免.md)
- [Claude Code官方插件大盘点：13个免费插件，从代码审查到安全检查全齐了](https://www.b2cc.com.cn/chajian/2556) · [📄 仓库内阅读](docs/2556-ClaudeCode官方插件大盘点：13个免费插件，从代码审查到安全检查全齐了.md)
- [Claude自定义技能怎么做？一个SKILL.md文件就够了，官方模板直接抄](https://www.b2cc.com.cn/jiaocheng/2555) · [📄 仓库内阅读](docs/2555-Claude自定义技能怎么做？一个SKILL.md文件就够了，官方模板直接抄.md)

## Claude Code版本动态

- 2026-09-07 · [Kimi API原生支持Claude Code：不用代理直接跑第三方模型](https://www.b2cc.com.cn/claudedt/2604) · [📄 仓库内阅读](changelog/2604-KimiAPI原生支持ClaudeCode：不用代理直接跑第三方模型.md)
- 2026-09-06 · [Claude Code默认模型换成Fable 5.1：1M上下文，缓存读取降价75%](https://www.b2cc.com.cn/claudedt/2603) · [📄 仓库内阅读](changelog/2603-ClaudeCode默认模型换成Fable5.1：1M上下文，缓存读取降价75%.md)
- 2026-09-05 · [Claude Code 现在能直连 Kimi 的模型了：不转格式、不挂代理](https://www.b2cc.com.cn/claudedt/2612) · [📄 仓库内阅读](changelog/2612-ClaudeCode现在能直连Kimi的模型了：不转格式、不挂代理.md)
- 2026-09-05 · [想把技能发出去，先看 Anthropic 仓库最近这几条规矩](https://www.b2cc.com.cn/claudedt/2614) · [📄 仓库内阅读](changelog/2614-想把技能发出去，先看Anthropic仓库最近这几条规矩.md)
- 2026-09-05 · [Claude Code v2.1.257：重开就换 Fable 5.1，缓存读取价降了 75%](https://www.b2cc.com.cn/claudedt/2610) · [📄 仓库内阅读](changelog/2610-ClaudeCodev2.1.257：重开就换Fable5.1，缓存读取价降了7.md)
- 2026-08-26 · [Claude Code一周发了8个版本，都改了什么](https://www.b2cc.com.cn/claudedt/2552) · [📄 仓库内阅读](changelog/2552-ClaudeCode一周发了8个版本，都改了什么.md)
- 2026-08-26 · [Claude Code一周发了8个版本：大功能一个没有，修的全是你踩过的坑](https://www.b2cc.com.cn/claudedt/2558) · [📄 仓库内阅读](changelog/2558-ClaudeCode一周发了8个版本：大功能一个没有，修的全是你踩过的坑.md)
- 2026-08-25 · [Claude Code auto mode拆解：93%的审批都在无脑点允许，问题出在这](https://www.b2cc.com.cn/claudedt/2551) · [📄 仓库内阅读](changelog/2551-ClaudeCodeautomode拆解：93%的审批都在无脑点允许，问题出在这.md)

---

**官方持续更新入口：[Claude中文站 官网](https://www.b2cc.com.cn/)**

© [Claude中文站](https://www.b2cc.com.cn/) · 本仓库为官网内容镜像，文章版权归原作者所有。