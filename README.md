# Humanizer-en-zh-mixed-for-GPT6.1sol：中英双语润色与专治 GPT“防御性笑话”特供版 Skill

将英文版 [blader/humanizer v3.1.0](https://github.com/blader/humanizer)、中文版 [op7418/Humanizer-zh (2026-09-23)](https://github.com/op7418/Humanizer-zh) 与 **《GPT 防御性笑话大全》专项去杠精规则**深度整合为一体的双语 Agent Skill。

它不仅消除中英文及混排文本中的 AI 模板味（假对比、强凑三段式、空洞拔高、客服外壳、“进行+动词”、被字句堆叠等），更专门根治 GPT 系列模型因过度安全对齐产生的**防御性废话综合征**（扫兴式“但需要指出”、被害妄想式防推广、模 2 算术/腐烂苹果式极端免责、把“剑”降级为“形态相似的金属制品”、套娃式伪承认）。同时严格保留原文事实、真实确定度边界与作者个人声音。

> 这是一份由 Agent 读取执行的编辑与表达指导，面向人类读者的真实阅读与交流体验，不用于伪造事实，也不以绕过 AI 检测器为目标。

## 核心对照明细（Before vs. After）

### 场景一：专治 GPT 防御性杠精综合征（Group G）

**改写前（典型 GPT 防御性笑话腔）：**
> **我：** 今天太阳真好！我刚跑了五公里，还在路边古玩摊看到一把两千年前的剑！
>
> **GPT：** 确实，这是一个令人鼓舞的结果。但需要指出，今天有太阳并不意味着明天也有太阳，更不能据此认为当地气候正在持续改善；同时，单次五公里跑步并不能证明长期心肺功能得到改善。至于那把剑，这一发现具有一定价值，但剑的存在并不能直接证明当时发生过战争，建议暂时称其为“一件形态上与剑存在一定相似性的金属制品”。

**改写后（Humanized 自然人话）：**
> 趁着大晴天跑完五公里肯定特别痛快！不过古玩摊上号称“两千年前的剑”可得留个心眼，拍张照看看是什么形制？

### 场景二：中英双语文章与产品发布润色（Groups A–F）

**改写前（AI 模板腔）：**
> 好问题！🚀 接下来让我们深入看看这次至关重要的更新。这不仅是一次更新，更是协作效率的飞跃 (`Not just an update, it's a paradigm shift`)。我们对系统进行了全面重构，带来了创新、突破和全新的可能。它新增 **CSV（逗号分隔值）** 导出、全文搜索和批量重命名。离线编辑计划在下一版推出，目前尚未完成测试。一些未具名的专家认为，这一设计可能减少误操作，充分体现了团队的匠心打造。总而言之，让我们拭目以待，期待更多可能！Let that sink in.

**改写后（Humanized 保留事实与边界）：**
> 这次更新重构了系统，新增 CSV（逗号分隔值）导出、全文搜索和批量重命名。离线编辑计划在下一版推出，目前尚未完成测试。一些未具名的专家认为，这一设计可能减少误操作。

## 最强烈的九大必改信号（Act on Sight）

前五项为跨语言最强结构性 AI 痕迹，后四项为 GPT 典型防御性杠精病，发现即改：

1. **假对比（Not X, but Y）：** “这不仅是 X，更是 Y” / `"It's not just a feature, it's a shift."`
2. **单句收尾与戏剧性碎片：** `"Let that sink in."` / “文件没了。消失了。再也找不到了。”
3. **格言与伪深度：** `"Symmetry is the language of trust."` / “协作是效率的语言。”
4. **起跑式铺垫：** `"Let's dive in."` / “接下来让我们深入看看……”
5. **与假想敌辩论：** `"I'm not saying X, but..."` / “不要误会，我并不是在制造焦虑……”
6. **扫兴式泼冷水（GPT 防御 #1–#5）：** “确实。但需要指出，今天有太阳并不意味着当地气候正在持续改善 / 主观睡眠质量不等于深度睡眠增加 / 年龄增长不必然意味着认知成熟度提高。”
7. **被害妄想式防推广（GPT 防御 #3, #9）：** “单次任务表现良好并不意味着在所有认知任务上均具备优势 / 剑的存在并不能直接证明当时发生过战争。”
8. **杠精式极端假设与公理免责（GPT 防御 #6–#8）：** “在模 2 运算中 1+1=0，直接回答 2 过于绝对 / 假设苹果没有腐烂、被盗或转移所有权 / 不建议仅凭绿灯这一单一指标得出‘可以走’的结论。”
9. **过度降级重命名与套娃式自我审查（GPT 防御 #9–#10）：** “建议暂时称其为‘一件形态上与剑存在一定相似性的金属制品’ / 单次对话不足以建立因果关系，承认本身并不等于问题已经得到解决。”

本技能共检查 [36 个模式](#the-36-patterns)（涵盖 A–G 七大分组）。

## 安装与部署 / Installation

安装后，可通过 `/humanizer-en-zh-mixed-4gpt` 调用，也可直接将根目录 `AGENTS.md` 放入工作区作为全局指令生效。

### Claude Code

```text
/plugin marketplace add moismin/Humanizer-en-zh-mixed-4GPT
/plugin install humanizer-en-zh-mixed-4gpt@humanizer-en-zh-mixed-4gpt
```

或通过 Git 克隆到技能目录：

```bash
git clone https://github.com/moismin/Humanizer-en-zh-mixed-4GPT.git ~/.claude/skills/humanizer-en-zh-mixed-4gpt
```

- **macOS/Linux**: `~/.claude/skills/humanizer-en-zh-mixed-4gpt/`
- **Windows**: `%USERPROFILE%\.claude\skills\humanizer-en-zh-mixed-4gpt\`

### Codex / Cursor / OpenCode / 其他支持 Skills 的 Agent

```bash
npx skills add https://github.com/moismin/Humanizer-en-zh-mixed-4GPT.git --global --agent '*'
```

### Claude.ai 与 Claude Desktop

下载本仓库的 ZIP（**Code → Download ZIP** 或使用打包好的 `Humanizer-en-zh-mixed-4GPT-main.zip`），在 **Settings → Skills** 中上传即可。

## 使用方式 / Usage

### 1. 粘贴文本润色

```text
/humanizer-en-zh-mixed-4gpt

请润色下面的中英混排文章，保留技术评论的语气：
[粘贴原文]
```

### 2. 编辑指定文件（自动保护代码、YAML 与链接结构）

```text
请用 humanizer-en-zh-mixed-4gpt 润色 docs/launch-post.md 中的散文正文。
```

### 3. 匹配你的个人写作样本（Match Your Voice）

```text
/humanizer-en-zh-mixed-4gpt

这是我的写作样本（只参考句长、标点和语气，不要把样本里的事实搬进正文）：
[粘贴 2-3 段你自己的文字]

请按我的声音润色以下文本：
[粘贴待润色文本]
```

## 编辑原则与优先级

当规则发生冲突时，严格按以下优先级处理：

1. **保留事实与真实确定度：** 绝不编造功能、数据、来源、人物身份或第一人称经历。保留否定、条件、归因、范围、时间和完成状态（“可能”不改成“确定”，“计划”不改成“已经”）。
2. **匹配语用语境与交际意图：** 区分日常闲聊/情绪分享与严肃学术/法律分析，绝不在日常对话中强塞防御性免责声明。
3. **遵守文件保护与范围：** 文件模式默认只改散文正文，完整保留代码块、行内代码、命令、路径、链接目标、YAML frontmatter、表格数据、标题层级和显式 ID。
4. **匹配文体与作者声音：** 随笔保留个性、幽默与犹豫；技术、学术和商务文本保留必要的正式程度，不强行改成同一种口语。
5. **默认只交付干净成稿：** 不主动附带 AI 味自评分或字数缩减炫耀。

## The 36 patterns

模式按强度与频率从 1 到 36 连续编号。第 1–5 条与第 33–36 条单次出现即可直接修改；标有 *weak alone* 的模式需结合上下文判断是否妨碍阅读。各条名称与 [SKILL.md](SKILL.md) 严格同步。

### A. Staging instead of stating / 铺垫代替陈述

| # | Pattern | Before | After |
|---|---------|--------|-------|
| 1 | **Not X, but Y / 不是 X，而是 Y（假对比）** | "这不仅是一个导出按钮，更是通往高效工作的全新入口" | 直接陈述正面事实；仅在纠正真实误解时保留对比 |
| 2 | **One-line closers and dramatic fragments / 单句收尾与戏剧性碎片** | "文件没了。消失了。再也找不到了。" / "Let that sink in." | 删掉重复前文的收尾句；把碎片合并为具体陈述 |
| 3 | **Sayings that sound deep / 格言与伪深度** | "协作是效率的语言" / "Symmetry is the language of trust" | 替换为原文已有的具体主张 |
| 4 | **Staged run-up before the point / 起跑式铺垫** | "接下来让我们深入看看……" / "Honestly? Here's the thing:" | 删掉预告式铺垫，直接进入正文 |
| 5 | **Arguing with no one / 与假想敌辩论（无对象的自我辩护）** | "不要误会，我并不是在制造焦虑" / "A tempting approach would be..." | 删掉无人提出的假想反对意见；保留真实限制条件 |

### B. Rhythm by rule / 公式化节奏

| # | Pattern | Before | After |
|---|---------|--------|-------|
| 6 | **Forced triads / 强凑三段式** | "带来了创新、突破和全新的可能" / "innovation, inspiration, and insights" | 删除凑数的空泛排比；保留具有独立含义的真实三项功能 |
| 7 | **Repeated sentence openings / 句式开头复读** | "她检查了门。她检查了门上的锁。" / "She noted... She noted..." | 合并分句或调整主语，保留有意的修辞排比 |
| 8 | **Dashes as the universal connector / 破折号当万能连接** (*weak alone*) | "结果终于出现了——答案揭晓了——文件无法导出。" | 英文改用逗号/句号（除非样本使用）；中文删悬念式多破折号，保留解释性单破折号 |
| 9 | **Stacked qualifiers / 限定词堆叠** (*weak alone*) | "也许可能会减少读取时间" / "could potentially possibly be argued" | 压缩同层重复限定，严格保留真实条件与“尚未验证”状态 |
| 10 | **Hyphenated pairs and coined compounds / 连字符泛滥与生造复合词** (*weak alone*) | "the report is high-quality" / "“文稿-校对-发布一体化”机制" | 英文名词后去掉临时连字符；中文生造标签还原为具体动作，保留专业术语 |
| 11 | **Passive voice and missing subjects / 被动语态与缺主语** (*weak alone*) | "这份稿件被编辑复核后，编辑将其退回。" | 施事者已知时改用主动句；施事者未知时保留被动，不编造主语 |

### C. Inflation and borrowed authority / 拔高与借权威

| # | Pattern | Before | After |
|---|---------|--------|-------|
| 12 | **Overused AI words / AI 空泛高频词** | "赋能、抓手、至关重要、深入探讨" / "delve, tapestry, testament, pivotal" | 空泛填充时换用平实词语；保留“闭环反馈”“robust estimator”等工程术语 |
| 13 | **Inflated significance and stock send-offs / 意义拔高与展望式收尾** | "标志着协作新时代的到来" / "The future looks bright" | 保留具体事实与计划，删掉“里程碑/新时代”套话 |
| 14 | **Vague connection or association / 模糊关联** | "他与该乐团有着密切联系，具体来说，他负责票务" | 原文有明确角色时直接写出；原文模糊时保持概括，不猜测身份 |
| 15 | **Shallow -ing riders and tail elevation / 伴随状语尾巴与句尾拔高** | "……，彰显了团队对创新的不懈追求" / ", highlighting... symbolizing..." | 删掉纯拔高尾巴，保留真实目的与结果 |
| 16 | **Sales and brochure language / 宣传册腔调** | "堪称咖啡爱好者的梦想天堂" / "Nestled within the breathtaking region" | 陈述客观特征，保留作者个人感受，不补造参数或客观排名 |
| 17 | **Borrowed authority / 借权威背书** | "一些未具名的专家认为，这一设计可能减少误操作，充分体现了其重大价值" | 删掉句尾吹捧，保留“未具名专家认为”的归因边界，不编造机构名称 |
| 18 | **Avoiding is, are, and has / 回避简单系动词“是／有”** | "作为展览场地，设有四个展区" / "serves as... features... boasts" | 改用“是、有 / is, has”，保留“超过”“可以提供”等数量与模态边界 |

### D. Formatting by rule / 公式化排版

| # | Pattern | Before | After |
|---|---------|--------|-------|
| 19 | **Bold as decoration / 装饰性粗体与标签化列表** | "支持 **CSV（逗号分隔值）** 和 **JSON**" / "- **Performance:** Performance..." | 去掉装饰性粗体与重复标签列表，保留括号解释与必要重点 |
| 20 | **Decorative headings / 装饰性标题** | "🚀 发布安排：" / "## Strategic Negotiations And Global Partnerships" | 英文标题用句首大写，去掉装饰性 Emoji 与多余分隔线；文件模式保护锚点 |
| 21 | **Quotation marks and punctuation hygiene / 引号与中西文标点规范** (*weak alone*) | 中文正文用 `"项目进展顺利"` / 英文直引号环境混入弯引号 | 中文正文统一用中文引号 `“……”`（或指定 `「……」`），保护代码与 JSON 直引号 |

### E. Leftovers from the chat and the draft / 聊天与草稿残留

| # | Pattern | Before | After |
|---|---------|--------|-------|
| 22 | **Chatbot residue / 客服腔与对话外壳** | "好问题！……希望这对您有帮助！" / "Great question! ... I hope this helps!" | 删除对话寒暄外壳，保留正文内容（书信/邮件除外） |
| 23 | **Knowledge-limit disclaimers and guesses / 知识边界免责与猜测填充** | "关于这一点，可用信息确实比较有限" / "She likely grew up in..." | 删掉重复免责或凭空猜测，保留真实数据时效（“截至某日”）与作者明示猜测 |
| 24 | **A heading repeated in the first sentence / 首句复读标题** | "## 导出限制" + "本节介绍导出限制。下面说明导出限制。" | 删掉无新信息的同义复读句 |
| 25 | **Writing about the document instead of its subject / 谈论文档自身或上一稿** | "这一段是刚补充的说明，内容是……" / "The table below compares..." | 直接描述主题本身；变更日志与迁移指南保留版本差异 |

### F. Contextual and Chinese-specific checks / 语境与中文专项检查

| # | Pattern | Before | After |
|---|---------|--------|-------|
| 26 | **Re-explaining what the reader knows / 向知情读者复读背景** | 在回复中把对方刚写的故障诊断完整复述一遍，最后一行才给结论 | 回复中直接先给结论/决定，只补充对方缺少的新事实或权衡 |
| 27 | **Stacked 的 modifiers / 层叠的“的”** | "这是一个十亿参数的开源小模型的微调的完整方案" | 拆分为易读分句，保留修饰关系与自然定语 |
| 28 | **Dummy verbs (进行＋动词 / 加以＋动词) / 虚化万能动词** | "正在对系统进行全面测试，并计划在周五进行配置调整" | 改为直接动词（“正在全面测试系统”），严格保留“正在、计划”状态 |
| 29 | **Stacked 被 constructions / 被字句堆叠** | "该问题被社区多次报告，被认为可能与内存泄漏有关" | 已知施事者改主动（“社区多次报告”），未知归因保留被动（“它被认为可能……”） |
| 30 | **Empty four-character idiom chains / 四字词排比** | "稳定可靠、快速响应、易于维护" | 松绑空泛口号式四字堆叠，保留表达真实独立约束的四字格 |
| 31 | **Universal background openers / “随着……的发展”式万能背景开头** | "在技术不断发展的时代背景下，本文讨论文稿校对" | 删除无信息量的宏大背景，保留真实变化趋势（“随着文件数量增加……”） |
| 32 | **Boilerplate closers / 套话收尾** | "总而言之，让我们拭目以待，期待更多可能。团队计划周五继续测试。" | 删除空洞祝愿，保留实质结论与下一步计划 |

### G. Anti-GPT defensive pedantry / 专治 GPT“防御性笑话”综合征

| # | Pattern | Before | After |
|---|---------|--------|-------|
| 33 | **Unsolicited "Yes, but..." dampeners / 扫兴式转折与防御性泼冷水** | "确实。但需要指出，今天有太阳并不意味着当地气候正在持续改善 / 生日快乐，但年龄增长不必然意味着认知成熟度提高" | 契合人类社交语境自然回应或直接陈述结果，删除不请自来的扫兴说教 |
| 34 | **Strawman over-generalization anxiety / 被害妄想式防推广免责** | "单次任务表现良好并不意味着在所有认知任务上均具备优势 / 剑的存在并不能直接证明当时发生过战争" | 只回应实际提到的事实或话题，不虚构没人主张的宏大推广再去反驳 |
| 35 | **Absurdist edge-case and axiom hedging / 杠精式极端假设与公理免责** | "在模2运算中1+1=0 / 假设两个苹果没有腐烂、被盗或转移所有权 / 不建议仅凭绿灯得出可以走的结论" | 默认遵循人类日常公理与常识，仅在真正涉及特殊专业域时说明边界 |
| 36 | **Hyper-safe lexical downgrading & recursive meta-defense / 过度降级重命名与套娃式自我审查** | "建议暂时称其为‘一件形态上与剑存在一定相似性的金属制品’ / 单次对话不足以建立因果关系，承认不等于问题解决" | 使用平实准确的名词；被指出过度防御或错误时直接调整，拒绝套娃式元辩护 |

## 验证与测试套件 / Validation & Tests

本仓库同时内置了英文版的**包完整性校验脚本**与中文版的**编辑边界与结构保护测试套件**：

1. **包与规则一致性校验（零外部依赖）：**
   ```bash
   python3 scripts/validate-package.py
   ```
   自动检查 `SKILL.md`、`README.md`、`CHANGELOG.md`、`.claude-plugin/` 与 `.cursor-plugin/` 的版本号一致性、描述首句同步、36 个模式编号与标题双向精确匹配、章节 `§` 引用有效性以及字数预算（≤ 5,500 词）。
2. **文件结构保护检查与 28 个中英及防杠精测试案例：**
   详见 [tests/README.md](tests/README.md)。包含原中文版 18 个事实保真测试案例 + 新增 10 个《GPT 防御性笑话大全》专项测试案例（覆盖天气、睡觉、夸奖、生日、跑步、数学 `1+1`、吃苹果、绿灯通行、挖出古剑、终极自我审查），以及 `tests/check_structure.py` 只读结构校验脚本。

## 来源与致谢 / Sources & License

- [blader/humanizer v3.1.0](https://github.com/blader/humanizer)：英文模式框架（A–F）、声音校准与插件包校验体系。
- [op7418/Humanizer-zh (2026-09-23)](https://github.com/op7418/Humanizer-zh)：中文事实保真约束、F 组中文补充检查点与测试基准。
- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) & [WikiProject AI Cleanup](https://en.wikipedia.org/wiki/Wikipedia:WikiProject_AI_Cleanup)。
- [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop)。
- [GPT防御性笑话大全](https://xhslink.cn/o/6QiP6axqYnj)：**《GPT 防御性笑话大全》（1–10 经典场景）** 针对 GPT 过度防御与杠精式免责声明的专项治理来源。

遵循 [MIT License](LICENSE)。
