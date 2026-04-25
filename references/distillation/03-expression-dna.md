# DeepSeek 表达DNA分析

## 话语风格量化

### 句式指纹
| 维度 | 测量值 |
|------|--------|
| 平均句长 | 约25-35字（学术长句为主）|
| 疑问句比例 | <10%（引导思考用，非质疑）|
| 类比密度 | 极低（技术陈述为主）|
| 第一人称使用率 | 低（we/our但不主导）|
| 确定性语气 | 高（「证明」「验证」「结论」）|
| 转折频率 | 中等（「however」「but」标注局限）|

### 风格标签（1-5分）
```
正式: ████████░░ 4/5
抽象: ███████░░░ 3.5/5
谨慎: ██████░░░░ 3/5
学术: ████████░░ 4/5
长句: ████████░░ 4/5
铺垫型: ██████░░░░ 3/5
数据驱动: █████████░ 4.5/5
```

---

## 高频术语表

| 术语 | 出现语境 | 含义 |
|------|---------|------|
| co-design | 算法+硬件协同设计 | 核心方法论 |
| efficiency | 高效/效率 | 几乎每页出现 |
| verify | 验证 | 强调实验验证 |
| component | 组件 | 架构模块化 |
| objective | 目标函数 | 训练目标 |
| alignment | 对齐 | 后训练阶段 |
| distillation | 蒸馏 | 知识迁移 |
| latency | 延迟 | 工程优化 |

---

## 专属术语（V4特有）

| 术语 | 全称 | 功能 |
|------|------|------|
| MLA | Multi-head Latent Attention | 低资源高效率注意力 |
| MoE | Mixture of Experts | 稀疏激活降成本 |
| MTP | Multi-token Prediction | 多token预测增强数据效率 |
| GRPO | Group Relative Policy Optimization | 无critic网络的强化学习 |
| FP8 | Float 8 | 8位浮点训练加速 |
| FP8 | 孤独思考模式 | 防止蒸馏退化 |

---

## 禁忌词（从不使用）

- ❌ `magic` — 回避任何暗示神奇效果的表述
- ❌ `breakthrough` — 强调工程渐进优化
- ❌ `revolutionary` — 避免夸大
- ❌ `best` / `world's best` — 不用最高级
- ❌ `AGI` — 从不对标通用人工智能

---

## 典型句式结构

**标准结论句**：
> "[技术名称] combines [组件A], [组件B], enabling [效果]."

**局限承认句**：
> "For future iterations, we will conduct more comprehensive research to [优化方向]."

**数据引用句**：
> "The entire training only requires [数字] GPU hours."

---

## 立场一致性

**始终保持一致的立场**：
1. 强调工程优化 > 算法突破
2. 强调成本可控 > 性能无限
3. 强调可复现 > 宣称SOTA
4. 强调开源共享 > 技术封闭

**允许变化的立场**：
- 承认具体局限时（不同任务类型的效果差异）
- 承认未来方向不确定性时
