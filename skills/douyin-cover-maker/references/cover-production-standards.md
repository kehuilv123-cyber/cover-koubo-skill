# Cover Production Standards

## Core Interpretation

Treat the user's standards as six production requirements. The first five control production quality; the sixth, "strengthen audience impression," is the final communication outcome.

Every cover must pass these standards before it is considered publishable. The default workflow is real-shoot-photo-first: use a photo from the corresponding video shoot as the base image or creator reference, then use the built-in image-generation tool to improve the cover and render the exact Chinese title/subtitle in the initial result. Use a targeted follow-up edit only when one clear defect needs correction. Manual Chinese text overlay remains the backup when generated text is inaccurate.

## 0. Matching Shoot Photo

The cover should come from the same video, not from a generic portrait library, unless the user explicitly asks for a different style.

Source photo priority:

1. A clear close-up or half-body photo from the actual shoot.
2. A frame grab from the video if it is sharp, bright, and expressive.
3. A wider scene photo from the actual shoot when the location is important.
4. A newly requested cover photo if no usable shoot photo exists.

The image-generation tool should preserve the creator's real face, outfit, body shape, and the actual scene. Use it to improve lighting, crop, background cleanliness, visual hierarchy, and title-safe blank space. Do not let it invent a different person, unrelated school, fake message content, or a scene that was not part of the video.

## 1. Complete Cover Theme

A complete cover theme means the viewer can understand the video's promise without reading the caption.

The cover should answer four questions at a glance:

- Who is in the video?
- Where or in what scene is it happening?
- What is the topic?
- Why should the viewer click?

For this user's account:

- Knowledge/education: show the creator plus a learning, AI, study, or university-application signal.
- Campus: show the creator plus a recognizable campus scene.
- Travel: show the creator plus a place, route, or travel mood.

Avoid:

- A beautiful but vague portrait.
- A scenic image with no creator identity.
- A title that does not match the visual scene.
- A generated scene that has nothing to do with the actual video.

## 2. Clear And Bright Base Image

The base image must be bright, clean, and strong enough to hold text.

Requirements:

- Face or person silhouette is sharp.
- Background is not muddy, overly dark, or noisy.
- Main light direction is clear.
- Text area has enough clean space.
- Important subject is not blocked by clutter.
- The selected source photo is from the corresponding video shoot or is clearly requested as a reshoot/reference image.

Practical default:

- Prefer natural daylight, window light, bright campus scenes, or clean desk lighting.
- For night travel covers, keep the person and title area brighter than the background.
- If the source photo is weak, ask for or recommend a quick reshoot before designing.

Avoid:

- Underexposed screenshots.
- Busy backgrounds behind text.
- Heavy filters that reduce face clarity.
- Low-resolution frames unless there is no alternative.

## 3. Strong Personal Expression

The cover must let the user feel like a real creator, not a stock-image model.

Strong personal expression can come from:

- Eye contact.
- A natural confident smile.
- A surprised or thoughtful expression that matches the topic.
- A walking/back-view pose with strong scene emotion.
- A hand gesture that points to the result or topic.

By content type:

- Knowledge/education: confident, useful, "I can teach you this."
- Campus: relaxed, youthful, authentic.
- Travel: curious, reflective, free, or moved by the place.

Avoid:

- Blank face.
- Stiff ID-photo posture.
- Excessively exaggerated expressions.
- A pose that looks unrelated to the video emotion.
- AI changes that make the creator no longer look like themselves.

## 4. Concise And Clear Copy

The cover copy must be short enough to read while scrolling. Include the exact Chinese main title/subtitle, placement, and hierarchy in the initial generation prompt. If the generated text is inaccurate, make one targeted correction that preserves the creator, scene, crop, and layout. Also provide a manual overlay backup.

Rules:

- Main title: 6-12 Chinese characters preferred.
- Maximum: 2 lines for the main title.
- Subtitle: optional, smaller, and only for added context.
- Highlight only 1-2 key words.
- Use specific results, scenes, or emotions instead of abstract claims.

Good copy should be:

- Clear: viewer understands instantly.
- Concrete: includes a result, scene, or conflict.
- Honest: matches the video.
- Memorable: easy to repeat or recognize.

Avoid:

- Long sentence titles.
- Too many selling points.
- Generic words like "超实用" without context.
- Titles that require reading the caption to understand.
- Overpromises that damage trust.

## 5. Ordered Layout Hierarchy

The layout must make the viewer's eye move in the right order.

Default hierarchy:

1. Person or strongest scene.
2. Main title.
3. Supporting scene/detail.
4. Subtitle or small label if needed.

Rules:

- Do not place large text over the face.
- Keep main title in the cleanest area.
- Use contrast between text and background.
- Use one visual center; do not make everything equally loud.
- Keep enough edge margin for platform cropping.

For 3:4:

- Best for portrait/person-first covers.
- Put person on one side and title on the other, or use top title plus lower portrait.

For 4:3:

- Best for wider scenes, campus/travel environment, desktop setups, or before/after comparisons.
- Keep title in a clean block; do not spread text across the whole image.

## 6. Strengthen Audience Impression

The cover should help viewers remember the creator, not just click once.

Strengthen impression through:

- Repeated personal face or recognizable figure.
- Consistent title style and color logic.
- Recurring account symbols: campus, desk, suitcase, laptop, notebook, route map.
- A clear series feeling: similar title rhythm or layout across related videos.

For this account, prioritize:

- Creator identity: real person appears often.
- Content identity: knowledge, campus, travel are visually distinguishable.
- Emotional identity: sincere, useful, youthful, and exploratory.

Avoid:

- Covers that look like unrelated accounts.
- Random style changes that break recognition.
- Designs that are high-click but damage trust.

## Ratio Standard

Generate covers in either 3:4 or 4:3 unless the user explicitly asks otherwise.

Default choice:

- Use 3:4 for Douyin portrait-first covers, creator close-ups, campus daily covers, and knowledge covers.
- Use 4:3 for wider campus scenes, travel scenery, desktop/tutorial scenes, and comparison-style covers.

Always state the chosen ratio and why.

Do not default to 9:16 for covers unless requested; 9:16 may be useful for full-screen visuals, but this workflow standard is 3:4 or 4:3.

## Mandatory Output Fields

For each cover concept, include:

```text
Cover direction:
Ratio: 3:4 / 4:3, with reason
Source photo recommendation:
Complete theme:
Base image plan:
Personal appeal:
Main title:
Subtitle:
Text overlay plan:
Initial generation/edit prompt (internal unless requested):
Targeted correction prompt (only if needed; internal unless requested):
Manual text overlay backup:
Layout hierarchy:
Audience memory cue:
Negative prompt:
QA conclusion:
```
