# Claude Code v2.1.257：重开就换 Fable 5.1，缓存读取价降了 75%

> 原文链接：[https://www.b2cc.com.cn/claudedt/2610](https://www.b2cc.com.cn/claudedt/2610)

<p><a href="https://www.b2cc.com.cn/claudedt" target="_blank" rel="noopener">Claude Code</a> 的 v2.1.257 更新，对天天开它干活的人来说，第一个变化是打开就能感觉到的：默认的 Fable 模型换成了 Claude Fable 5.1。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/claude/2026/09/20260904190952_534587.png" alt="Claude Code v2.1.257默认模型升级"></p>
<p>不用手动改任何配置，重开会话就在用新模型了。上下文支持 100 万 token，输入一百万个 token 收 10 美元，输出收 50 美元，缓存读取一百万个只收 0.25 美元。干这行的人都清楚，缓存读取价几乎决定整体账单，5.1 比 Fable 5 降了 75%，典型任务总成本能省下 25% 上下。</p>
<p>能力上也有变化。5.1 默认按 High 档努力跑，官方给它的定位是修根因，不只在表面打补丁。用下来的反馈比较集中，普遍说更快、更省 token、废话更少。</p>
<p>这版还加了几项设置。timeFormat 和 timeZone 管日志和显示时间，跟着个人习惯走。auto mode 里新增了 containment-escape 规则，防子任务跑出沙盒边界，跑自动审批流程的人会安心一点。新的环境变量 CLAUDE_CODE_SUBAGENT_MODEL_FORCE 能强制指定子 Agent 用的模型。</p>
<p>默认模型切换这种更新，不需要你改什么，代价是成本结构跟着变。平时任务缓存命中率高的话，这轮大概率是省钱的。更新完拿几个典型任务跑一跑，敲 /cost 对比下实际花费，心里就有底了。</p>

---

原文链接：[https://www.b2cc.com.cn/claudedt/2610](https://www.b2cc.com.cn/claudedt/2610)
