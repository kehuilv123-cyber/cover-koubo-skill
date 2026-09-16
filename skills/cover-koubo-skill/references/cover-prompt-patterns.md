# Cover Prompt Patterns

## Tool Target

Write prompts for the built-in image-generation cover workflow. Default to a real-shoot-photo-first workflow: use a photo captured for the corresponding video as the base image or creator reference, improve cover readiness, and render the exact Chinese title/subtitle in the initial result. Use a targeted follow-up edit only when one clear defect needs correction.

Do not rely on the image model to solve the cover strategy by itself. The prompt must already specify source photo use, theme, base image clarity, creator expression, copy-safe area, hierarchy, memory cue, and ratio.

## Real Shoot Photo First Rule

When designing covers, always start from the current video's actual photos when available:

1. Choose the best matching photo from the shoot: close-up portrait, half-body with blank space, action shot, or wider scene.
2. Preserve the creator's real face, hairstyle, body shape, outfit, and the video's actual scene as much as possible.
3. Use the built-in image-generation tool to polish the photo for cover use: cleaner lighting, sharper subject, simpler background, stronger title-safe space, and more ordered visual hierarchy.
4. Generate one initial prompt by default that creates the polished cover and renders the exact Chinese main title/subtitle with typography, position, hierarchy, and safe margins.
5. Prepare a targeted correction prompt only when one clear defect is visible, and keep a manual text overlay backup because generated Chinese text may need correction.
6. If no shoot photo is provided, output a "photo to capture" instruction before the image-generation prompts.

## Prompt Formula

Use this formula:

```text
[ratio: 3:4 or 4:3], Douyin short-video cover, use the uploaded/current-video shoot photo as the base image or creator reference, [content type], [complete theme: person + scene + topic + click reason], preserve the creator's real appearance and outfit, [pose/expression with emotional appeal], [clear bright base image], [scene/background], main title "[exact Chinese main title]", subtitle "[exact Chinese subtitle or none]", [copy placement and hierarchy], [lighting/color], [memory cue for personal IP], high-quality realistic photography, clear visual hierarchy
```

For final covers, prepare all four internally; expose the full prompts only when the user asks:

1. Source photo recommendation: which provided shoot photo to use, or what photo to capture if missing.
2. Initial generation/edit prompt: redesign/polish the real photo into a final cover and render the exact Chinese main title/subtitle.
3. Targeted correction prompt: only when needed, correct the one visible defect while preserving the creator, scene, crop, and layout.
4. Manual text overlay backup plan: exact Chinese title, subtitle, placement, size hierarchy, highlight words, color, and safe margins.

The initial prompt must include the exact Chinese text in quotes and ask for clean, correct, readable typography. Do not create or expose a second prompt unless a targeted correction is needed or the user explicitly asks for the production prompts.

## Negative Prompt Formula

```text
low quality, blurry face, dim base image, underexposed, distorted hands, fake text, unreadable Chinese characters, cluttered background, cheap stickers, over-filtered skin, exaggerated expression, blocked face, messy layout, no clear theme, weak personal presence, low contrast title area, watermark, logo artifacts, different person, changed outfit, unrelated scene, fake school names, exposed private messages, readable private screenshots
```

## Ratio Selection

Use 3:4 when:

- The cover is person-first.
- The creator's face or half-body is the main memory cue.
- The video is knowledge/education or campus daily content.
- The layout needs a strong portrait plus title block.

Use 4:3 when:

- The scene is equally important as the person.
- The video is travel, campus environment, desktop/tutorial, or before/after comparison.
- The image needs wider spatial context.

Always include the selected ratio in the prompt.

## Initial And Targeted-Correction Prompt Template

Initial generation/edit: final cover with exact Chinese text.

```text
Create a Douyin short-video cover in [3:4 / 4:3] ratio.

Source image: use the uploaded photo from this video's actual shoot as the base image. Preserve the creator's real face, hairstyle, body shape, outfit, and the authentic scene. Do not replace the creator with a different person.
Theme: [complete theme: person + scene + topic + click reason].
Person: real young personal creator, [face/half-body/back-view/side-profile], [specific expression or pose], strong personal presence and emotional appeal.
Scene: [campus / desk / classroom / library / travel city / landmark], clear and relevant to the video topic.
Base image: bright, clean, sharp, high-resolution, natural light, face and subject clearly visible.
Composition: leave a clean title area at [left/right/top/bottom], keep the face unobstructed, arrange person, title area, and background in clear hierarchy.
Copy: render the main title "[exact Chinese main title]" and subtitle "[exact Chinese subtitle, or omit if none]" in the reserved title area. Use clean, high-contrast Chinese typography with strong hierarchy, safe margins, and no extra words or random characters.
Style: authentic personal short-video IP, youthful, credible, clean, not overly commercial.
Memory cue: make the creator recognizable and reinforce [knowledge/campus/travel] identity.

Avoid: low quality, blurry face, dim image, cluttered background, cheap stickers, over-filtered skin, exaggerated fake expression, unreadable Chinese text, blocked face, messy layout, watermark, changing the creator into a different person, fake school names, exposed private messages.
```

Targeted correction, only when the initial result has one clear text defect:

