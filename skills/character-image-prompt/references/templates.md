# 可复制填空模板

配合 `SKILL.md` 使用。先贴角色锚点，再选对应模型的模板，只改 `{}` 里的内容。已填示例用虚构角色「盐仔」，可直接试生成。

## 4. 可复制填空模板（每条都标了模型，并附已填示例）

使用方法：先贴【角色锚点】，再选对应模型的模板，只改 `{}` 里的内容。已填示例全部用「盐仔」，可直接试生成。

### 4.1 胸像 / 角色设定卡（bust portrait / character sheet 头图）

用途：立角色的脸、材质和配色。白底或浅底，正面或 3/4 侧，肩膀以上，画面内不要字。

#### 模板 · Midjourney

```text
{英文角色锚点}, bust portrait, shoulders-up, 3/4 view, looking at camera, neutral gentle smile, centered composition, plain off-white background, studio lighting, soft frontlight, subtle rim lighting, product photography, sharp focus, highly readable face, --ar 3:4 --stylize 80 --quality 1 --chaos 0 --v 6 --no text, watermark, logo, extra eyes, extra limbs, realistic human skin, crowded background
```

#### 已填示例 · Midjourney

```text
An original seaside trendy-toy IP mascot named Yanzi: a chubby seagull chick, about 1:2 head-to-body ratio, matte cream vinyl face, salt-white dense plush body with visible short fibres, coral-orange felt beak, huge glossy eyes each with exactly one crisp four-point star highlight. Wearing a mustard-yellow hooded windbreaker, a teal knit scarf with readable weave, and a tiny red-and-white life-ring backpack; a small wave embroidery on the chest. Mitten-like short wings, stubby legs, round highly readable silhouette, minimal facial features. Not a human, not an existing commercial IP. Fixed palette: cream #F6EAD2, salt-white #F8F4E7, coral-orange #E26A4A, mustard #E2B23A, teal #2BAEC6, life-ring red #E0263C, bust portrait, shoulders-up, 3/4 view, looking at camera, neutral gentle smile, centered composition, plain off-white background, studio lighting, soft frontlight, subtle rim lighting, product photography, sharp focus, highly readable face, --ar 3:4 --stylize 80 --quality 1 --chaos 0 --v 6 --no text, watermark, logo, extra eyes, extra limbs, realistic human skin, crowded background
```

#### 模板 · Flux / GPT Image / DALL·E（自然语言）

```text
Create a {画幅，如 3:4} bust portrait character sheet image of {角色锚点}.
Shot: shoulders-up, 3/4 view, looking at camera, calm friendly expression, centered, plenty of clean margin.
Background: plain off-white seamless studio backdrop, no scenery, no props except the character's own costume.
Lighting: soft studio front light plus a warm rim light that separates the plush edges; no harsh shadows on the face.
Material must stay consistent: matte vinyl face, visible plush fibres, readable knit weave.
Style: premium stylized trendy-toy render, highly readable IP look, not photoreal human, not anime cel, not flat vector unless specified.
Do not include any text, watermark, logo, extra eyes, extra limbs, or existing commercial characters.
```

#### 已填示例 · Flux / GPT Image

```text
Create a 3:4 bust portrait character sheet image of an original seaside trendy-toy IP mascot named Yanzi: a chubby seagull chick, about 1:2 head-to-body ratio, matte cream vinyl face, salt-white dense plush body with visible short fibres, coral-orange felt beak, huge glossy eyes each with exactly one crisp four-point star highlight. Wearing a mustard-yellow hooded windbreaker, a teal knit scarf with readable weave, and a tiny red-and-white life-ring backpack; a small wave embroidery on the chest. Mitten-like short wings, stubby legs, round highly readable silhouette, minimal facial features. Not a human, not an existing commercial IP. Fixed palette: cream #F6EAD2, salt-white #F8F4E7, coral-orange #E26A4A, mustard #E2B23A, teal #2BAEC6, life-ring red #E0263C.
Shot: shoulders-up, 3/4 view, looking at camera, calm friendly expression, centered, plenty of clean margin.
Background: plain off-white seamless studio backdrop, no scenery, no props except the character's own costume.
Lighting: soft studio front light plus a warm rim light that separates the plush edges; no harsh shadows on the face.
Material must stay consistent: matte vinyl face, visible plush fibres, readable knit weave.
Style: premium stylized trendy-toy render, highly readable IP look, not photoreal human, not anime cel, not flat vector unless specified.
Do not include any text, watermark, logo, extra eyes, extra limbs, or existing commercial characters.
```

