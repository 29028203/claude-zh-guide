# Claude Code v2.1.260：看改动有了全屏面板，账单变贵了它会告诉你为什么

> 原文链接：[https://www.b2cc.com.cn/jiaocheng/2609](https://www.b2cc.com.cn/jiaocheng/2609)

<p><a href="https://www.b2cc.com.cn/claudedt" target="_blank" rel="noopener">Claude Code</a> 9 月 3 日更新到 v2.1.260。这版没发新模型，改的东西都是天天在用的人会撞上的。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/claude/2026/09/20260904191048_372160.png" alt="Claude Code /diff与/cost用法"></p>
<p>代码改动怎么看，这版体验先变了。以前 diff 要么切到别的窗口，要么挤在终端里一行行翻，代码改多了一眼看不过来。现在对话旁边多了个全屏 diff 面板，敲 /diff 就能切换。一次改了好几个文件的活，全屏里挨个核对不容易漏。做代码评审要把改动整个过一遍时，也比在窄窗口里扫得清楚，容易发现不该动的地方。看完再敲一次 /diff，或者按快捷键，就退回普通对话。面板里键盘照常能用，光标移哪看哪。</p>
<p>花钱这块也有人管了。/cost 输出和状态行现在会显示缓存没命中的原因。用久了会发现，费用忽高忽低，多半是缓存悄悄没命中。命中了只按 0.25 美元每百万 token 收，没命中就得按全价输入算，差好几倍。工具把原因直接点出来，像消息被截断，会话改动太大，或工具上下文切换，都是常见情形。照着调整，比如把大任务拆成小会话，别每轮都往里塞一大段不变的内容，命中率能明显提上来，不用再对着账单猜。</p>
<p>这版还顺带修了一批零碎问题，权限规则、Bash 沙箱和模型切换，后台会话、VSCode 集成这些都有涉及。节奏没变，Claude Code 基本保持每周一更。</p>
<p>想省时间的，先试 /diff 全屏面板。跑长任务、在意花费的，敲一遍 /cost 看看缓存提示。两个功能都在这一版里，更新完就能用。</p>

---

原文链接：[https://www.b2cc.com.cn/jiaocheng/2609](https://www.b2cc.com.cn/jiaocheng/2609)
