# Anthropic官方技能库全解：Word、PPT、Excel、PDF文档技能免费用

> 原文链接：[https://www.b2cc.com.cn/chajian/2557](https://www.b2cc.com.cn/chajian/2557)

<p>docx，pdf，pptx，xlsx，支撑 Claude 文档能力的四个技能，源码在 Anthropic 的官方 skills 仓库里全部公开，四个文件夹随便读。这个答案是上周让 Claude 改一份 Word 格式、改得又快又准之后，我出于好奇去翻仓库才找到的。授权严格说属于 source-available，不是完全开源，但作为一套在生产环境真实跑着的实现，参考价值足以甩市面上多数教程几条街。你在 Claude.ai 里说&#8221;帮我做份 PPT&#8221;&#8221;把这份 Word 改一下&#8221;，真正动手的就是这四位。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/claude/2026/08/20260825010645_117410.png" alt="文档技能四件套"></p>
<h2>仓库的布局：三块各管一摊</h2>
<p>布局清清爽爽。skills 目录是重头戏，按用途划四类：创意与设计方向，收绘画、音乐等技能。开发与技术方向，有 Web 应用测试、MCP 服务器生成等。企业与沟通方向，放品牌规范、沟通模板。文档四件套压轴。spec 目录存放 Agent Skills 规范，template 目录则放技能模板，想自己动手写技能的，从 template 起步最顺。</p>
<h2>同一套四件套，普通人看功能，开发者看门道</h2>
<p>这四个技能是 Claude 文档能力的发动机：新建文档，调整格式，抽取内容，处理表单字段，你点&#8221;创建文件&#8221;时忙活的就是它们。对普通用户，意义很直接，付费版 Claude.ai 里这些能力全部就位，开箱即用。开发者盯的是另一层：官方如何把&#8221;操作 Office 文档&#8221;这种复杂任务一步步拆成技能指令，这套拆解思路，是做企业自动化技能时最值得照抄的样板。</p>
<h2>两步接入 Claude Code</h2>
<p>第一步注册官方市场：<code>/plugin marketplace add anthropics/skills</code>。第二步用一条命令装包：</p>
<p><code>/plugin install document-skills@anthropic-agent-skills</code>（文档四件套）</p>
<p><code>/plugin install example-skills@anthropic-agent-skills</code>（示例技能集）</p>
<p>装完即用，自然语言触发，比方说&#8221;用 PDF 技能把这份文件的表单字段提出来&#8221;。桌面端用户无需碰命令行，设置界面的插件市场里搜一下就能装。API 用户走另一扇门：Skills 接口既支持上传自定义技能，也支持调用官方预置技能，做产品集成的选这条。</p>
<p>一个务实的提醒别省：官方在仓库里白纸黑字写明，这批技能定位演示和教学，实际行为可能与 Claude 产品内的表现有差异，进关键业务流程前，先在自己的环境里完整测一轮。生态里还有 Notion 等合作伙伴的官方技能在路上，站内<a href="https://www.b2cc.com.cn/chajian" target="_blank" rel="noopener">插件</a>栏目后续持续跟进。</p>

---

原文链接：[https://www.b2cc.com.cn/chajian/2557](https://www.b2cc.com.cn/chajian/2557)