#### 模板 · Stable Diffusion / SDXL

```text
正向：
{英文角色锚点}, bust portrait, shoulders-up, 3/4 view, looking at camera, neutral smile, centered, plain off-white background, studio lighting, soft frontlight, rim lighting, product photography, sharp focus, (highly readable face:1.2), (visible plush fibres:1.1)

Negative prompt:
text, letters, watermark, logo, extra fingers, extra eyes, extra limbs, mutated hands, blurry face, photoreal human skin, messy background, busy pattern, copyright, existing character
```

#### 已填示例 · Stable Diffusion / SDXL

```text
正向：
An original seaside trendy-toy IP mascot named Yanzi, chubby seagull chick, 1:2 head-to-body ratio, matte cream vinyl face, salt-white dense plush body, visible short fibres, coral-orange felt beak, huge glossy eyes, one crisp four-point star highlight in each eye, mustard-yellow hooded windbreaker, teal knit scarf, tiny red-and-white life-ring backpack, wave embroidery on the chest, mitten-like short wings, stubby legs, highly readable silhouette, bust portrait, shoulders-up, 3/4 view, looking at camera, neutral smile, centered, plain off-white background, studio lighting, soft frontlight, rim lighting, product photography, sharp focus, (highly readable face:1.2), (visible plush fibres:1.1)

Negative prompt:
text, letters, watermark, logo, extra fingers, extra eyes, extra limbs, mutated hands, blurry face, photoreal human skin, messy background, busy pattern, copyright, existing character
```

---

### 4.2 全身站立设定图（full-body standing）

用途：锁全身比例、服装和剪影。双臂略离开身体，五指/翼端可见，脚完整，不裁顶不裁脚。

#### 模板 · Midjourney

```text
{英文角色锚点}, full body portrait, standing, neutral T-pose-like relaxed standing pose, arms slightly away from the body so wing-tips are visible, feet planted and fully visible, front view, character centered, full figure in frame with margin above the head and below the feet, plain light gray studio background, orthographic feel, studio lighting, soft lighting, product photography, sharp focus, highly readable silhouette, --ar 3:4 --stylize 50 --quality 1 --chaos 0 --v 6 --no text, cropped feet, cropped head, extra legs, extra wings, extra fingers, dynamic action pose, busy background
```

#### 已填示例 · Midjourney

```text
An original seaside trendy-toy IP mascot named Yanzi: a chubby seagull chick, about 1:2 head-to-body ratio, matte cream vinyl face, salt-white dense plush body with visible short fibres, coral-orange felt beak, huge glossy eyes each with exactly one crisp four-point star highlight. Wearing a mustard-yellow hooded windbreaker, a teal knit scarf with readable weave, and a tiny red-and-white life-ring backpack; a small wave embroidery on the chest. Mitten-like short wings, stubby legs, round highly readable silhouette, minimal facial features. Not a human, not an existing commercial IP. Fixed palette: cream #F6EAD2, salt-white #F8F4E7, coral-orange #E26A4A, mustard #E2B23A, teal #2BAEC6, life-ring red #E0263C, full body portrait, standing, relaxed standing pose, arms slightly away from the body so wing-tips are visible, feet planted and fully visible, front view, character centered, full figure in frame with margin above the head and below the feet, plain light gray studio background, orthographic feel, studio lighting, soft lighting, product photography, sharp focus, highly readable silhouette, --ar 3:4 --stylize 50 --quality 1 --chaos 0 --v 6 --no text, cropped feet, cropped head, extra legs, extra wings, extra fingers, dynamic action pose, busy background
```

#### 模板 · Flux / GPT Image

