# Claude Code官方插件大盘点：13个免费插件，从代码审查到安全检查全齐了

> 原文链接：[https://www.b2cc.com.cn/chajian/2556](https://www.b2cc.com.cn/chajian/2556)

<p>anthropics/claude-code 这个仓库里，藏着一个多数人没翻过的角落：CLI 本体之外码着一个官方插件目录，13 个由官方亲手维护的插件，一分钱不收。这是我帮朋友搭 Claude Code 环境时顺手翻出来的，他看完直呼白瞎，裸用了俩月才晓得。这批插件还附带一层隐藏价值：它们本身就是插件系统的教科书示范，斜杠命令，专职 agent，钩子，MCP 服务器之间怎么咬合运转，源码翻一遍就全明白。下面按值得装的程度，挨个过一遍。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/claude/2026/08/20260825010625_715022.png" alt="官方插件矩阵"></p>
<h2>先把最好玩的两个摆出来</h2>
<p>ralph-wiggum，名字出自《辛普森一家》，本体是台自循环执行器：敲下 /ralph-loop，Claude 便对着同一任务无限迭代，直到彻底做完。中途想溜。Stop 钩子把它拦下来，逼着继续。挂机跑长任务的邪道玩法，官方亲自示范。security-guidance 则像个不知疲倦的安全哨兵：PreToolUse 钩子实时盯九类危险模式，命令注入，XSS，eval 滥用，危险 HTML，pickle 反序列化，os.system 调用全在名单上，编辑文件一旦碰到立即告警。想让 AI 写代码又怕它写出漏洞的，闭眼装。</p>
<h2>第一梯队：代码审查加 Git 日常</h2>
<p>code-review 值得单开一段。一次审查，五个 Sonnet agent 并行开工：一个查 CLAUDE.md 合规，一个挖潜在 bug，一个补历史上下文，一个翻 PR 历史，一个读代码注释。各自产出先按置信度筛掉误报，再汇成一份干净报告。小团队腾不出人看 PR 的，拿它兜底。</p>
<p>commit-commands 包揽 Git 三件套的体力活：/commit 完成提交，/commit-push-pr 一步推送加建 PR，/clean_gone 清扫失效分支。pr-review-toolkit 走的是反向思路，不打综合分，只做专项：评论质量，测试覆盖，静默失败，类型设计，代码简化，六个专项 agent 各守一摊，哪块薄弱就跑哪块。</p>
<h2>剩下八个，一人一句带过</h2>
<p>frontend-design 专治&#8221;一眼 AI 审美&#8221;，检测到前端任务会自动启用。feature-dev 是条七阶段的结构化开发流，探索，架构，审查三个 agent 随行伺候。hookify 最省心，对话里说句&#8221;别再干 XX 了&#8221;，钩子自动生成。plugin-dev 提供八阶段向导，手把手教造插件。agent-sdk-dev 给 Agent SDK 项目搭脚手架。explanatory-output-style 会在会话开头注入实现原理讲解。learning-output-style 走教学模式，到关键决策点要你亲手写 5 到 10 行代码。claude-opus-4-5-migration 负责搬家，把代码从 Sonnet 4.x / Opus 4.1 平滑迁到 Opus 4.5。</p>
<p>安装有两条路可选：在 Claude Code 里用 /plugin 命令装，或者写进项目的 .claude/settings.json。另外，每个插件的标准目录结构，.claude-plugin/plugin.json 加 commands/，agents/，skills/，hooks/ 四件套，本身就是现成的插件开发参考模板。想看系统性拆解，站内<a href="https://www.b2cc.com.cn/chajian" target="_blank" rel="noopener">插件</a>栏目持续更新中。</p>

---

原文链接：[https://www.b2cc.com.cn/chajian/2556](https://www.b2cc.com.cn/chajian/2556)
