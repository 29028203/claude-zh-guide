# Claude Code安装教程2026最新版：npm已弃用，官方推荐这四种方式

> 原文链接：[https://www.b2cc.com.cn/jiaocheng/2554](https://www.b2cc.com.cn/jiaocheng/2554)

<p><code>npm install -g @anthropic-ai/claude-code</code>，如果你最近照着某篇安装教程敲了这条命令，最好停一下：官方在 2026 年 1 月更新了安装文档，npm 方式被明确标为弃用。朋友前两天转来一篇教程让我掌掌眼，开头赫然就是这行命令。这类文章搜索引擎里一抓一大把，当下装得上，后续版本却难保证兼容。官方现在主推四种渠道，这篇按最新 README 把安装一次讲透。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/claude/2026/08/20260825010544_085528.png" alt="Claude Code 安装方式"></p>
<h2>四种官方渠道，对号入座</h2>
<p>MacOS 和 Linux 用户，首选安装脚本：</p>
<p><code>curl -fsSL https://claude.ai/install.sh | bash</code></p>
<p>同平台还有 Homebrew 可选：<code>brew install --cask claude-code</code>。</p>
<p>到了 Windows，官方推荐 PowerShell：</p>
<p><code>irm https://claude.ai/install.ps1 | iex</code></p>
<p>要是机器上装了 WinGet，<code>winget install Anthropic.ClaudeCode</code> 走微软的包管理器，往后更新省心得多。npm 那条路眼下暂时还能走通，但 Deprecated 的标记已经挂出，新装用户不必再打这儿进。</p>
<h2>装完第一件事：cd 进项目目录</h2>
<p>装好后把目录切到项目里，敲 <code>claude</code> 回车，交互界面随即开启。官方给它的定位是&#8221;住在你终端里的编程智能体&#8221;：代码库整体结构它来理解，例行任务它来执行，复杂代码它来解释，git 工作流它来处理，指挥方式全靠自然语言。</p>
<p>终端之外，这同一套能力还留着两个入口：IDE 扩展算一个（VS Code 等编辑器可用）。GitHub 上的 @claude 算另一个，PR 或 issue 里 @它一声，代码审查、修 bug 远程就能办。</p>
<h2>新手常问的几件事，答案先备好</h2>
<p>报 bug 用不着翻论坛，CLI 里直接输 <code>/bug</code>，问题描述连同上下文一并带走，比手写 issue 高效得多。使用问题去官方 Claude Developers Discord，维护者和重度用户都在那儿出没。</p>
<p>隐私方面官方口径明确：收集的数据涵盖代码接受率，会话对话，用户反馈。用户反馈不会拿去训练模型，这一点有承诺。会话数据的访问权限设有严格限制。</p>
<p>安装卡住，两件事先查：系统版本达不达标、有没有挂代理，安装脚本要从 claude.ai 拉文件，网络不通一切白搭。跑通之后，进阶玩法（自定义命令，技能，插件）站内<a href="https://www.b2cc.com.cn/jiaocheng" target="_blank" rel="noopener">教程</a>区会陆续更新，先把<a href="https://www.b2cc.com.cn/" target="_blank" rel="noopener">Claude</a> 本身用顺手再说。</p>

---

原文链接：[https://www.b2cc.com.cn/jiaocheng/2554](https://www.b2cc.com.cn/jiaocheng/2554)
