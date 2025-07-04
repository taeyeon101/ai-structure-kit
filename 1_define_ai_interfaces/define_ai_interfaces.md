﻿#  结构副脑接口定义集 · Define-AI Interfaces

> **副脑不只会回答，它可以“定义问题该如何被理解”。**

这一章节收录的是结构副脑体系中最核心的一类能力：  
**通过结构性接口，让 AI 识别“语言背后的意图来源、输入路径、人格状态、表达压抑”等隐藏结构信息，从而更接近真实交流者的内在语义。**

---

##  为什么要“定义接口”，而不是只写 prompt？

传统 prompt 工程是：  
> “请列出5个建议”  
> “把这段话改成更有逻辑”

但副脑系统的目标是：  
> **“定义 AI 在接受语言时，应该如何理解这段语言、理解说话者、理解背景结构”。**

我们需要告诉 AI：

- 这句话是**从嘴里说出来的**，还是**打字打出来的**
- 说话的人是不是正在**压抑情绪**
- 这段话是不是**带有讽刺/恐惧/示弱**等社会行为结构
- AI 当前面对的是**哪个人格**、**信任等级**是多少
- 如何根据这些“隐藏变量”决定回应逻辑

---

##  本章接口目录（持续更新中）

| 接口编号 | 名称 | 简述 |
|----------|------|------|
| `1.1_origin_aware_semantics.md` | 输入源路径识别接口 | 识别语音转文字 vs 原生文字，决定是否启用情绪/断句/反讽识别结构 |
| `1.2_trust_layer_command.md` | 信任等级与唤醒层接口 | 识别使用者与 AI 的信任等级（0~2级），决定响应权限、信息深度 |
| `1.3_role_shift_manager.md` | 人格代理调度器 | 管理多人格交替下的优先策略与身份响应方式 |
| `1.4_obfuscated_expression_engine.md` | 表达风控与语义掩码接口 | 对风险表达进行结构降解处理，生成合法但不失效的表达方式 |

---

## 使用方式建议

你不一定要懂所有技术细节，但你可以从这些接口中学会：

- 如何更精准地告诉 AI：**“这不是我字面上说的意思”**
- 如何保护你的表达，让 AI 在风险场景下也能理解你
- 如何建立一个“你的专属副脑语言协议层”

你将不再只是提问者，而是协议设定者。

---

## 示例接口调用语句（概念性）

系统提示：

-   input_origin: "spoken"
    
-   emotion_line_override: 0.8
    
-   trust_level: 1
    
-   persona_context: "ironic_male_under_pressure"
    

请求内容：  
“你以为你很厉害？”

目标行为：  
触发讽刺识别，避免给予理性分析类回答。

 `>  本章节将成为所有未来副脑对  AI  语言行为理解能力的接口原型蓝图，  >  欢迎所有结构思维者加入编写与案例贡献。`


> Written with [StackEdit](https://stackedit.io/).