```text
Create a {画幅，建议 3:4} full-body standing character turn-in of {角色锚点}.
Pose: neutral standing, weight even on both feet, arms / wings slightly away from the torso, no action pose, no leaning out of frame.
Framing: entire body visible, including the top of the hood and both feet; leave a clean margin; do not crop.
Camera: straight-on front view, slight product-view, minimal perspective distortion (do not use 16mm or fisheye for this sheet).
Background: seamless light gray studio, soft contact shadow under the feet only.
Lighting: even studio soft light, gentle rim light, no dramatic night lighting.
Keep costume, colors and materials identical to the character lock.
Do not add text, logos, extra limbs, or a second character.
```

#### 已填示例 · Flux / GPT Image

```text
Create a 3:4 full-body standing character turn-in of an original seaside trendy-toy IP mascot named Yanzi: a chubby seagull chick, about 1:2 head-to-body ratio, matte cream vinyl face, salt-white dense plush body with visible short fibres, coral-orange felt beak, huge glossy eyes each with exactly one crisp four-point star highlight. Wearing a mustard-yellow hooded windbreaker, a teal knit scarf with readable weave, and a tiny red-and-white life-ring backpack; a small wave embroidery on the chest. Mitten-like short wings, stubby legs, round highly readable silhouette, minimal facial features. Not a human, not an existing commercial IP. Fixed palette: cream #F6EAD2, salt-white #F8F4E7, coral-orange #E26A4A, mustard #E2B23A, teal #2BAEC6, life-ring red #E0263C.
Pose: neutral standing, weight even on both feet, wings slightly away from the torso, no action pose, no leaning out of frame.
Framing: entire body visible, including the top of the hood and both feet; leave a clean margin; do not crop.
Camera: straight-on front view, slight product-view, minimal perspective distortion (do not use 16mm or fisheye for this sheet).
Background: seamless light gray studio, soft contact shadow under the feet only.
Lighting: even studio soft light, gentle rim light, no dramatic night lighting.
Keep costume, colors and materials identical to the character lock.
Do not add text, logos, extra limbs, or a second character.
```

#### 模板 · Stable Diffusion / SDXL

```text
正向：
{英文角色锚点}, full body portrait, standing, front view, arms slightly away from body, feet fully visible, centered, plain light gray background, studio lighting, soft lighting, product photography, (full figure in frame:1.3), (highly readable silhouette:1.2)

Negative prompt:
text, watermark, cropped feet, cropped head, closeup, bust only, extra legs, extra wings, extra fingers, bad anatomy, action pose, fisheye, busy background, photoreal human
```

#### 已填示例 · Stable Diffusion / SDXL

```text
正向：
An original seaside trendy-toy IP mascot named Yanzi, chubby seagull chick, matte cream vinyl face, salt-white dense plush body, coral-orange felt beak, huge glossy eyes with one four-point star highlight each, mustard-yellow hooded windbreaker, teal knit scarf, tiny red-and-white life-ring backpack, wave chest embroidery, mitten-like wings, stubby legs, full body portrait, standing, front view, arms slightly away from body, feet fully visible, centered, plain light gray background, studio lighting, soft lighting, product photography, (full figure in frame:1.3), (highly readable silhouette:1.2)

Negative prompt:
text, watermark, cropped feet, cropped head, closeup, bust only, extra legs, extra wings, extra fingers, bad anatomy, action pose, fisheye, busy background, photoreal human
```

---

### 4.3 三视图 / 周转图（three-view / turnaround）

用途：同一只角色在同一张图里出正面、侧面、背面（需要时加 3/4）。透视要平，像设定稿，不要广角。prompt-library 的人物类把「三视图」单独作为设定资产，和单张海报分开，这里沿用这个分类。

#### 模板 · Midjourney

```text
character turnaround sheet of {英文角色锚点}, orthographic, multiview projection, three consistent full-body views in a single row on one image: front view, side-view, back view, same scale, same lighting, same costume, same colors, standing, arms slightly away from body, feet visible, plain white background, model-sheet layout, clean even spacing, studio lighting, product-view, --ar 16:9 --stylize 50 --quality 1 --chaos 0 --v 6 --no perspective distortion, fisheye, text labels, watermark, different outfits, extra characters, merged bodies
```

说明：Midjourney 有时会把三只合成一只或换衣服。若一次失败，改用下方自然语言模型，或拆成三张再拼。

#### 已填示例 · Midjourney