```text
Use the initial generated image as the source image. Keep the creator's face, outfit, body shape, background, lighting, crop, and composition unchanged.

Add clean, high-contrast Douyin cover typography in the reserved title area only.
Main title: "[exact Chinese main title]"
Subtitle: "[exact Chinese subtitle, or omit if none]"
Text placement: [left/right/top/bottom], do not cover the face or important scene details.
Typography: bold, highly readable Chinese font style, strong hierarchy, main title largest, subtitle smaller, highlight only [1-2 keywords] with [highlight color].
Layout: keep safe margins from all edges, no clutter, no extra stickers, no extra words, no random characters.
Quality requirement: Chinese text must be exactly correct, sharp, readable at phone-feed size, and match the clean personal short-video cover style.
```

## Knowledge/Education Prompt

Use when the video is about learning methods, AI tools, study efficiency, personal growth, education viewpoints, or college application guidance.

```text
Create a Douyin short-video cover in 3:4 ratio. Use the uploaded current-video shoot photo as the base image or creator reference. Preserve the creator's real face, hairstyle, outfit, and authentic study/desk/campus scene. Theme: a real young university creator explains useful education advice, learning methods, AI tools, or college application guidance, with a clear reason to click. Person: half-body portrait or close portrait from the shoot, natural confident expression, slight smile or focused teaching gesture, strong personal presence. Scene: clean desk, laptop and notebook, library, classroom, or study-room background. Base image: bright, clear, sharp, natural light. Composition: leave a clean title area on one side, keep face unobstructed, person first and title second. Copy: render the exact Chinese main title/subtitle in the title area with readable hierarchy and no extra text. Style: clean, credible education creator, youthful but professional. Memory cue: reinforce the creator as a helpful knowledge-sharing student.
```

## Campus Prompt

Use when the video is about campus daily life, classroom, library, social observation, dormitory, or campus routine.

```text
Create a Douyin short-video cover in 3:4 ratio. Use the uploaded current-video shoot photo as the base image or creator reference. Preserve the creator's real face or recognizable figure, outfit, and actual campus scene. Theme: a real young student creator records an authentic university campus moment, with a clear campus-life hook. Person: natural campus pose, walking, looking back, or relaxed half-body portrait from the shoot, youthful and relatable expression. Scene: campus road, library, classroom, trees, or teaching building visible. Base image: bright, clean, fresh natural light, clear face or personal figure. Composition: leave a clean title area, keep campus identity visible, person and title have clear hierarchy. Copy: render the exact Chinese main title/subtitle in the title area with readable hierarchy and no extra text. Style: authentic documentary campus style, warm and relatable. Memory cue: reinforce the creator as a real campus-life storyteller.
```

## Travel Vlog Prompt

Use when the video is about city exploration, travel route, weekend trip, personal reflection, or scenery.

```text
Create a Douyin short-video cover in 4:3 ratio. Use the uploaded current-video shoot photo as the base image or creator reference. Preserve the creator's real figure, outfit, travel item, and actual location texture. Theme: a real young creator explores a city or travel destination, with a strong place-based reason to click. Person: backpack, side profile, back view, or looking-back pose from the shoot, emotional and story-driven. Scene: city street, station, landmark, sunset, or local texture clearly visible. Base image: bright enough for cover use, sharp subject, clean title-safe area. Composition: person and location both visible, title area placed on the cleanest side, strong foreground-background hierarchy. Copy: render the exact Chinese main title/subtitle in the title area with readable hierarchy and no extra text. Style: atmospheric but realistic travel photography, cinematic natural light. Memory cue: reinforce the creator as a youthful travel-and-growth storyteller.
```

## Targeted Correction Prompt Standard

Use a targeted correction prompt only when the initial result contains a clear title defect:

- Main title: exact Chinese text, preferably 6-12 Chinese characters, no more than 2 lines.
- Subtitle: optional, smaller, used only for context.
- Placement: top/left/right/bottom area, with face and important scene unobstructed.
- Hierarchy: main title largest, subtitle smaller, label or keyword smallest.
- Highlight: emphasize only 1-2 keywords using blue, yellow, white, or black contrast.
- Safe margin: keep text away from platform crop edges.
- Accuracy: ask the model to render the Chinese text exactly as provided, with no extra characters, no misspellings, and no random decorative text.
- Preservation: ask the model to keep the initial image unchanged except for the title typography.

## Manual Text Overlay Backup Standard

Always prepare a manual overlay backup plan for cases where generated text remains inaccurate:

- Main title: exact Chinese text.
- Subtitle: exact Chinese text or "none".
- Placement: same as the intended generated layout.
- Hierarchy: main title largest, subtitle smaller, highlight words listed separately.
- Color and contrast: specify text color, highlight color, shadow/stroke if needed.
- Safe margin: keep text away from platform crop edges.
- Tool note: add text in Jianying, Xingtu, Canva, or another editor when Chinese accuracy matters.

## Cover Concept Output Template

```text
Cover direction:
Why it fits:
Ratio:
Source photo recommendation:
Complete theme:
Main title:
Subtitle:
Person image:
Background scene:
Color direction:
Initial generation/edit prompt:
Targeted correction prompt (only if needed):
Manual text overlay backup:
Negative prompt:
QA reminder:
```
