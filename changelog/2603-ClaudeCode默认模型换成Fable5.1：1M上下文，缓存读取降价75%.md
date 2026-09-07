# Claude Code默认模型换成Fable 5.1：1M上下文，缓存读取降价75%

> 原文链接：[https://www.b2cc.com.cn/claudedt/2603](https://www.b2cc.com.cn/claudedt/2603)

<p>Claude Code最近一次版本<a href="https://www.b2cc.com.cn/claudedt" target="_blank" rel="noopener">更新</a>（v2.1.257）里藏了个重要变化：默认的Fable模型换成了<a href="https://www.b2cc.com.cn/" target="_blank" rel="noopener">Claude</a> Fable 5.1。别小看这个&#8221;默认&#8221;，它直接影响每个Claude Code用户的日常花费和效果。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/claude/2026/09/20260904190952_534587.png" alt="Claude Code v2.1.257默认模型升级" style="max-width:100%;height:auto;border-radius:8px;margin:16px 0" /></p>
<h2>默认模型升级意味着什么</h2>
<p>v2.1.257把claude-fable-5-1设成了默认Fable模型，上下文支持100万token，定价每百万输入token 10美元、输出50美元，缓存读取只要0.25美元。对Claude Code这种重度依赖长上下文的工具来说，缓存读取的价格几乎决定了整体花费——Fable 5.1把缓存读取比Fable 5降了75%，典型任务总成本能省25%左右。</p>
<p>能力上，Fable 5.1在Claude Code里默认以High档努力运行，官方称它能修问题的根因而不是只修表面，早期用户的反馈普遍是&#8221;更快、更省token、更少废话&#8221;。</p>
<h2>这版还改了什么</h2>
<p>除了换默认模型，v2.1.257还加了几项实用设置：timeFormat和timeZone，让日志和显示时间跟随你的习惯；auto mode新增了containment-escape规则，防止自动模式里子任务跳出沙盒边界——对跑自动审批流程的用户，这是安全性的补强；另外新增了CLAUDE_CODE_SUBAGENT_MODEL_FORCE环境变量，可以强制指定子Agent用的模型。</p>
<p>每次大版本默认模型切换，都是一次&#8221;系统性的体验迁移&#8221;：你不需要手动改任何配置，重开Claude Code就会用上新模型，但成本结构会跟着变化。如果你平时跑的任务缓存命中率高，这轮升级大概率是省钱的；建议更新后跑几个典型任务，用/cost看一眼实际花费对比。</p>
<p>Claude Code几乎每周都在更新。想看更完整的版本历史，可以翻翻官方更新日志，或者留意本站的版本解读。</p>

---

原文链接：[https://www.b2cc.com.cn/claudedt/2603](https://www.b2cc.com.cn/claudedt/2603)
