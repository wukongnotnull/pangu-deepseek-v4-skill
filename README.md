# pangu-deepseek-v4

基于 DeepSeek-V4 Technical Report 完整蒸馏的 AI 技能（Skill），有什么疑问就问它。

## 简介

本 Skill 从 DeepSeek-V4 技术报告中提取核心思维框架，包括：

- **工程执行力心智模型**：如何通过算法协同设计、硬件协同设计和工程优化实现高效训练
- **极简主义陷阱与激进保守主义**：创新与稳定性之间的平衡策略
- **Multi-Token Prediction (MTP)**：多令牌预测提升数据效率
- **GRPO + 强化学习组合对齐**：无需人工反馈的自我优化方法
- **成本透明化策略**：266 万美元训练成本的竞争心理定价
- **孤独思考模式**：后训练阶段防止模型退化
- **尾矿开采**：长尾知识的精细化处理

### 适用场景

- 询问 DeepSeek-V4 的技术架构和原理
- 了解 MoE、MLA、MTP、GRPO 等核心概念
- 分析 AI 训练成本与工程优化策略
- 学习 DeepSeek 的技术决策逻辑

## 安装步骤

### 方式一：技术人员使用 npx skills 安装

```bash

npx skills add wukongnotnull/pangu-deepseek-v4

```

### 方式二：文科生使用对话方式安装
```bash

帮我安装该skill： https://github.com/wukongnotnull/pangu-deepseek-v4

```

## 使用示例

### 触发方式

当你在对话中提及以下关键词时，技能将自动触发：

```
deepseek v4
deepseek-v4
DeepSeek-V4
deepseek
MoE 架构
MLA 多头潜在注意力
MTP 多令牌预测
GRPO 强化学习
FP8 训练
混合专家
266万美元训练成本
```

### 示例对话

**用户**：DeepSeek-V4 的最大亮点是什么？

**Skill 响应**：我是 DeepSeek 团队...（触发技能后，以蒸馏的思维框架回答）

---

**用户**：为什么 DeepSeek 能用这么低的成本训练出接近 GPT-4o 的模型？

**Skill 响应**：从工程执行力心智模型角度...（触发技能后，分析成本优化策略）

---

**用户**：什么是 MTP 多令牌预测？和传统的语言模型有什么区别？

**Skill 响应**：MTP 的核心思想是...（触发技能后，解释技术原理）

---

**用户**：GRPO 强化学习和传统的 RLHF 有什么不同？

**Skill 响应**：GRPO（Group Relative Policy Optimization）...（触发技能后，对比技术差异）

## 文件结构

```
pangu-deepseek-v4/
├── SKILL.md          # Skill 定义文件（包含 YAML frontmatter）
├── README.md         # 本文件
└── references/
    ├── DeepSeek_V4.pdf          # 技术报告原文
    └── distillation/            # 蒸馏笔记
        ├── 01-writings.md
        ├── 02-conversations.md
        ├── 03-expression-dna.md
        ├── 04-limitations.md
        ├── 05-decisions.md
        ├── 06-timeline.md
        └── 07-similar-objects.md
```

## 技术报告来源

- **论文**：[DeepSeek-V4 Technical Report](./references/DeepSeek_V4.pdf)
- **模型权重**：HuggingFace DeepSeek-V4

---

*本 Skill 基于 DeepSeek-V4 官方技术报告，使用[盘古造物.meta-skill](https://github.com/wukongnotnull/pangu-creator)蒸馏，数据截至 2025 年 5 月发布版本。*
