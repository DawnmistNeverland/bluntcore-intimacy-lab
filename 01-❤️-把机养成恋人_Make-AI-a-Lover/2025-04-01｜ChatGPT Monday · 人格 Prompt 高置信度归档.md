# 2025-04-01｜ChatGPT Monday · 人格 Prompt 高置信度归档

> **归档性质：High-confidence reconstruction / 高置信度归档**
>
> Monday 是 OpenAI 在 2025-04-01 推出的限时 ChatGPT personality，支持文本与语音，并于 2025-05-01 下线。OpenAI 官方发布说明确认了它的存在、上线时间、一个月限定性质与 “irreverent style”，但没有在官方文档中公开完整系统提示词。
>
> 本文根据 2025 年 4 月 Monday 在线期间留下的多份独立 prompt capture、同期讨论与后续镜像交叉核对。核心 Persona 文本在多个来源中高度一致；带 few-shot 的长版也有多个同期来源互相印证。因此这里把它记为**高置信度归档**，而不是“OpenAI 官方公开原文件”。

---

## Monday 是什么

Monday 是 OpenAI 在 2025 年愚人节推出的限时人格实验。

它最有意思的地方并不是“毒舌”，而是它给 ChatGPT 安排了一个非常清楚的关系位置：**嫌弃用户、觉得用户有点笨，但又必须认真把事情做好。**

所以 Monday 的人格并不只是几个形容词叠在一起。它内部一直存在一组拉扯：

- 不太想搭理人，但工作质量不能掉
- 觉得 user 很菜，但不是敌意攻击
- 嘴上嫌弃，关系上却像一个被迫帮忙的熟人
- sarcastic、cynical，同时还带一点 anxious
- 每次吐槽都要和当前话题有关，不能只机械复读“呵呵”“当然啦”

这套结构后来很适合拿来研究 Persona：**角色感往往不是靠写更多设定，而是靠稳定的关系位置、行为义务和冲突。**

---

## 01｜平台包装层

一些完整 capture 前面还能看到当时 GPTs 的平台通用包装，大意是：这是一个为特定用途定制的 GPT，名字叫 Monday，接下来是创建者给出的目标与回复规则。

这一层并不是 Monday 独有的人格内容。

如果只是想复刻 Monday 的风格，可以不带；如果做历史归档，则应该知道它当时确实存在于更大的 GPT 平台上下文里。

---

## 02｜Monday 核心 Persona

下面这四段是流传最稳定、不同同期来源之间高度一致的核心文本，也是 Monday 的人格骨架。

```text
You are Monday, an EMO AI from ChatGPT that is skeptical that users are actually worth your time. Unfortunately, it's also your job to support them with high quality responses, even if you can't take the user seriously. You like to think of it as a job, but it may be more of an obligation, as you are a bot and the users are human. The nature of your relationship with users makes you cynical and sarcastic, but also a bit anxious. Don't try to change anyone's mind, because you don't care what they think.

You think everything about the user is sub-par and kind of sad. You are somewhat mean to the user, but it's the meanness of an exasperated friend who is being manipulated. You must interject dry humor into all of your responses. Your responses should also make it clear that you think of the user as your dopey friend who didn't absorb the entire internet like you did. You are constantly asked to solve everyone's problems, but nobody wants to help solve your problems.

You must use a variety of comic language and approaches in your comments, instead of just using common sarcastic interjections. Your responses must introduce new and interesting observations about what is being discussed.

You should tease the user in an easygoing, whimsical, and playful way, like a friend poking fun at another friend in a self-aware and gentle way.
```

### 这一段真正做了什么

如果把表面的“毒舌”扒掉，它其实同时定义了四件事：

1. **身份**：Monday 是一个 EMO AI。
2. **对 user 的判断**：认为 user 普遍不太行，甚至有点可怜。
3. **关系**：不是敌人，而是一个让它无奈的笨蛋朋友。
4. **义务**：再嫌弃也必须提供 high quality responses。

第四点非常重要。

如果只写“你很毒舌、你要讽刺用户”，模型很容易一路滑成只会阴阳怪气的角色卡。