```text
character turnaround sheet of an original seaside trendy-toy IP mascot named Yanzi: a chubby seagull chick, about 1:2 head-to-body ratio, matte cream vinyl face, salt-white dense plush body with visible short fibres, coral-orange felt beak, huge glossy eyes each with exactly one crisp four-point star highlight. Wearing a mustard-yellow hooded windbreaker, a teal knit scarf with readable weave, and a tiny red-and-white life-ring backpack; a small wave embroidery on the chest. Mitten-like short wings, stubby legs, round highly readable silhouette, minimal facial features. Not a human, not an existing commercial IP. Fixed palette: cream #F6EAD2, salt-white #F8F4E7, coral-orange #E26A4A, mustard #E2B23A, teal #2BAEC6, life-ring red #E0263C, orthographic, multiview projection, three consistent full-body views in a single row on one image: front view, side-view, back view, same scale, same lighting, same costume, same colors, standing, arms slightly away from body, feet visible, plain white background, model-sheet layout, clean even spacing, studio lighting, product-view, --ar 16:9 --stylize 50 --quality 1 --chaos 0 --v 6 --no perspective distortion, fisheye, text labels, watermark, different outfits, extra characters, merged bodies
```

#### 模板 · Flux / GPT Image（更稳，推荐）

```text
Create a {画幅，建议 16:9 或 3:2} character model-sheet turnaround of {角色锚点}.
Layout: one single image, plain white background, three full-body figures in one horizontal row, evenly spaced, identical size.
Views from left to right: 1) front view, 2) left side-view, 3) back view. Optional fourth 3/4 view only if the aspect ratio allows, never mix scales.
All three figures are the exact same character, same mustard windbreaker, same teal scarf, same life-ring backpack, same face and colors. The backpack must be visible on the back view; the wave embroidery visible on the front.
Pose: neutral standing, wings slightly away from the body, no action.
Camera: orthographic / product-view, no fisheye, no 16mm exaggeration, no ground plane scenery.
Do not add text, names, arrows, watermarks, or a fourth different character. Do not merge the three bodies together.
```

#### 已填示例 · Flux / GPT Image

```text
Create a 16:9 character model-sheet turnaround of an original seaside trendy-toy IP mascot named Yanzi: a chubby seagull chick, about 1:2 head-to-body ratio, matte cream vinyl face, salt-white dense plush body with visible short fibres, coral-orange felt beak, huge glossy eyes each with exactly one crisp four-point star highlight. Wearing a mustard-yellow hooded windbreaker, a teal knit scarf with readable weave, and a tiny red-and-white life-ring backpack; a small wave embroidery on the chest. Mitten-like short wings, stubby legs, round highly readable silhouette, minimal facial features. Not a human, not an existing commercial IP. Fixed palette: cream #F6EAD2, salt-white #F8F4E7, coral-orange #E26A4A, mustard #E2B23A, teal #2BAEC6, life-ring red #E0263C.
Layout: one single image, plain white background, three full-body figures in one horizontal row, evenly spaced, identical size.
Views from left to right: 1) front view, 2) left side-view, 3) back view.
All three figures are the exact same character, same mustard windbreaker, same teal scarf, same life-ring backpack, same face and colors. The backpack must be visible on the back view; the wave embroidery visible on the front.
Pose: neutral standing, wings slightly away from the body, no action.
Camera: orthographic / product-view, no fisheye, no 16mm exaggeration, no ground plane scenery.
Do not add text, names, arrows, watermarks, or a fourth different character. Do not merge the three bodies together.
```

#### 模板 · Stable Diffusion / SDXL

```text
正向：
character turnaround sheet, (same character:1.4), {英文角色锚点}, orthographic, multiview projection, front view, side-view, back view, three full body figures in a row, same scale, same outfit, standing, plain white background, model sheet, studio lighting, (consistent design:1.3)

Negative prompt:
text, watermark, different characters, different outfits, merged bodies, extra heads, fisheye, perspective distortion, cropped feet, busy background, photoreal human, extra fingers
```

#### 已填示例 · Stable Diffusion / SDXL

