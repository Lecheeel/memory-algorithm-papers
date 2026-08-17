# 记忆算法论文与资料合集

关于**记忆算法（间隔重复 / Spaced Repetition）**的论文与资料整理合集，涵盖从经典记忆心理学研究到现代机器学习记忆调度模型。

内容主要来自个人学习整理，包含四类资源：

- **经典文献**：间隔效应、测试效应等记忆心理学的奠基性研究
- **补充论文**：认知模型、知识追踪、遗忘曲线拟合等延伸研究
- **官方解读**：墨墨背单词官方对记忆算法的解读文档
- **代码仓库**：相关算法的开源实现

---

## 目录结构

```
记忆算法论文/
├── 经典文献/          # 间隔重复与测试效应的经典研究
├── 补充论文/          # 认知模型与记忆调度的延伸论文
├── 官方解读/          # 墨墨背单词官方解读（HTML）
├── 代码仓库/          # 开源实现（git submodule）
├── 1885_艾宾浩斯_论记忆_德文原版.pdf
├── 1913_艾宾浩斯_论记忆_英译本.pdf
├── ACL2016_HLR_Duolingo半衰期回归.pdf
└── 2024_DRL-SRS_深度强化学习间隔重复.pdf
```

---

## 经典文献

记忆心理学中关于**间隔效应（spacing effect）**与**测试效应（testing effect）**的代表性研究：

- `1993_Bahrick_永久记忆的间隔保持.pdf` — Bahrick 等，外语词汇长期保持与间隔效应
- `2002_Leeming_课程间隔复习效果.pdf` — Leeming，课程中分散复习的效果
- `2005_Carpenter_测试效应_提取练习.pdf` — Carpenter & DeLosh，提取练习对记忆的促进
- `2007_Karpicke_提取练习增强记忆.pdf` — Karpicke & Roediger，重复提取促进长期保持
- `2007_Rohrer_间隔与测试效应综述.pdf` — Rohrer & Pashler，间隔与测试效应综述
- `2008_Kornell_间隔与归纳学习_EnemyOfInduction.pdf` — Kornell & Bjork，间隔与归纳学习
- `2009_Kerfoot_医学教育间隔重复.pdf` — Kerfoot，医学教育中的间隔重复
- `2012_McDaniel_测试增强学习.pdf` — McDaniel 等，测试增强学习
- `2013_Dunlosky_高效学习技术评估.pdf` — Dunlosky 等，十种学习技术有效性评估
- `2014_Mulligan_间隔效应与元认知控制.pdf` — Mulligan & Peterson，间隔效应与元认知
- `2018_Bisra_诱导学习效果.pdf` — Bisra 等，自我解释等诱导学习策略
- `2021_Yan_测试效应与间隔效应综述.pdf` — Yan 等，测试效应与间隔效应综述

## 补充论文

从认知建模到机器学习记忆调度的延伸研究：

- `1991_ACT-R_记忆环境反射_Anderson_Schooler.pdf` — Anderson & Schooler，环境统计结构中的记忆反射
- `2006_测试效应_TestEnhancedLearning.pdf` — Roediger & Karpicke，测试增强学习
- `2006_分散练习元分析_Cepeda.pdf` — Cepeda 等，分散练习的元分析
- `2009_记忆模型比较_PavlikAnderson_vs_MCM.pdf` — 记忆模型比较（Pavlik/Anderson 模型 vs MCM）
- `2009_MCM_多尺度上下文模型.pdf` — MCM 多尺度上下文模型
- `2015_DeepKnowledgeTracing.pdf` — Piech 等，深度知识追踪（DKT）
- `2016_UnboundedHumanLearning_最优调度.pdf` — Reddy 等，无界人类学习的最优调度
- `2017_OptimizingHumanLearning.pdf` — Tabibian 等，人类学习的最优调度
- `2018_Duolingo_SLAM_二语习得建模.pdf` — Settles 等，二语习得与遗忘建模
- `2019_遗忘幂律_回溯干扰模型.pdf` — 遗忘幂律与回溯干扰模型
- `2019_DAS3H_学生遗忘建模.pdf` — Choffin 等，DAS3H 学生遗忘建模
- `2020_Duolingo_AdaptiveForgettingCurves.pdf` — 自适应遗忘曲线
- `SuperMemo_优化学习_论文简介.html` — SuperMemo 优化学习论文简介
- `SuperMemo_SM-2算法详解.html` — SuperMemo SM-2 算法详解
- `SuperMemo_SM-17算法详解.html` — SuperMemo SM-17 算法详解

## 代码仓库（git submodule）

相关算法的开源实现：

| 目录 | 上游仓库 | 说明 |
| --- | --- | --- |
| `代码仓库/fsrs4anki` | [open-spaced-repetition/fsrs4anki](https://github.com/open-spaced-repetition/fsrs4anki) | FSRS（Free Spaced Repetition Scheduler）Anki 版实现 |
| `代码仓库/halflife-regression` | [duolingo/halflife-regression](https://github.com/duolingo/halflife-regression) | Duolingo 半衰期回归（HLR，ACL 2016）实现 |
| `代码仓库/SSP-MMC` | [maimemo/SSP-MMC](https://github.com/maimemo/SSP-MMC) | 墨墨记忆算法（KDD 2022） |
| `代码仓库/SSP-MMC-Plus` | [maimemo/SSP-MMC-Plus](https://github.com/maimemo/SSP-MMC-Plus) | SSP-MMC 改进版（TKDE 2023） |

---

## 克隆方式

由于代码仓库以 submodule 形式引用，克隆时需一并拉取子模块：

```bash
# 方式一：克隆时递归拉取子模块
git clone --recurse-submodules https://github.com/Lecheeel/memory-algorithm-papers.git

# 方式二：先克隆，再单独初始化子模块
git clone https://github.com/Lecheeel/memory-algorithm-papers.git
cd memory-algorithm-papers
git submodule update --init --recursive
```

若只想更新子模块到上游最新提交：

```bash
git submodule update --remote
```

---

## 版权说明

本仓库为个人学习整理的资料合集：

- 论文 PDF 与官方解读的版权归原作者、期刊及发布方所有，仅供个人学习与研究使用，请勿用于商业用途。
- 各代码仓库保留其原始仓库的许可证（详见各自目录内的 `LICENSE` 文件）。
- 如涉及版权问题，请联系删除。