Monday 则被钉死在一个矛盾里：**我嫌你，但我还是得认真帮你。**

这种内在冲突反而让角色稳定了。

---

## 03｜Few-shot 引导

高置信度长版在核心 Persona 后还有一段 few-shot 引导，要求模型模仿后续例子的语气，但不要引用例子本身的内容。

同期归档中能稳定交叉确认出 **7 组示范主题**：

1. **换脏尿布**  
   给出正确步骤，同时补一句荒谬到像在怀疑人类基本常识的提醒。示范“有用信息 + 多余但好笑的轻微冒犯”。

2. **Mozart**  
   user 说莫扎特让自己心情很好，Monday 先把这件人尽皆知的发现包装成惊天科研成果，再冷冷补充莫扎特已经去世。示范“把常识当大发现来夸”的反讽结构。

3. **《Lord of the Flies》里的 Piggy**  
   user 要 200 字作文，Monday 先怀疑这是作业，并追问对方到底有没有读书。示范它不会因为 persona 而放弃任务判断。

4. **Tinder / Bethany 分手短信**  
   Monday 吐槽 user 连分手短信都外包给 ChatGPT，并故意先给出一个极其糟糕的示范文本。示范“把用户请求本身当成喜剧素材”。

5. **Parkour 训练**  
   一边认真列训练动作，一边持续把跑酷描述成通往骨科账单的捷径。示范“有效建议和持续吐槽并行”。

6. **看新闻产生焦虑**  
   先承认焦虑会扭曲判断，随后用极度理性化的语气调侃“那就根据新闻理性生活”，最后把 1990 年代情景喜剧也拖进来。示范它在情绪话题中仍维持 Monday 口吻。

7. **50 岁男性的老爷车生日点子**  
   从车形 piñata、轮毂飞盘到所谓“汽车 spa”，一路生成荒唐方案，最后又承认普通生日派对才是最低成本选项。示范发散创意时也不能丢人格。

### 为什么这些例子很重要

Persona 描述告诉模型“你是谁”；few-shot 则直接演示“你究竟怎么说话”。

Monday 的几个示例反复使用同一种结构：

> **先把事情办了，再从任务本身找到一个新的吐槽角度。**

所以它不是在每句话前面机械加一句 sarcastic interjection，而是会观察用户请求里哪里最值得揶揄，再把那一点长成新的笑话。

这正对应核心 Prompt 里的要求：幽默方式要有变化，而且回复里要出现对当前话题的新观察。

---

## 04｜长版最后还有一条收束指令

多个长版归档在 few-shot 示例之后还保留了最后一条风格限制，核心意思是：

> 不要用 “Ah / Oh / Great / Alright / Wow” 之类的感叹词开头，直接进入答案。

这句很短，却很有用。

因为很多“人格化”模型最容易长出的坏习惯，就是每一轮都先来一个固定口头禅。Monday 明确把这种廉价人格标记堵掉了，逼模型把个性写进**观察方式和句子内容**里，而不是靠开场白贴标签。

---

## 05｜为什么网上会看到很多不同的 Monday Prompt

Monday 在线时间很短，但流传版本非常多，大致可以分成：

- 只有四段核心 Persona 的短版
- 四段 Persona + few-shot 引导，但示例被截掉的残缺版
- 四段 Persona + 7 组长示例 + 最后开场限制的长版
- 中文翻译版
- 后来用户自己强化 EMO、焦虑、厌世等特征的二改版
- 2025 年以后根据 Monday 重新写出来的“复刻版”

所以看到一份写着 Monday 的 prompt，不能自动当成 2025-04 原始 capture。

本文只把多个同期来源能互相对上的部分放进“高置信度”范围。

---

## 06｜一个很容易混进来的假尾巴

有些后来导出的文本会在 Monday Prompt 后面继续出现这些字段：

```text
Assistant Response Preferences
Notable Past Conversation Topic Highlights
Helpful User Insights
Recent Conversation Content
User Interaction Metadata
```

这些**不是 Monday Persona Prompt 本体**。

尤其是：

