# 想把技能发出去，先看 Anthropic 仓库最近这几条规矩

> 原文链接：[https://www.b2cc.com.cn/claudedt/2614](https://www.b2cc.com.cn/claudedt/2614)

<p>想把技能传上 Anthropic 官方仓库的人，最近别急着打包，仓库这两天刚动过一轮，前端技能更新了，还有几个技能改了名。改名的动静里，能看出上传的门道。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/claude/2026/09/20260904191121_058649.png" alt="Anthropic 技能仓库上传规范"></p>
<p>最明显的是 claude-academy-guide 改名 academy-guide。提交说明里写得直白，技能名不能带 claude、anthropic 这类保留词。起名把品牌词塞进去，打包上传会在头一关就被校验拦下来。</p>
<p>同一个提交里，官方把它的描述从一千多字符压到 992。SKILL.md 的 description 字段限了 1024 字符，超了就传不上去。这字段是给 AI 判断什么时候调用技能的，写太长把匹配稀释了，一两句话讲清用途和触发场景最好。</p>
<p>仓库 README 现在指向 agentskills.io，技能格式是开放标准，不是哪一家关起门定的。一个技能就是一个文件夹加一份 SKILL.md，顶部用 YAML 写 name 和 description，正文写怎么操作。新建技能直接抄 template 目录里的模板，不用自己发明格式。</p>
<p>想照官方学写法的，把 skills 目录翻一遍就够，几十个示例分好类放着，随便打开一个看 SKILL.md 怎么写。目录里最实用的是 docx、pdf、pptx、xlsx 四个文档技能，PDF 提字段这类活就靠它们。源码公开能参考，商用前把授权条款翻一遍。</p>
<p>真被拦过一次就知道，卡住的多数是名字带保留词，或者描述超了长度。校验提示会直接指出是哪一处，改一行再传就是。</p>

---

原文链接：[https://www.b2cc.com.cn/claudedt/2614](https://www.b2cc.com.cn/claudedt/2614)
