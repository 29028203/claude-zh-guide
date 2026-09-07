# Claude Code 现在能直连 Kimi 的模型了：不转格式、不挂代理

> 原文链接：[https://www.b2cc.com.cn/claudedt/2612](https://www.b2cc.com.cn/claudedt/2612)

<p>把 <a href="https://www.b2cc.com.cn/claudedt" target="_blank" rel="noopener">Claude Code</a> 的模型切成 Kimi 的 k3 用了一阵子，今天把配置过程记下来，想省接口费的人可以照着走。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/claude/2026/09/20260904191010_044329.png" alt="Claude Code 直连 Kimi 模型"></p>
<p>先说怎么切。Claude Code 设置里加一个自定义 provider，接口地址和密钥填 Kimi 文档里给的那两串，模型名写 kimi-k3 这类，保存完重启会话就生效。密钥是 Kimi 官网注册后用手机号领的，不用绑卡。</p>
<p>以前这事干不成。Claude Code 只认 Anthropic 自家的模型，想跑别的得自己架一层代理，或者写脚本把请求转格式。我试过一次，代理半夜崩了，第二天早上起来连不上，排查半天才想起来是代理的事，从那以后就懒得折腾了。这周 Kimi 的 API 宣布原生支持 Codex 和 Claude Code，等于官方把路铺好了，不用再自己搭桥。</p>
<p>我这几天的用法是，写脚本、改文案这类小活挂 k3，便宜。真要重构代码、跑长任务，再切回主力模型。切换就在会话里改模型名，几秒钟的事。这几天账单少了大概三分之一，这个数我盯着 /cost 看的，不是凭感觉。</p>
<p>有个坑说一句。挂着官方技能的任务切到 Kimi 上偶尔报不兼容，自动审批相关的尤其明显。我后来把依赖技能的活都留在默认模型，只把纯对话的活切过去，这套分法用下来挺顺。</p>
<p>跑通一套配置不难，难的是搞清楚哪些活能切。我这两天先把整理周报这类小活切过去跑，跑顺了才往大的放，账单缩水是看得见的。</p>

---

原文链接：[https://www.b2cc.com.cn/claudedt/2612](https://www.b2cc.com.cn/claudedt/2612)
