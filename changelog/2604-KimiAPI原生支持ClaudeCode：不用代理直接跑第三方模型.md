# Kimi API原生支持Claude Code：不用代理直接跑第三方模型

> 原文链接：[https://www.b2cc.com.cn/claudedt/2604](https://www.b2cc.com.cn/claudedt/2604)

<p>Claude Code生态最近多了个新玩法：Kimi API宣布原生支持Codex和Claude Code。简单说，用Claude Code的用户不用转换格式、不用本地代理，就能通过自定义model provider直连Kimi的模型（包括kimi-k3、kimi-k2.7系列）。对国内开发者来说，这是个挺实在的变化。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/claude/2026/09/20260904191010_044329.png" alt="Kimi 接入 Claude Code" style="max-width:100%;height:auto;border-radius:8px;margin:16px 0" /></p>
<h2>意味着什么</h2>
<p>Claude Code默认绑定Anthropic的模型，而想用Claude Code的&#8221;壳&#8221;（终端工作流、技能、自动审批这些能力）来跑其他模型，以前需要各种曲线操作。Kimi这次的原生支持，等于官方在model provider层把路铺好了：在Claude Code里配好自定义模型，就能直接调用Kimi，不需要本地起代理、不需要格式转换。</p>
<p>这种&#8221;工具壳+第三方模型&#8221;的组合对国内用户尤其有意义：一是网络与支付门槛低，Kimi国内直接可用；二是多模型可以随时切换——日常简单任务用便宜的模型，重活切回主力模型，省下来的都是真金白银。</p>
<h2>怎么配</h2>
<p>思路不复杂：在Claude Code的模型配置里添加自定义provider，填入Kimi的API地址和密钥，指定模型名（如kimi-k3等），保存后重启会话即可。具体字段以Kimi官方文档和Claude Code配置说明为准——不同版本的Claude Code，自定义模型配置入口可能略有差异。</p>
<p>几点提醒：第一，跨模型跑Claude Code，官方技能和部分高级能力可能不完全兼容，复杂任务建议先小范围验证；第二，模型切换涉及上下文和成本结构差异，建议用/cost这类工具盯一下实际消耗；第三，如果你主要看重Claude Code的自动审批、长任务稳定性，主力场景还是建议留在官方模型上。</p>
<p>Claude Code正在从&#8221;一个产品&#8221;变成&#8221;一个生态&#8221;——壳是Claude Code，芯可以自选。这对开发者的好处是明显的：工具的体验和模型的选择，终于可以分开挑了。</p>

---

原文链接：[https://www.b2cc.com.cn/claudedt/2604](https://www.b2cc.com.cn/claudedt/2604)