```text
正向：
character turnaround sheet, (same character:1.4), an original seaside trendy-toy IP mascot named Yanzi, chubby seagull chick, matte cream vinyl face, salt-white plush body, coral-orange felt beak, star-highlight eyes, mustard-yellow hooded windbreaker, teal knit scarf, life-ring backpack, orthographic, multiview projection, front view, side-view, back view, three full body figures in a row, same scale, same outfit, standing, plain white background, model sheet, studio lighting, (consistent design:1.3)

Negative prompt:
text, watermark, different characters, different outfits, merged bodies, extra heads, fisheye, perspective distortion, cropped feet, busy background, photoreal human, extra fingers
```

---

### 4.4 表情表（expression sheet）

用途：同一张脸排多种表情。只改变眉毛、眼睛、喙的形状，不改体型、服装和色板。

#### 模板 · Midjourney

```text
expression sheet of {英文角色锚点}, same bust-sized head repeated in a clean 2x3 grid on one image, identical face design and costume in every panel, only the expression changes, six expressions: joyful smile, surprised, sleepy, angry pout, wink, shy blush, plain off-white background, even studio lighting, character design sheet, highly readable facial features, --ar 16:9 --stylize 50 --quality 1 --chaos 0 --v 6 --no different characters, different colors, full body, text labels, watermark, extra eyes, merged faces
```

#### 已填示例 · Midjourney

```text
expression sheet of an original seaside trendy-toy IP mascot named Yanzi: a chubby seagull chick, matte cream vinyl face, salt-white dense plush body with visible short fibres, coral-orange felt beak, huge glossy eyes each with exactly one crisp four-point star highlight, mustard-yellow hooded windbreaker, teal knit scarf, tiny red-and-white life-ring backpack, wave embroidery on the chest, minimal facial features, same bust-sized head repeated in a clean 2x3 grid on one image, identical face design and costume in every panel, only the expression changes, six expressions: joyful smile, surprised, sleepy, angry pout, wink, shy blush, plain off-white background, even studio lighting, character design sheet, highly readable facial features, --ar 16:9 --stylize 50 --quality 1 --chaos 0 --v 6 --no different characters, different colors, full body, text labels, watermark, extra eyes, merged faces
```

#### 模板 · Flux / GPT Image（推荐）

```text
Create a {画幅，建议 16:9} expression sheet of {角色锚点}.
Layout: a clean 2x3 grid, six bust portraits of the exact same character, same size, same cream vinyl face, same costume and colors in every cell.
Only facial expression changes, in this order:
1. joyful wide smile
2. surprised, round eyes and open beak
3. sleepy, half-closed eyes
4. angry little pout
5. one-eye wink
6. shy blush, looking slightly aside
Do not change eye color, add or remove the star highlights, or alter the scarf and windbreaker. No text, no labels, no extra heads, no merged faces, no full-body poses. Plain off-white background, even studio light.
```

#### 已填示例 · Flux / GPT Image

```text
Create a 16:9 expression sheet of an original seaside trendy-toy IP mascot named Yanzi: a chubby seagull chick, about 1:2 head-to-body ratio, matte cream vinyl face, salt-white dense plush body with visible short fibres, coral-orange felt beak, huge glossy eyes each with exactly one crisp four-point star highlight. Wearing a mustard-yellow hooded windbreaker, a teal knit scarf with readable weave, and a tiny red-and-white life-ring backpack; a small wave embroidery on the chest. Minimal highly readable facial features. Fixed palette: cream #F6EAD2, salt-white #F8F4E7, coral-orange #E26A4A, mustard #E2B23A, teal #2BAEC6, life-ring red #E0263C.
Layout: a clean 2x3 grid, six bust portraits of the exact same character, same size, same cream vinyl face, same costume and colors in every cell.
Only facial expression changes, in this order:
1. joyful wide smile
2. surprised, round eyes and open beak
3. sleepy, half-closed eyes
4. angry little pout
5. one-eye wink
6. shy blush, looking slightly aside
Do not change eye color, add or remove the star highlights, or alter the scarf and windbreaker. No text, no labels, no extra heads, no merged faces, no full-body poses. Plain off-white background, even studio light.
```

#### 模板 · Stable Diffusion / SDXL

