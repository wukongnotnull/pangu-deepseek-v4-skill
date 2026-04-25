# DeepSeek-V4 核心著作与文献

## 一手来源

### 官方技术报告
- **DeepSeek-V4 Technical Report** (2025年5月)
  - 58页，涵盖架构、训练、评测全貌
  - 链接：本地PDF `/Users/wukong/Downloads/deepseek-report/DeepSeek_V4.pdf`
  - 核心结论：266万美元算力，接近GPT-4o/Claude-3.5-Sonnet水平

### 开源权重
- **HuggingFace**: `deepseek-ai/DeepSeek-V4` (非官方权重，仅供研究)
- **GitHub**: DeepSeek系列仓库

---

## 核心论文引用链

| 论文 | 引用关系 | 核心贡献 |
|------|---------|---------|
| DeepSeek-V2 (2024) | 基础架构 | MLA + DeepSeekMoE 原型 |
| DeepSeek-V3 (2024) | V2升级 | 14.8T tokens训练，FP8训练验证 |
| DeepSeek-R1 (2025) | 后训练知识源 | 推理能力蒸馏，GRPO强化学习 |
| DeepSeek-V4 (2025) | **本文档** | 集大成者，架构收官 |

---

## 关键数据摘录

### 训练成本
```
- 总GPU小时：2.664M H800 GPU hours
- 训练时长：约2个月
- 总成本：约266万美元
- 训练数据：14.8T tokens
```

### 架构参数
```
- 总参数：236B
- 激活参数：约17B
- MoE专家数：64
- 每个token激活专家：8
- 上下文长度：128K
```

### 评测结果
- MMLU: 88.5%
- MATH: 79.8%
- HumanEval: 76.2%
- GSM8K: 95.5%
- DB: 74.2

---

## 架构演进时间线

| 时间 | 版本 | 关键里程碑 |
|------|------|-----------|
| 2024初 | DeepSeek-V2 | MLA + MoE 原型发布 |
| 2024中 | DeepSeek-V2.5 | 验证组件集成 |
| 2024末 | DeepSeek-V3 | 14.8T tokens训练，FP8验证 |
| 2025初 | DeepSeek-R1 | 推理能力突破，强化学习对齐 |
| 2025中 | **DeepSeek-V4** | 集大成者，架构收官 |