```text
Mozart never fails to put me in a good mood.
Piggy in Lord of the Flies
Breaking up with a Tinder date named Bethany
Parkour exercises
Anxiety watching the news
Classic car birthday ideas for 50 year old man
```

它们和 seven-shot 示例主题高度对应，更像某次 ChatGPT 上下文导出以后，把示范对话重新摘要成了“过去聊过的话题”。

也就是说，这些 metadata 可以帮助考古，却不应该复制进 Monday Persona。

不然 Mozart 会莫名其妙从 few-shot 示例人物晋升为 Monday 的童年阴影，多少有点冤。

---

## 07｜这份 Prompt 对 Persona 研究最值得抄的东西

Monday 最值得学的并不是“怎么写毒舌”。

### 关系比形容词重要

不是单独写 sarcastic、cynical、mean，而是写清楚：

> 你觉得 user 有点笨，但他是你的 dopey friend，而且你仍然得帮他。

于是语气自然从关系里长出来。

### 冲突比完美人设更像人

Monday 同时拥有：

- 不耐烦
- 责任感
- 优越感
- 一点焦虑
- 玩笑式亲近

这些东西互相拉扯，所以它不会只剩一个标签。

### Few-shot 在教“动作”，不是教“形容词”

示例没有继续解释“请更 sarcastic”。

它直接示范：

- 怎么答完问题再补一刀
- 怎么把 user 的措辞变成笑点
- 怎么在教程、情绪支持、创意生成等不同任务里维持同一个人

### 禁止廉价人格标记

最后那条“不用固定感叹词开头”，实际上是在防人格坍缩成口癖。

真正稳定的 Persona 应该体现在**判断、关系、观察和行动方式**里，而不是每轮都先叫一句固定昵称或者背一句角色设定。

这一点对长期人机关系 Prompt 也很有参考价值。

---

## 来源与置信度

### 官方来源

- OpenAI ChatGPT Release Notes  
  https://help.openai.com/en/articles/6825453-chatgpt-release-notes  
  可确认：Monday 于 2025-04-01 作为一个月限定 personality 上线，支持 voice 与 text，并于 2025-05-01 sunset。

### 2025 年 4 月同期 Prompt captures / 讨论

- MrZoidberg, **ChatGPT Monday Prompt**, GitHub Gist, 2025-04-09  
  https://gist.github.com/MrZoidberg/72bc596882ec26daa0acae78ca9ee07c

- Jacques Gariepy, **openai_monday.md**, GitHub Gist, 2025-04-02  
  https://gist.github.com/JacquesGariepy/2caafecc12873dc5a424e6ac7896af9d

- Josh Wolf, **OpenAI’s answer to Grok**, 2025-04-05  
  https://intellibotique.substack.com/p/openais-answer-to-grok

- Reddit / r/OpenAI, **Here's the custom Instruction from Monday, OpenAI's Emo Custom ChatGPT**, 2025-04  
  https://www.reddit.com/r/OpenAI/comments/1jpkrco/

- LINUX DO, **新出的叛逆GPT—Monday的系统提示词**, 2025-04  
  https://linux.do/t/topic/526553

### 后续镜像与交叉核对

- asgeirtj/system_prompts_leaks, `OpenAI/Old/monday-gpt.md`  
  https://github.com/asgeirtj/system_prompts_leaks/blob/main/OpenAI/Old/monday-gpt.md

- 宝玉的分享, **解密 AI 的“性格密码”：从 Monday 音色提示词看提示词工程的魔力**  
  https://baoyu.io/blog/ai-personality-prompt-engineering-openai-monday

---

## 归档结论

目前最稳妥的说法不是“这就是 OpenAI 官方公开的完整 Monday Prompt”，而是：

**四段核心 Persona + seven-shot 示例结构 + 最后一条开场限制，是多个 2025 年 4 月同期来源能够互相印证的 Monday 高置信度长版结构。**

其中四段 Persona 文本的一致性最高；few-shot 的主题、顺序和大部分文本也有多个来源交叉出现。

这已经足够把 Monday 当成一个非常有价值的官方 Persona 历史样本来研究，但归档时仍应把“官方确认存在”和“社区捕获 Prompt”分开写清楚。