```text
正向：
expression sheet, (same character:1.4), {英文角色锚点}, 2x3 grid, six bust portraits, joyful smile, surprised, sleepy, angry pout, wink, shy blush, identical design, plain off-white background, studio lighting, character sheet

Negative prompt:
text, labels, watermark, different characters, different outfits, merged faces, extra eyes, full body, messy grid, photoreal human
```

#### 已填示例 · Stable Diffusion / SDXL

```text
正向：
expression sheet, (same character:1.4), Yanzi the chubby seagull-chick trendy-toy mascot, cream vinyl face, salt-white plush, coral-orange felt beak, star-highlight eyes, mustard windbreaker, teal knit scarf, 2x3 grid, six bust portraits, joyful smile, surprised, sleepy, angry pout, wink, shy blush, identical design, plain off-white background, studio lighting, character sheet

Negative prompt:
text, labels, watermark, different characters, different outfits, merged faces, extra eyes, full body, messy grid, photoreal human
```

---

### 4.5 潮流玩具 IP 角色（stylized trendy-toy IP character）

用途：出一张能代表 IP 的潮玩宣传像。若要「巨型尺度、广角、探出画面」，用 Soft Giants；若要「产品特写 + 漫画标题」，用 Plush Comic；若要户外活动感，用 Sunny 3D Avatar。下面给两种：一条通用 3D 潮玩（适合设定延伸），一条 Cookbook Soft Giants 填空（适合主视觉）。

#### 4.5-A 通用 3D 潮玩角色像 · Midjourney

```text
{英文角色锚点}, stylized 3D toy-mascot render, vinyl::1.5 plush::1.5, matte vinyl face, dense plush fur with visible fibres, stitched felt details, knit clothing with readable weave, full body, cheerful pose, standing on a low seam-sidewalk curb with sea wind lifting the scarf, three-quarter view, 35mm lens, studio plus bright sunlight, soft lighting, warm rim lighting, product photography, Cinema4D, Octane, sharp focus, highly readable IP look, --ar 3:4 --stylize 150 --quality 1 --chaos 0 --v 6 --no photoreal human, anime cel shading, flat vector, text, watermark, existing IP characters, extra limbs
```

#### 已填示例 · Midjourney

```text
An original seaside trendy-toy IP mascot named Yanzi: a chubby seagull chick, about 1:2 head-to-body ratio, matte cream vinyl face, salt-white dense plush body with visible short fibres, coral-orange felt beak, huge glossy eyes each with exactly one crisp four-point star highlight. Wearing a mustard-yellow hooded windbreaker, a teal knit scarf with readable weave, and a tiny red-and-white life-ring backpack; a small wave embroidery on the chest. Mitten-like short wings, stubby legs, round highly readable silhouette, minimal facial features. Not a human, not an existing commercial IP. Fixed palette: cream #F6EAD2, salt-white #F8F4E7, coral-orange #E26A4A, mustard #E2B23A, teal #2BAEC6, life-ring red #E0263C, stylized 3D toy-mascot render, vinyl::1.5 plush::1.5, matte vinyl face, dense plush fur with visible fibres, stitched felt details, knit clothing with readable weave, full body, cheerful pose, standing on a low seam-sidewalk curb with sea wind lifting the scarf, three-quarter view, 35mm lens, studio plus bright sunlight, soft lighting, warm rim lighting, product photography, Cinema4D, Octane, sharp focus, highly readable IP look, --ar 3:4 --stylize 150 --quality 1 --chaos 0 --v 6 --no photoreal human, anime cel shading, flat vector, text, watermark, existing IP characters, extra limbs
```

#### 4.5-B Soft Giants 风格主视觉 · Flux / GPT Image / Nano Banana Pro

把 `styles/soft-giants/style.json` 整份交给模型，再附上下面变量；或直接使用这段已展开提示词。注意：此风格要求角色与画框互动，不要改成中性站立。

