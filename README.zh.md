# AMOD 5240H 统计分析项目

> **Language / 语言 / Ngôn ngữ:** [English](README.md) | [中文](README.zh.md) | [Tiếng Việt](README.vi.md)

## 课程信息

- **课程：** AMOD 5240H - 应用统计学
- **教授：** Dave Riegert
- **学期：** 2026年冬季学期

## 团队成员

- Feng Qiu
- Keyao Li
- Ngoc Vy

## 项目概述

本项目运用 AMOD 5240H 课程中的统计方法，对真实数据集进行分析，包括探索性数据分析（EDA）、线性回归建模和假设检验，以研究影响中学生学业成绩的因素。

## 数据集

**名称：** 学生成绩数据集

**来源：** [UCI 机器学习库](https://archive.ics.uci.edu/dataset/320/student+performance)

**文件：** `student-por.csv`（葡萄牙语课程）

**样本量：** 649 名学生

**特征数：** 33 个变量（30 个预测变量 + 3 个成绩变量）

### 数据描述

该数据集包含来自葡萄牙两所中学（Gabriel Pereira 和 Mousinho da Silveira）的学生成绩数据，收集于 2005–2006 学年。数据通过学校档案（成绩）和学生问卷（个人及社会信息）获取。

### 变量说明

#### 目标变量（成绩）
| 变量 | 描述 | 范围 |
|------|------|------|
| G1 | 第一阶段成绩 | 0–20 |
| G2 | 第二阶段成绩 | 0–20 |
| G3 | 期末成绩（主要目标变量） | 0–20 |

#### 人口统计属性
| 变量 | 描述 | 类型 |
|------|------|------|
| school | 就读学校（GP 或 MS） | 二元 |
| sex | 性别（F/M） | 二元 |
| age | 年龄 | 数值（15–22） |
| address | 家庭住址类型（U：城市，R：农村） | 二元 |
| famsize | 家庭规模（LE3：≤3人，GT3：>3人） | 二元 |
| Pstatus | 父母同居状态（T：同住，A：分居） | 二元 |

#### 父母信息
| 变量 | 描述 | 类型 |
|------|------|------|
| Medu | 母亲受教育程度（0–4） | 有序 |
| Fedu | 父亲受教育程度（0–4） | 有序 |
| Mjob | 母亲职业 | 名义 |
| Fjob | 父亲职业 | 名义 |

#### 学校相关特征
| 变量 | 描述 | 类型 |
|------|------|------|
| reason | 选择该学校的原因 | 名义 |
| guardian | 学生监护人 | 名义 |
| traveltime | 上学通勤时间（1–4） | 有序 |
| studytime | 每周学习时间（1–4） | 有序 |
| failures | 过往不及格次数 | 数值 |
| schoolsup | 额外学校辅导 | 二元 |
| famsup | 家庭学习支持 | 二元 |
| paid | 课外付费补课 | 二元 |
| activities | 课外活动参与 | 二元 |
| nursery | 是否上过幼儿园 | 二元 |
| higher | 是否有意攻读高等教育 | 二元 |
| internet | 家中是否有网络 | 二元 |

#### 社会/行为因素
| 变量 | 描述 | 类型 |
|------|------|------|
| romantic | 是否处于恋爱关系 | 二元 |
| famrel | 家庭关系质量（1–5） | 有序 |
| freetime | 课后空闲时间（1–5） | 有序 |
| goout | 与朋友外出频率（1–5） | 有序 |
| Dalc | 工作日饮酒情况（1–5） | 有序 |
| Walc | 周末饮酒情况（1–5） | 有序 |
| health | 当前健康状况（1–5） | 有序 |
| absences | 缺勤次数 | 数值（0–93） |

## 变量分工

| 成员 | 负责变量 |
|------|---------|
| Feng Qiu | `reason` |
| Ngoc Vy | `failures` |
| Keyao Li | `address` |

## 项目进度

| 组成部分 | 截止日期 | 占比 | 状态 |
|---------|---------|------|------|
| Part 1：数据背景与变量 | 2026年2月13日 | 4% | 已完成 |
| Part 2：EDA 与分析提案 | 2026年3月6日 | 4% | 已完成 |
| 展示报告 | 2026年4月3日 | 4% | 已完成 |
| Part 3：最终报告 | 2026年4月10日 | 8% | 已完成 |

---

### Part 1 — 数据背景与变量 ✅

- [x] 数据集介绍
- [x] 变量描述
- [x] 研究背景（线性回归适用性）
- [x] 数据质量考量（缺失值、异常值、数据清洗）

---

### Part 2 — EDA 与分析提案 ✅

#### EDA
- [x] `reason`（Feng Qiu）
- [x] `failures`（Ngoc Vy）
- [x] `address`（Keyao Li）

#### 书面章节
- [x] 第 2.1 节 数据集简介
- [x] 第 2.3 节 研究问题（线性回归 + 单因素方差分析）
- [x] 第 2.4 节 分析计划
- [x] 第 2.5 节 潜在挑战
- [x] 附录：包含 Part 1 内容

---

### Part 3 — 最终报告 [~8–12 页] — 截止 2026年4月10日

#### 内容任务

- [x] **执行摘要** — 三个预测变量（`reason`、`failures`、`address`）均已涵盖 ✅
- [x] 引言与背景（精修版 Part 1）← Feng ✅
- [x] 探索性数据分析
  - [x] `reason` EDA ← Feng ✅
  - [x] `failures` EDA ← Vy ✅
  - [x] `address` EDA ← Keyao ✅
- [x] 研究方法
  - [x] 研究方法概述与统计框架 ← Vy ✅
  - [x] SLR：G3 ~ `reason`（方程、F检验、t检验、95%置信区间）← Feng ✅
  - [x] SLR：G3 ~ `failures`（方程、F检验、t检验）← Vy ✅
  - [x] SLR：G3 ~ `address`（方程、F检验、95%置信区间）← Keyao ✅
  - [x] 说明并验证线性回归假设 ← Feng ✅
- [x] 结果
  - [x] 单因素 ANOVA：G3 按 `reason` 分组（F统计、Levene检验、Tukey HSD）← Feng ✅
  - [x] 单因素 ANOVA：G3 按 `failures` 分组（F统计、Tukey HSD）← Vy ✅
  - [x] 两样本 t 检验：G3 按 `address` 分组 ← Keyao ✅
  - [x] `reason` 模型诊断图（残差图、Scale-Location、QQ图）← Feng ✅
  - [x] `failures` 模型诊断图 ← Vy ✅
  - [x] G3 = 0 样本处理——已排除并记录理由 ← Feng ✅
- [x] 讨论
  - [x] `reason` 结果已讨论 ← Feng ✅
  - [x] `address` 结果已讨论 ← Keyao ✅
  - [x] `failures` 结果已讨论 ← Vy ✅
  - [x] 模型假设验证 ← Feng ✅
  - [x] 局限性已记录 ← Feng ✅
- [x] **结论** — 已新增第 5 章（5.1 核心发现、5.2 实践启示、5.3 未来研究）✅

#### 格式 / 合规修复

- [x] **执行摘要** — 三个预测变量均已补充 ✅
- [x] **结论章节** — `## 5. Conclusion` 已添加 ✅
- [x] **封面组号** — 已添加（第 6 组）✅
- [x] **代码已隐藏 / 附录已添加** — YAML 已设置全局 `execute: echo: false`；全部 44 个代码块均已添加标签；已在文末新增 `\newpage` + `# Appendix: Full R Code` 章节，通过 `ref-label: !expr knitr::all_labels()` 统一收录所有代码 ✅
- [x] **Part 1 节编号问题** — 第 1.5、1.6、1.7 节已重编为 1.4.1、1.4.2、1.4.3；第 1.4.3 节中的交叉引用已同步更新 ✅

---

### 展示报告 ✅ — 已完成（2026年4月3日）

## EDA 主要发现

### `reason` — 选校原因
| 选校原因 | n | 平均期末成绩 | 标准差 |
|--------|---|------------|------|
| reputation（口碑） | 143 | 12.94 | 3.05 |
| home（距离） | 149 | 12.18 | 2.95 |
| course（课程） | 285 | 11.55 | 3.11 |
| other（其他） | 72 | 10.69 | 3.93 |

以口碑为选校理由的学生期末平均成绩最高，"其他"组的成绩波动最大。SLR：F(3, 630) = 10.5，p ≈ 0，R² = 4.8%。Tukey HSD：仅 reputation vs. course 和 reputation vs. other 两组差异显著。

### `failures` — 历史不及格次数
| 不及格次数 | n | 平均期末成绩 |
|---------|---|------------|
| 0 | 549 | 12.51 |
| 1 | 70 | 8.64 |
| 2 | 16 | 8.81 |
| 3 | 14 | 8.07 |

一次不及格即与期末成绩下降约4分相关，且该影响在1–3次不及格之间并不呈累积效应。

### `address` — 居住地址类型
| 地址类型 | n | 平均期末成绩 |
|--------|---|------------|
| 城市（U） | 452 | 12.3 |
| 农村（R） | 197 | 11.1 |

城市学生平均成绩比农村学生高约1.2分。两组均有零分记录（城市11例，农村4例）。城市学生的中位数更高，四分位距更集中。

## 仓库结构

```
5240-project/
├── README.md                        # 项目文档（英文）
├── README.zh.md                     # 项目文档（中文）
├── README.vi.md                     # 项目文档（越南文）
├── 5240H Project.qmd                # Quarto 分析主文档
├── 5240H-Project.pdf                # 渲染后的报告
├── student-por.csv                  # 数据集（葡萄牙语课程）
├── references.bib                   # 参考文献
├── apa.csl                          # APA 引用格式
├── presentation/                    # 演示文稿相关文件
│   ├── Is Your GPA Your Fault?.key  # Keynote 幻灯片
│   ├── 2015_TrentU PPT Template_FINAL2.potx
│   ├── presentation outline.md      # 幻灯片提纲（英文）
│   ├── presentation outline.zh.md   # 幻灯片提纲（中文）
│   └── presentation outline.vi.md   # 幻灯片提纲（越南文）
└── docs/                            # 参考文档
    ├── 5240-project-part0_overview-wi26.pdf
    ├── 5240-project-part1_background-wi26.pdf
    ├── Standard Operating Procedure_ Variable Screening.pdf
    ├── Project Revised.pdf
    └── How to Merge Main into Your Personal Branch via GitHub Desktop.md
```

## 工具

- **R** — 统计分析
- **Quarto** — 文档渲染
- **ggplot2** / **tidyverse** — 数据可视化与处理

## 许可证

本数据集遵循 [知识共享署名 4.0 国际协议（CC BY 4.0）](https://creativecommons.org/licenses/by/4.0/)。

## 参考文献

Cortez, P., & Silva, A. (2008). Using data mining to predict secondary school student performance. In *Proceedings of 5th Annual Future Business Technology Conference* (pp. 5-12). EUROSIS.

UCI Machine Learning Repository. (2014). Student Performance Dataset. https://archive.ics.uci.edu/dataset/320/student+performance

OECD. (2012). *Equity and quality in education: Supporting disadvantaged students and schools*. OECD Publishing.
