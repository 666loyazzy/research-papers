# Awesome Robotics & ROS 2 Papers

仓库导航：[总索引（58 篇）](https://github.com/666loyazzy/research-papers/blob/main/PAPERS.md) · [严格边云（20 篇）](https://github.com/666loyazzy/research-papers/blob/edge-cloud-papers/PAPERS.md) · [辅助知识（25 篇）](https://github.com/666loyazzy/research-papers/blob/other-knowledge/PAPERS.md) · [机器人与 ROS 2（13 篇）](https://github.com/666loyazzy/research-papers/blob/robotics-papers/PAPERS.md)。

机器人与 ROS 2 论文选读仓库。当前收录课程“论文选读·第 1 期”的 12 篇论文，以及第 2 期的 SAC，共 **13 篇论文**，覆盖算法实现、ROS 2 架构、传感器、点云、定位建图、路径规划、导航控制和卡尔曼滤波。

每篇论文统一整理：原文 PDF、纯中文嵌字版、中英双语版、BibTeX 引用和阅读提示。

## 分支导航

- [`main`](https://github.com/666loyazzy/research-papers/tree/main) - 总入口，58 篇不重复论文
- [`edge-cloud-papers`](https://github.com/666loyazzy/research-papers/tree/edge-cloud-papers) - 严格边云协同集合，20 篇，含 PipeSD 与 SpecEdge
- [`other-knowledge`](https://github.com/666loyazzy/research-papers/tree/other-knowledge) - 辅助知识，25 篇
- [`robotics-papers`](https://github.com/666loyazzy/research-papers/tree/robotics-papers) - 机器人与 ROS 2，13 篇（当前分支）

## 第 1 期论文清单

| # | 主题 | 论文 | 年份 |
|---:|---|---|---:|
| 1 | 机器人算法与 Python 实现 | PythonRobotics | 2018 |
| 2 | ROS 2 的设计与系统架构 | Robot Operating System 2 | 2022 |
| 3 | 移动机器人传感器综述 | A Review of Sensing Technologies for Indoor Autonomous Mobile Robots | 2024 |
| 4 | 二维激光建图 | SLAM Toolbox | 2021 |
| 5 | 移动机器人路径规划综述 | Path Planning for Autonomous Mobile Robots | 2021 |
| 6 | 点云与三维数据处理 | Open3D | 2018 |
| 7 | Nav2 与行为树 | The Marathon 2 | 2020 |
| 8 | 路径跟踪与速度调节 | Regulated Pure Pursuit | 2023 |
| 9 | 卡尔曼滤波推导 | A Step by Step Mathematical Derivation and Tutorial on Kalman Filters | 2019 |
| 10 | 激光里程计与 ICP | KISS-ICP | 2023 |
| 11 | 视觉 SLAM 系统 | ORB-SLAM2 | 2017 |
| 12 | SLAM 整体知识框架 | Past, Present, and Future of SLAM | 2016 |

## 第 2 期补充论文

| 课程编号 | 主题 | 论文 | 年份 |
|---:|---|---|---:|
| 8 | 最大熵强化学习与连续控制 | [Soft Actor-Critic（SAC）](PAPERS.md#13-最大熵强化学习与连续控制第-2-期第-8-篇) | 2018 |

## 建议阅读路线

无需按编号顺序读。初学路线可按以下顺序：

1. **PythonRobotics**：先用动画建立定位、规划和控制的直觉。
2. **ROS 2 → SLAM Toolbox → Marathon 2**：把节点、话题、QoS、建图和 Nav2 串成系统。
3. **Open3D → KISS-ICP**：理解点云处理和相邻帧配准。
4. **路径规划综述 → Regulated Pure Pursuit**：区分全局规划与局部跟踪。
5. **Kalman Filters → ORB-SLAM2**：补状态估计和视觉 SLAM。
6. **传感器综述 → SLAM 综述**：最后建立完整知识地图。

## 仓库文件

- [`PAPERS.md`](PAPERS.md) - 13 篇论文的完整索引、来源、译文和阅读提示
- [`references.bib`](references.bib) - 可直接用于 Overleaf 的 BibTeX
- [`papers/original/`](papers/original/) - 原文 PDF
- [`papers/translated/`](papers/translated/) - 纯中文嵌字版与中英双语版
- [`papers/README.md`](papers/README.md) - PDF 来源、页数、校验值与翻译状态
- [`notes/`](notes/) - 每篇论文的阅读抓手和先修知识

## 翻译说明

第 1 期的 12 篇译文使用 PDFMathTranslate / `pdf2zh` 和 Google 翻译服务生成。新增 SAC 使用 [paper-translate-agent-skill](https://github.com/AIKONG2024/paper-translate-agent-skill/tree/main/pdf-translate)：由当前对话模型翻译，本地 `pdf2zh` 负责排版，无需另配翻译 API 或密钥。SAC 保留公式与原始矢量图，中文字体已嵌入，完成 10 页逐页检查，详见 [检查记录](papers/SAC_QA_REPORT.md)。

PDF 著作权归原作者及出版机构所有，本仓库仅用于个人学习与学术研究。