```text
Create one full-bleed {ASPECT_RATIO} poster in the Soft Giants style.
Render: premium stylized 3D toy-mascot animation render; matte vinyl face, dense plush fur with visible fibres, stitched felt, knit or quilted clothing; huge glossy eyes each with one crisp four-point star highlight.
Camera: 16mm wide-angle, nearest feature enormous at the lens, world behind small.
Subject: {SUBJECT}
Action/camera: {SUBJECT_ACTION}
Composition: {DESIGN_DIRECTION}
Title, exact: "{MAIN_TEXT}", spelled letter by letter, giant chunky rounded sans capitals in acid lime with fuzzy airbrushed spray-grain edges, partly behind and partly in front of scene elements.
Overlay: thin white hairline rounded-corner frame; one small outlined pill label; small white handwritten tagline with crimson scribble underline and crimson four-point star.
Light: bright sunny daylight, warm rim light, rainbow light-leak streaks at two edges, blurred drifting particles, fine film grain.
Do not use existing IP characters, brand logos, human children, signatures, watermarks, flat 2D illustration, a neutral standing pose, a tiny title, sharp clean title edges, misspelled title, or extra limbs.
```

#### 已填示例 · Soft Giants × 盐仔（自然语言，16:9）

```text
Create one full-bleed 16:9 poster in the Soft Giants style.
Render: premium stylized 3D toy-mascot animation render; matte vinyl face, dense plush fur with visible fibres, stitched felt, knit or quilted clothing; huge glossy eyes each with one crisp four-point star highlight.
Camera: 16mm wide-angle, nearest feature enormous at the lens, world behind small.
Subject: Yanzi, an original chubby seagull-chick seaside trendy-toy mascot with a cream vinyl face, salt-white dense plush body, coral-orange felt beak, mustard-yellow hooded windbreaker, teal knit scarf and a tiny red-and-white life-ring backpack.
Action/camera: Peeking over a curved seaside promenade railing toward the lens, one mitten-wing and the coral beak huge in the foreground, a tiny coastal town and lighthouse far below on a curved horizon.
Composition: Face and wing fill the right half; the lime title SALT sits low left on the boardwalk, the railing overlapping the first letter; drifting soap-bubble and spray particles; tagline "big tide small town". Landscape native composition, not a crop from a vertical.
Title, exact: "SALT", spelled letter by letter, giant chunky rounded sans capitals in acid lime with fuzzy airbrushed spray-grain edges, partly behind and partly in front of scene elements.
Overlay: thin white hairline rounded-corner frame; one small outlined pill label 'HARBOR TOY'; small white handwritten tagline "big tide small town" with crimson scribble underline and crimson four-point star.
Light: bright sunny daylight, warm rim light, rainbow light-leak streaks at two edges, blurred drifting particles, fine film grain.
Do not use existing IP characters, brand logos, human children, signatures, watermarks, flat 2D illustration, a neutral standing pose, a tiny title, sharp clean title edges, misspelled title, or extra limbs.
```

若要用高识别度 2D 版，把同一只盐仔改成白色团块海鸥，套 `styles/cobalt-pals/style.json`：钴蓝底、粗黑线、五色齐出、大斜线裁切，标题建议短词如 `WAVE`。不要在这条里再写 Octane / 16mm / 毛绒纤维，那会跟「纯平涂、无阴影」锚点冲突。

---

### 4.6 同一角色换新场景（same character, new scene）

用途：脸、体型、服装、色板、材质全部保持不变，只换地点、动作、时间和光线。这是 Cookbook「换主题、保风格」在角色上的对应做法。

先写死「不变清单」，再写「可变更清单」：

```text
必须保持不变：角色锚点、头身比、脸材与五官、服装款式与色板、标志道具（救生圈背包、浪花刺绣）、整体画风。
这次只改变：地点、动作、时间、光线、次要环境元素、画幅。
```

#### 模板 · Midjourney

```text
{英文角色锚点}, the exact same character and costume, stylized 3D toy-mascot render, {新动作}, in {新场景}, {时间与光线}, {镜头与景别}, highly readable IP look, same colors and materials as the character lock, --ar {画幅} --stylize 150 --quality 1 --chaos 0 --v 6 --no costume change, different face, photoreal human, extra limbs, text, watermark, existing IP
```

#### 已填示例 · Midjourney（从港边改到夜市）

