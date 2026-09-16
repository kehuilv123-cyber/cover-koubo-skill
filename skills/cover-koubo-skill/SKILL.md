---
name: cover-koubo-skill
description: 把短视频灵感推进为选题、口播、拍摄、封面和发布后数据复盘。适用于完整口播制作与跨环节迭代。
---

# 口播内容生产与复盘闭环

先判断当前阶段，只完成当前请求需要的环节。完整制片时沿用：灵感 → 选题 → 前两秒 → 口播 → 拍摄 → 封面 → 24 小时数据 → 下一条迭代。

## 选题、口播与拍摄

读取 `references/account-positioning.md` 和 `references/production-sop.md`。根据真实材料输出受众、核心承诺、标题、完整可拍摄口播、A-roll/B-roll 和拍摄提醒。观点、经历、数据均以用户材料为准；不补造成绩。

## 各环节

| 环节 | 独立 Skill | 主包内可直接使用的标准 |
| --- | --- | --- |
| 封面 | cover-skill | `references/cover-production-standards.md`、`references/cover-quality-checklist.md` |
| 前两秒 | two-second-retention-skill | `references/two-second-retention-script-standards.md` |
| 中段节奏与完播 | completion-rate-skill | `references/completion-rate-standards.md` |
| 发布后复盘 | 当前主入口 | `references/post-publish-24h-feedback-standards.md` |

安装了对应子 Skill 时可调用；没有安装时读取主包内标准即可，不要求额外插件或子 Agent。

## 24 小时复盘

按播放分发、停留完播、互动、关注转化四层整理数据。只计算分母已知且大于零的指标，未知不填零。比较同账号、相近题材和时长、相同观察窗口的数据；早期诊断规则视为假设，不视为平台推荐机制的确定解释。

给出一个优先修改点、可直接执行的下一条方案以及复查指标。没有对照数据时陈述实际表现，不声称某个 Skill 导致了增长。真实发布由用户执行。
