# Roam Research 的思维算法（AOT）

Algorithms of Thought（AOT）是一个 Roam Research 扩展，用来提供一套**结构化思考脚手架**。它通过轻量、可重复使用的提示，帮助你更清晰地思考决策、问题、权衡以及下一步行动。

AOT **不是自动化工具**，也**不是 AI**。它是一组有意设计的认知工具：小而明确的思考模式，你可以在恰当的时候主动调用。它的价值来自你按结构去思考，而不是把思考过程交给别人替你完成。

你可以通过以下方式触发 AOT：

- **命令面板**
- **Roam 快捷键**
- **SmartBlocks 流程**

---

## 最近更新（架构与安全性）

这个扩展最近经过了**较大幅度的重写**，目标是提升稳定性、可预测性和安全性，尤其是在频繁使用 SmartBlocks 和命令面板时。

### 具体改了什么

- **统一的执行引擎**  
  所有 AOT 现在都走一条统一、稳定的执行路径。

- **更安全的取消与清理机制**  
  取消 AOT 时，不会再留下半成品结构，也不容易覆盖已有内容。

- **感知焦点的行为设计**  
  执行引擎会尊重当前 block 的焦点状态，避免破坏性编辑。

- **每次运行彼此隔离**  
  每次调用都是独立的，状态不会在不同 AOT 之间泄漏。

- **可扩展注册表**  
  可以更安全地增加新的 AOT，而不至于破坏已有功能。

目标很简单：**AOT 应该可靠到让你感觉“它没什么存在感”。**

---

## 什么是思维算法（Algorithms of Thought）？

一个思维算法，本质上就是一种**有名字的思考模式**，它通常具备：

- 明确的用途
- 固定的结构
- 尽量少的仪式感

它们的设计目标是：

- 降低认知负担
- 把推理过程外显出来
- 避开常见思维陷阱
- 鼓励更审慎、更结构化的反思

你可以把它们理解成一种**思维层面的宏命令**。

---

## AOT 列表：按主题分类

下面是当前可用的全部 AOT，按照它们支持的思考类型分组。每个条目都附带了简短说明和对应的 SmartBlocks 命令。

### 方向、目标与优先级

- **Aims, Goals, Objectives**
  - 用来区分高层意图与具体目标。
  - `<%AOTAGO%>`
- **First Important Priorities**
  - 当一切看起来都很重要时，强迫你做优先级排序。
  - `<%AOTFIP%>`
- **Next Action**
  - 把模糊意图转成一个具体、可执行的动作。
  - `<%AOTNEXTACTION%>`

### 决策与权衡

- **Basic Decision**
  - 一个简单、最小化的决策脚手架。
  - `<%AOTBASICDECISION%>`
- **Simple Choice**
  - 适合复杂度较低时做轻量对比。
  - `<%AOTCHOICE%>`
- **Alternatives, Possibilities, Choices**
  - 先扩展选项空间，再逐步收敛。
  - `<%AOTAPC%>`
- **Regret Minimisation**
  - 从长期后悔的角度评估选择。
  - `<%AOTREGRET%>`
- **Design / Decision, Outcome, Channels, Action (DODCA)**
  - 强制把决策与执行对齐。
  - `<%AOTDODCA%>`

### 批判性思考与挑战

- **Assumptions X-Ray**
  - 把隐藏的假设显性化。
  - `<%AOTAX%>`
- **Examine Both Sides**
  - 用来对抗单边思考。
  - `<%AOTEBS%>`
- **Difference Engine**
  - 帮你识别选项或立场之间真正的差异。
  - `<%AOTDIFFERENCE%>`

### 分析、诊断与理解

- **Five Whys**
  - 通过连续追问做根因分析。
  - `<%AOTFIVEWHYS%>`
- **Recognise, Analyse, Divide**
  - 把复杂问题拆成可处理的部分。
  - `<%AOTRAD%>`
- **Consequence and Sequel**
  - 同时看短期与长期影响。
  - `<%AOTCS%>`
- **Consider All Factors**
  - 把注意力从显而易见的因素扩展出去。
  - `<%AOTCAF%>`

### 分歧与视角

- **Agreement, Disagreement and Irrelevance**
  - 在争论中分离真正有信号的内容和噪音。
  - `<%AOTADI%>`
- **Right to Disagree (Cortex Futura)**
  - 一种有结构、不升级冲突的分歧处理方式。
  - `<%AOTRTD%>`
- **Right to Disagree (Deeper Version)**
  - 更深入、更完整的对抗式思考脚手架。
  - `<%AOTRTDDEEP%>`

### 创造力与重构视角

- **Six Thinking Hats**
  - 通过明确的思考模式并行处理问题。
  - `<%AOTSIXHATS%>`