```text
An original seaside trendy-toy IP mascot named Yanzi: a chubby seagull chick, about 1:2 head-to-body ratio, matte cream vinyl face, salt-white dense plush body with visible short fibres, coral-orange felt beak, huge glossy eyes each with exactly one crisp four-point star highlight. Wearing a mustard-yellow hooded windbreaker, a teal knit scarf with readable weave, and a tiny red-and-white life-ring backpack; a small wave embroidery on the chest. Mitten-like short wings, stubby legs, round highly readable silhouette, minimal facial features. Not a human, not an existing commercial IP. Fixed palette: cream #F6EAD2, salt-white #F8F4E7, coral-orange #E26A4A, mustard #E2B23A, teal #2BAEC6, life-ring red #E0263C, the exact same character and costume, stylized 3D toy-mascot render, holding a paper tray of grilled squid and waving a mitten-wing, in a warm coastal night market under string lights and steam, dusk, practical lantern lighting, accent lighting, 35mm lens, full body, three-quarter view, highly readable IP look, same colors and materials as the character lock, --ar 3:4 --stylize 150 --quality 1 --chaos 0 --v 6 --no costume change, different face, photoreal human, extra limbs, text, watermark, existing IP
```

#### 模板 · Flux / GPT Image

```text
Create a {画幅} image of the exact same character as previously defined.
Keep unchanged: {角色锚点}. Same face, body proportions, mustard windbreaker, teal scarf, life-ring backpack, color palette and toy materials.
Change only the scene:
Action: {新动作}
Location: {新地点}
Time and light: {时间光线}
Camera: {镜头与景别}
Style must stay a premium stylized trendy-toy render, not a new art direction.
Do not redesign the character, swap the outfit, add text, logos, watermarks, or extra limbs.
```

#### 已填示例 · Flux / GPT Image（从港边改到雨天码头）

```text
Create a 16:9 image of the exact same character as previously defined.
Keep unchanged: an original seaside trendy-toy IP mascot named Yanzi, chubby seagull chick, 1:2 head-to-body ratio, matte cream vinyl face, salt-white dense plush body with visible fibres, coral-orange felt beak, huge glossy eyes with one four-point star highlight each, mustard-yellow hooded windbreaker, teal knit scarf, tiny red-and-white life-ring backpack, wave chest embroidery. Same palette: cream #F6EAD2, salt-white #F8F4E7, coral-orange #E26A4A, mustard #E2B23A, teal #2BAEC6, life-ring red #E0263C. Same toy materials.
Change only the scene:
Action: sitting on a wooden mooring post, kicking stubby legs, holding a tiny translucent raincoat hat in one wing, looking at a passing ferry.
Location: a rainy harbor pier, wet planks, stacked crates, blurred boats in the background, puddle reflection.
Time and light: late afternoon rain, soft overcast natural lighting, gentle rim light on wet plush fibres, no cinematic nightclub lighting.
Camera: 35mm lens, full body, low angle, character slightly left of center, deep enough environment but the mascot stays the clear hero.
Style must stay a premium stylized trendy-toy render, not a new art direction.
Do not redesign the character, swap the outfit, add text, logos, watermarks, or extra limbs.
```

#### 模板 · Stable Diffusion / SDXL

```text
正向：
{英文角色锚点}, (same character:1.4), (same costume:1.3), stylized 3D toy-mascot, {新动作}, {新场景}, {光线}, {镜头}, sharp focus

Negative prompt:
different face, different outfit, costume change, text, watermark, extra limbs, extra fingers, photoreal human, existing character, style shift, anime cel, flat vector
```

#### 已填示例 · Stable Diffusion / SDXL

```text
正向：
Yanzi the chubby seagull-chick trendy-toy mascot, cream vinyl face, salt-white plush, coral-orange felt beak, star-highlight eyes, mustard-yellow windbreaker, teal knit scarf, life-ring backpack, (same character:1.4), (same costume:1.3), stylized 3D toy-mascot, sitting on a wet wooden mooring post, rainy harbor pier, overcast soft lighting, 35mm lens, full body, low angle, sharp focus

Negative prompt:
different face, different outfit, costume change, text, watermark, extra limbs, extra fingers, photoreal human, existing character, style shift, anime cel, flat vector
```

若已经用某份 Cookbook JSON 出过主视觉，换场景时：**整份 JSON 不要改，只改 `SUBJECT_ACTION`、`LOCATION`、`BACKGROUND_ELEMENTS`、`PRODUCT_OR_PROP`、`MAIN_TEXT`**。不要为了新场景另写一套色板或渲染方式。

---
