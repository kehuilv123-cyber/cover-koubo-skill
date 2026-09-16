# cover-koubo-skill

**从口播创意到发布复盘的短视频创作工具包。** 作者：吕柯辉。

把灵感变成能拍摄的脚本，优化前两秒与正文节奏，制作封面，再根据真实数据确定下一条改什么。

## 实践成绩

2026 年 7 月 19 日整理的账号记录：一个月发布 **7 条视频，4 条破万，3 条达到 10 万级，单条最高 19 万播放**。四条破万作品页面显示播放量合计 **43.8 万**。

| 代表作品 | 页面播放量 |
| --- | ---: |
| 湖南考生问爆的楚怡工匠计划 | 10.5 万 |
| 谁配好生 / Zero to One | 11.3 万 |
| 线上兼职时薪 40？我成了背词软件 | 3.0 万 |
| 比亚迪工厂见习后，我对智能制造祛魅了 | 19.0 万 |

这些创作与复盘案例沉淀为本工具包。数字来自当时的账号主页截图整理，属于历史页面显示值；尚无同口径使用前后对照，不能据此量化 Skill 带来的播放增长。详见 [案例数据](docs/results.md)。

## 四个独立入口

| Skill | 解决的问题 | 交付 |
| --- | --- | --- |
| [cover-koubo-skill](skills/cover-koubo-skill/SKILL.md) | 完整口播创作闭环 | 选题、口播、拍摄方案、复盘与下一条迭代 |
| [cover-skill](skills/cover-skill/SKILL.md) | 封面表达与手机端可读性 | 封面文案、成图或制作方案、质检 |
| [two-second-retention-skill](skills/two-second-retention-skill/SKILL.md) | 前两秒能否留住人 | 第一帧、第一句话、字幕、开头备选 |
| [completion-rate-skill](skills/completion-rate-skill/SKILL.md) | 正文能否让人看完 | 结构诊断、节奏调整、完整改稿、复查指标 |

主入口自带完整参考标准；三个专项 Skill 都可以单独安装。

## 安装与使用

```bash
git clone https://github.com/kehuilv123-cyber/cover-koubo-skill.git
```

从 `skills/` 中选择需要的文件夹，复制到客户端 Skill 目录。Codex 通常为 `$CODEX_HOME/skills` 或 `~/.codex/skills`，安装后刷新客户端。

```text
使用 $cover-koubo-skill，把这段真实经历整理成 60 秒口播、拍摄清单和复盘计划。
使用 $two-second-retention-skill，为这段口播设计三个开头，并说明各自的判断依据。
使用 $completion-rate-skill，检查这份口播哪些段落可以前移或删减，给出完整改稿。
使用 $cover-skill，根据本期口播和实拍照片制作封面。
```

口播与复盘可以只用文字材料；生成封面图片需要客户端有图像工具。发布、剪辑与后台数据读取不自动执行。更名后的主入口为 `cover-koubo-skill`，旧版 `douyin-cover-maker` 可自行备份后停用。

## 许可

MIT · 吕柯辉。创作流程与规则在 AI 协作中整理；使用者需自行拥有上传照片、字体与其他素材的使用权。