- **Plus, Minus, Interesting**
  - 不做过度分析，也能快速换个角度看问题。
  - `<%AOTPMI%>`
- **SWOT Analysis**
  - 经典的情境评估框架。
  - `<%AOTSWOT%>`

### 行动与解决

- **Want, Impediment, Remedy**
  - 用来识别阻碍和可执行的补救措施。
  - `<%AOTWANT%>`
- **TOSCA**
  - 从触发条件、结果和行动三个角度给问题定框架。
  - `<%AOTTOSCA%>`
- **Pain Button (Ray Dalio)**
  - 把情绪触发点视为学习机会。
  - `<%AOTPAIN%>`

### 来源分析与评估

- **REALLY?**
  - 一个快速、结构化的检查清单，用来评估主张、研究、统计数字或说服性论证。它的设计目标是尽早触发认识论上的不舒服感，避免你太早接受薄弱或误导性的结论。
  - `<%AOTREALLY%>`
- **REAPPRAISED Checklist**
  - 一个结构化清单，用来批判性评估来源、论点或证据整体（例如文章、主张、提案）。特别适合学术阅读、政策文件和说服性写作。
  - `<%AOTREAPPRAISED%>`

---

## 我该用哪一个 AOT？

如果你不确定从哪里开始，可以看这个指引。先判断你需要的是什么类型的思考，而不是先回忆工具名字。

### “我其实还没搞清楚问题到底是什么”

先用这些帮助你理解或诊断，再考虑行动：

- **Recognise, Analyse, Divide**：先把复杂性拆开
- **Five Whys**：找到根因
- **Consider All Factors**：把视野拉宽
- **Difference Engine**：澄清真正不同的地方
- **Consequence and Sequel**：探索后续影响

### “我需要做一个决定”

当你在不同选项之间做选择时，可以用这些：

- **Simple Choice**：低风险、选项不多
- **Basic Decision**：日常决策
- **Alternatives, Possibilities, Choices**：先拓展选项空间
- **Regret Minimisation**：长期、会塑造身份的决策
- **DODCA**：必须导向执行的决策

### “所有事情都很重要，我需要聚焦”

这些适合拿来定向和排优先级：

- **Aims, Goals, Objectives**：澄清意图和执行的关系
- **First Important Priorities**：强制排序
- **Next Action**：从思考走向行动

### “我担心自己的思考有偏见，或者太浅”

这些适合拿来给推理做压力测试：

- **Assumptions X-Ray**：把隐藏假设拉出来
- **Examine Both Sides**：对抗确认偏误
- **Agreement, Disagreement and Irrelevance**：把真正有意义的内容和噪音分开

### “这里有分歧，或者存在竞争性观点”

这些适合做建设性的对抗式思考：

- **Right to Disagree (Cortex Futura)**：有原则地保留分歧
- **Right to Disagree (Deeper Version)**：更严格的对抗性分析
- **Agreement, Disagreement and Irrelevance**：映射共识与分歧

### “我想更有创造力，或者换个框架思考”

这些适合用来改换视角：

- **Six Thinking Hats**：平行思考
- **Plus, Minus, Interesting**：快速重构视角
- **SWOT Analysis**：快速看整体情境

### “我已经有洞见了，但还没进入行动”

当问题已经理解得差不多，但推进卡住时，可以用这些：

- **Want, Impediment, Remedy**：识别阻碍和对应修复
- **TOSCA**：澄清触发、结果与行动
- **Pain Button (Ray Dalio)**：从情绪摩擦里学习
- **Consequence and Sequel**：检查行动在时间上的后果

### “我正在读资料，或者评估一个主张”

当任务重点是*评估*而不是*决策*时，用这些：

- **REALLY?**：快速评估主张
- **REAPPRAISED Checklist**：系统性评估来源与证据

### “如果你卡在执行上 → Ultraworking”

可以安装 Ultraworking 扩展来增强执行（Roam Depot）。

### “如果你卡在创意上 → Oblique Strategies”

可以通过 Roam Depot 安装 Oblique Strategies 扩展来打破创作卡顿。

一个实用的经验法则：

- 如果你是**困惑**的：先诊断
- 如果你在**选择**：先决策
- 如果你**卡住**了：先排优先级或转成行动
- 如果你在**争论**：用对抗式思考
- 如果你在**阅读**：做评估

AOT 最有效的用法，是你先**给当前的思考问题命名**。

---

## 即将加入

- After Action Review
- Circle of Control
- Claim, Evidence, Confidence
- Claim–Evidence–Warrant
- Constraint–Bottleneck–Relief
- Constraints First
- Evidence Hierarchy Check
- Issue Log
- Other People’s Views
- PDSA
- Pre-Mortem
- Stakeholder Mapping
