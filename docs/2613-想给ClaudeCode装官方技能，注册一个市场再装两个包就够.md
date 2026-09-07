# 想给 Claude Code 装官方技能，注册一个市场再装两个包就够

> 原文链接：[https://www.b2cc.com.cn/jiaocheng/2613](https://www.b2cc.com.cn/jiaocheng/2613)

<p>下午要处理一份合同 PDF，想把里面的表单字段提出来。可 <a href="https://www.b2cc.com.cn/jiaocheng" target="_blank" rel="noopener">Claude Code</a> 默认不会这手活，大多数人这时候才想起来装技能。第一个找的就是 Anthropic 的官方仓库 anthropics/skills，文档处理、编程辅助这些能力都打包成了插件。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/claude/2026/09/20260904191026_172609.png" alt="Claude Code 官方技能安装"></p>
<p>装之前得先把仓库注册成插件市场。在对话里敲这一行命令。</p>
<p>/plugin marketplace add anthropics/skills</p>
<p>回车之后，Claude Code 会自己去官方仓库拉取。几秒钟后它告诉你市场注册好了，顺带指了能翻技能列表的地方。</p>
<p>接下来挑包。仓库里现成的有两个。document-skills 管文档，Word、PPT、Excel、PDF 的创建和编辑都归它管。想让它干活，装这一个包。</p>
<p>/plugin install document-skills@anthropic-agent-skills</p>
<p>example-skills 是另一个，里面是创意、设计、开发这些方向的演示技能。想看看别人怎么把技能写成能用的样子，装这个包。</p>
<p>/plugin install example-skills@anthropic-agent-skills</p>
<p>不想敲命令也能走菜单。注册完市场，进 Browse and install plugins，选中 anthropic-agent-skills。勾上你要的包，点 Install now 就完事。</p>
<p>装完回到刚才那份合同 PDF，把它拖进对话，说一句把表单字段提出来。它会自己去翻刚装好的技能，调对应的工具干活。你只管看结果，不用记它内部有多少个子命令。</p>
<p>两个包的分寸不一样，用之前留意一下。example-skills 偏演示和教育，官方自己说过线上行为和示例可能有差异。重要场景先亲手测一遍，再拿它干活。document-skills 的源码能看，但不是完全开源。自己参考学习没问题，商用之前把授权条款核对清楚。想学技能本身怎么写，翻仓库的 skills 目录。几十个示例按 SKILL.md 的结构排着，从艺术音乐到测试再到 MCP 生成都有。照着拆一遍，一套写法基本就摸熟了。</p>
<p>装完拿一份真实文档试一遍，比看多少说明都直观。</p>

---

原文链接：[https://www.b2cc.com.cn/jiaocheng/2613](https://www.b2cc.com.cn/jiaocheng/2613)
