# Claude自定义技能怎么做？一个SKILL.md文件就够了，官方模板直接抄

> 原文链接：[https://www.b2cc.com.cn/jiaocheng/2555](https://www.b2cc.com.cn/jiaocheng/2555)

<p>每周给 Claude 交代一遍周报格式，这活儿同事干了三周，到第三周已经面露菜色。我给他指了条十分钟一劳永逸的路：写个自定义技能。剥掉营销包装，Claude 的技能（Skills）系统朴素得吓人，一个文件夹，里面一份 SKILL.md，需要的话再添几个脚本和资源文件，仅此而已。加载之后，Claude 就学会了按你的规矩办某类任务：照公司品牌规范产文档、按团队流程跑数据分析，一次编写，永久复用。这篇从零手把手拆，素材全部来自 Anthropic 官方 skills 仓库的说明文档，照抄结构就行。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/claude/2026/08/20260825010605_181426.png" alt="自定义技能文件结构"></p>
<h2>SKILL.md 的最小可用骨架</h2>
<p>想跑起来，frontmatter 只需两个字段，外加正文指令：</p>
<p><code>---<br />name: my-skill-name<br />description: 说清这个技能干什么、什么时候该用它<br />---</p>
<p># 技能名称<br />[这里写 Claude 要遵循的指令]<br />## 示例<br />- 用法示例1<br />## 约束<br />- 规则1</code></p>
<p>几个坑提前避开。name 有硬性要求：全小写、连字符分词，&#8221;claude&#8221;&#8221;anthropic&#8221;等保留词一个不能沾，官方仓库前阵子刚为此给自家 academy-guide 技能改了名，教训摆在眼前。description 的讲究在于二合一：既说做什么，也说何时用，Claude 靠这段文字判断要不要自动启用技能，写得含糊，技能就成了永不触发的摆设。正文负责承载完整指令：步骤，示例，边界情况怎么处理，颗粒度越细，触发后的表现越稳。</p>
<h2>起步姿势：拿模板当骨架</h2>
<p>空白文档不必硬憋。官方仓库的 template 目录里躺着现成的技能模板，fork 过来改，比从零起步快得多。自己写完想对标成熟案例。几十个官方示例在仓库里敞开供应，从创意设计到企业工作流一应俱全，它们本身就是&#8221;指令该怎么组织&#8221;的活教材。</p>
<h2>安装路径：三端各走各的门</h2>
<p>Claude Code 用户最省事，一条命令挂官方市场：<code>/plugin marketplace add anthropics/skills</code>，然后用 /plugin 装技能包。自研技能更简单，往项目的 .claude 目录里一扔就自动被识别。Claude.ai 网页版的付费用户可以直接上传自定义技能。API 调用方另有 Skills 接口可走。</p>
<p>顺带一个值得知道的信息：Agent Skills 已有独立开放标准（agentskills.io），Claude 的实现只是其中之一。也就是说，你写的技能文件结构有机会在其他 agent 工具里直接通用，这份资产的保值性比想象中好。</p>
<p>最后一条实操建议：第一个技能切忌贪大。挑一件每周都要重复交代的琐事，典型如&#8221;按我们的格式写周报&#8221;，五十行以内写完，投用一周，再按 Claude 的实际表现迭代三个版本。这个循环走完，整套玩法就吃透了。想直接用现成技能的，站内<a href="https://www.b2cc.com.cn/chajian" target="_blank" rel="noopener">插件</a>栏目有持续整理。</p>

---

原文链接：[https://www.b2cc.com.cn/jiaocheng/2555](https://www.b2cc.com.cn/jiaocheng/2555)
