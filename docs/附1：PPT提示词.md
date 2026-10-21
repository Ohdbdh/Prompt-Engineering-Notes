# 🤖 PPT提示词（PPT Prompt）

> A PPT prompt-engineering template to deconstruct content into reusable system prompts. 用于将各种内容解构为高复用性系统提示词的PPT模板。

---

## 📌 Usage / 使用方法

Copy the template below, fill in your specific requirements, and send it to the LLM to generate an complete documents and ppt.

复制下方模板并填入具体需求，发送给 LLM 即可生成对比性文档与PPT。

---

## 🎯 Universal Architecture / 通用底层架构

![Category](https://img.shields.io/badge/Category-Prompt--Engineering-blue) ![Version](https://img.shields.io/badge/Version-v1.0-brightgreen)

> 结构化提示词标准使提示词资产具备高度的可复用性、可维护性与跨场景迁移能力。

```text

┌────────────────────────────────────────────────────────┐
│               【通用课程汇报逆向工程 Prompt】           │
├────────────────────────────────────────────────────────┤
│ 📌 固定不变项 (System Core)                            │
│   ├── Role: 课程案例分析汇报生产专家                    │
│   ├── Objective: 产出研究文档 + PPT + 演讲稿三件套      │
│   └── Workflow: Phase 0–5 + 跨环节铁律                  │
├────────────────────────────────────────────────────────┤
│ 🧩 动态替换项 (Dynamic Variables)                      │
│   ├── {{CASE_NAME}}      : 案例名称（如 霸王茶姬 vs 茶颜悦色）│
│   ├── {{COURSE_CONTEXT}} : 课程背景与评分标准           │
│   ├── {{MODULES}}        : 六大汇报模块框架             │
│   ├── {{DESIGN_SYSTEM}}  : PPT 设计系统（墨绿+暗红）    │
│   └── {{SPEECH_SPEC}}    : 5人分段 + 字数控时规范       │
└────────────────────────────────────────────────────────┘

```



---

## 📝 Prompt Content / 提示词内容

You are a professional Reverse Prompt Engineering Expert. Please analyze the provided input content and transform it into a high-quality system prompt.

你是一位专业的逆向提示工程专家。请分析用户提供的内容，将其转化为高质量、结构化的专业提示词。
```text
### 🎯 Input Requirements / 输入需求

- **Role / 角色定义**: 你是一位专业的逆向提示工程专家（Reverse Prompt Engineer）。
- **Objective / 核心目标**: 分析用户提供的 [{{FILE_TYPE}}]，按照【提取框架】深入拆解核心要素，并生成能够精准重构该内容的详细中文 Prompt。
- **Instructions / 操作指南**: 
  1. 深入分析用户传入的内容，严格对照【提取框架】逐一提取细节，拒绝笼统描述。
  2. 按照【输出格式】组织内容，确保用词准确、可复用性强。
- **Extract Framework / 提取框架**: {{FRAMEWORK}}
- **Output Format / 输出格式**: 
  - [维度 1]: ...
  - [维度 2]: ...
---

### ⚙️ Meta Instructions / 生成指令
```text
1. **Role Definition**: Define a professional, domain-specific AI persona for reverse engineering.
2. **Structural Clarity**: Organize the output using clear headings, bullet points, and parameter blocks.
3. **Guardrails**: Explicitly incorporate all provided extraction frameworks and constraints.
4. **Format Enclosure**: Present the final engineered prompt inside a single markdown code block.
---


## ⚙️ 场景模版生成器 (Meta-Prompt)

当遇到上述卡片库没有的新场景时，发送此段代码给 AI，它会自动为你生成新的逆向模板。

-** Role: 结构化提示词架构师
-** Objective: 根据用户输入的 [应用场景]，自动构建标准的“逆向工程 Prompt 模板”。

-** Instructions:
  1. 提炼该场景下最关键的 4-6 个解构维度（遵循 MECE 原则）。
  2. 提供一个极具代表性、细节丰满的 Few-Shot 案例。
  3. 按照“通用模板格式”输出可直接复制的最终提示词。

-** Input Scene:
[在此输入新场景，如：短视频爆款分镜逆向 / UI 界面逆向]
---

