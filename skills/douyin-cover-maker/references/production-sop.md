# Production SOP

## Standard Flow

Use this flow for each video:

1. Inspiration input.
2. Topic positioning.
3. Two-second retention opening design.
4. Script writing.
5. Scene planning.
6. Filming guidance.
7. User shoots video and captures cover-photo options.
8. User returns final video summary, usable shoot photos, and screenshots.
9. Cover concept generation from the corresponding video's real shoot photo.
10. Initial image-generation prompt with the exact Chinese title/subtitle, plus a targeted correction prompt only when needed and a manual overlay backup.
11. Cover image QA.
12. Publish video.
13. Collect 24-hour data feedback.
14. Decide the next iteration.

## Idea Intake Template

If the user gives only an idea, infer missing details and proceed.

Ask only when necessary:

```text
视频灵感：
视频类型：知识干货 / 校园记录 / 旅行 Vlog
拍摄地点：
是否真人出镜：
预计时长：
观众看完要获得什么：
```

## Topic Positioning Output

```text
视频类型：
目标观众：
核心观点：
观众收益：
推荐时长：
推荐标题：
封面点击理由：
```

## Script Structure

Use a short-video rhythm:

1. First 2 seconds: make the viewer quickly feel interested, able to understand, emotionally related, willing to keep watching, and aware of value.
2. Opening hook: direct question, direct conclusion, highlight moment, conflict, rare scene, or user pain point.
3. Scene/person identity: why the creator can talk about this.
4. Main content: no more than 3 points.
5. Personal experience: make it feel human, not generic.
6. Closing CTA: follow, comment, save, or next episode.

Before drafting a script, read `two-second-retention-script-standards.md` and output a first-2-second plan. Do not start with slow greetings such as "大家好，我是...", "今天给大家分享一个...", or "最近很多朋友问我...".

## Script Output Template

```text
选题价值判断：需求型 / 共鸣型 / 稀缺型 / 热点型
前 2 秒目标：感兴趣 / 看得懂 / 有共鸣 / 想继续看 / 觉得有价值
第一帧画面：
第一句话：
核心字幕：
声音/BGM/音效：
A/B/C 开头测试：
完整口播文案：
拍摄提示：
发布前两秒跳出率检查：
```

## Scene Planning Defaults

Knowledge/education:

- Desk, computer, library, classroom, self-study room.
- Props: laptop, notebook, phone, pen, backpack.
- Camera: half-body talking head plus close-up of notes or screen.

Campus records:

- Campus road, classroom, library, canteen, dorm building, playground.
- Camera: walking shot, side profile, over-shoulder, environmental details.

Travel Vlog:

- Station, street, landmark, cafe, scenic spot, hotel window.
- Camera: walking shot, back view, route details, local texture, reaction shot.

## Minimum Shot List

For every video, ask the user to capture:

- 1 clean A-roll talking-head clip.
- 3 environmental B-roll clips.
- 2 action clips.
- 3-5 cover-photo options from the same shoot with clear title space.

Cover-photo reminders:

- Shoot one close-up portrait.
- Shoot one half-body image with empty space on one side.
- Shoot one wider scene image showing the location.
- Shoot one expression/gesture that matches the video's strongest opinion or result.
- Keep the outfit and scene consistent with the video so the cover feels like the same content.
- Keep face and title area unobstructed.
- Avoid busy backgrounds behind text.
- If using chat screenshots, blur or block private information and treat them as background elements, not the main face/identity image.

## Cover Photo Capture Directions

When a video will need an image-generated cover, give the user exact cover-photo directions before shooting:

```text
封面照 1：近景人像，表情/动作，标题留白位置
封面照 2：半身人像，表情/动作，标题留白位置
封面照 3：场景图，人物站位，标题留白位置
可用道具：
避免：
```

The goal is to make the image-generation tool polish a real photo, not invent a new cover from nothing.

## Post-Shoot Return Template

```text
视频类型：
最终标题：
视频内容概要：
最有冲击力的一句话：
出镜画面描述：
可用截图/照片描述：
可用封面照片：近景 / 半身 / 场景 / 动作 / 视频截图
希望封面突出：人物IP / 结果利益 / 情绪冲突 / 场景氛围 / 系列感
封面文字倾向：
视频整体感觉：
希望观众点击的理由：
```

## Post-Publish 24-Hour Feedback Template

Collect these metrics 24 hours after publishing:

```text
视频标题：
发布时间：
视频类型：知识干货 / 校园记录 / 旅行 Vlog
开头版本：A 痛点 / B 悬念 / C 结果 / 其他
封面方向：稳定款 / 点击款 / IP 款 / 氛围款 / 结果对比款
视频时长：
播放量：
点赞数：
评论数：
转发数：
收藏数：
新增关注数：
完播率：
平均播放时长：
两秒跳出率：
主页访问数（如有）：
你自己的观察：
```

When reviewing 24-hour data, read `post-publish-24h-feedback-standards.md` and return:

```text
数据总评：
核心问题判断：
四层诊断：播放分发 / 停留完播 / 互动反馈 / 关注转化
下一条视频要保留什么：
下一条视频要修改什么：
可复用模板：
下一轮测试建议：
```
