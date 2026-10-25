# Soft Actor-Critic（ICML 2018）阅读提示

- 原文：[PMLR](https://proceedings.mlr.press/v80/haarnoja18b.html)。
- 核心问题：连续控制中，怎样兼顾交互样本效率与训练稳定性？
- 方法：Actor-Critic、离策略经验回放、最大熵目标与随机策略。
- 阅读顺序：第 3 节目标定义 -> 第 4 节推导与更新 -> 算法 1 -> 第 5 节实验。
- 实验抓手：图 1 的横轴是环境交互步数，比较学习速度、最终回报和不同随机种子下的变化；主对比曲线不能单独证明某个模块的因果作用。
- 课程联系：小车线速度、角速度和关节力矩都是连续动作；将课程场景作为应用分析，与论文实际完成的仿真基准区分。
- 个人理解：讨论熵项如何影响探索、旧数据如何复用，以及训练时的随机策略与评估时采用均值动作的区别。
- 版本：此处收录 ICML 2018 原始 SAC，包含独立的 V 网络；勿把后续自动温度调节机制写成本文的方法。
- 报告方式：使用原文实验图表开展文献分析，无需自行训练或复现实验。

## 来源与译文

Haarnoja, T., Zhou, A., Abbeel, P. & Levine, S. (2018). Soft Actor-Critic: Off-Policy Maximum Entropy Deep Reinforcement Learning with a Stochastic Actor. PMLR 80:1861-1870.

中文文件由当前对话模型翻译，并通过无需额外 API 的 paper-translate-agent-skill 在本地嵌字排版，原作者及原出版信息保留。PMLR 出版协议采用 CC BY 4.0，参见 https://proceedings.mlr.press/pmlr-license-agreement.pdf 与 https://creativecommons.org/licenses/by/4.0/ 。
