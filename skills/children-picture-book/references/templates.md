# 角色圣经与逐页提示词模板

换成自己的角色时，只改圣经和锚点，不要删掉图文契约、肢体约束和禁止项。示例角色「阿潮」是虚构的海边小镇小朋友，不是真实儿童，也不是现有商业 IP。

## 角色圣经填空

```markdown
## 主角
- 名字：
- 物种 / 年龄感：
- 身份：
- 性格：
- 体型与头身比：
- 脸部特征：
- 发型 / 毛色：
- 固定服装与颜色：
- 固定配饰：
- 常见表情与表情基调：
- 标志性动作：
- 手部 / 肢体规则：正常只有两只手、两条手臂、两条腿；常见拿法；被遮挡时哪些不可见
- 不能改变：
- 适合的画风：与全书主风格一致

## 配角（如有，每人也写同样字段）

## 世界锚点
- 地点、季节、时间：
- 场景锚点（少而醒目）：
- 道具锚点：
- 色彩锚点：
```

已填示例（阿潮）：

```text
阿潮，一个约 5 岁的原创男孩，圆脸，短而黑的头发，额头有一络常常翘起的碎发，眼睛圆而清楚，不是写实儿童照片。头身比大约 1:4，四肢短而稳。穿海沫蓝罩衫、米白短裤，脚上是芥末黄雨靴，背上一个扇贝形状的小布包，包上有一粒珊瑚橙纽扣。表情基调是认真而轻微着急。不是真人，不是现有商业 IP。
不能改变：海沫蓝罩衫、芥末黄雨靴、扇贝小包和那粒珊瑚橙纽扣、翘起的一络碎发。
场景锚点：海埠街家门口的蓝色小门，门边一块白底贝壳垫，门楣上有一个手写的「家」字（如需在画面出现文字，只保留这一个字，否则留给后期排版）。
道具锚点：一对芥末黄雨靴、一块小布、一碗热汤冒着的白气。
肢体规则：只画出两只手。若抱着小布，写清左手按布、右手扶靴；不要第三只手，不要多余手指。
```

英文锚点（投 Midjourney、Flux 或其他英文模型时用）：

```text
A-Chao, an original fictional boy about 5 years old, round face, short black hair with one little tuft that always sticks up, clear round eyes, not a photorealistic child portrait. About 1:4 head-to-body proportion, short sturdy limbs. Sea-foam blue smock, rice-white shorts, mustard-yellow rain boots, a scallop-shaped cloth backpack with one coral-orange button. Earnest, slightly hurried expression. Not a real person, not an existing commercial IP.
Must stay the same: sea-foam blue smock, mustard-yellow boots, scallop backpack and its coral-orange button, the sticking-up tuft of hair.
```

## 逐页提示词：自然语言（Flux / GPT Image / DALL·E / Nano Banana Pro）

把方括号换成本页内容。不要加入 `--ar` 或 `(word:1.2)`。

```text
Create a 3:4 children's picture-book illustration, wholesome and age-appropriate.

Book: [书名]
Page: [封面 / 第 N 页]
Readers: [年龄段]

Character (repeat every page):
[完整角色锚点]

This page only:
[一个动作、场景、情绪、镜头；只讲一件事]

Visual evidence for the page text:
[正文提到的物件和动作，逐项列出，必须在画面中可见]

Hands and body:
[可见手/脚数量，左右手用途，遮挡关系]

Style (CORE, repeat every page):
[从 children-illustration-styles 复制的风格锚点、材质和色板]

Continuity:
Keep the same character design, clothes, props, palette, and medium as previous pages. Only the pose, expression, and this page's action may change.

Text in the image:
[内页默认：Do not include any text, letters, captions, signatures, watermarks, or logos in the image. Text will be added later in layout.]
[封面若需要标题：The cover must show the exact Chinese title「……」and the exact subtitle「……」, spelled correctly, with no extra words. Leave clear space so type does not cover the face or key props.]

Do not include: photorealistic children, 3D CGI, commercial posters, user-interface chrome, watermarks, logos, brand marks, copyrighted characters, scary or violent content, adult themes, unsafe instructions a child could copy, extra arms, a third hand, fused limbs, or extra fingers.
```

## 逐页提示词：Midjourney / Niji

正文用自然语言或短词，参数只放末尾。不要写 Negative prompt，也不要写 `(word:1.2)`。

```text
children's picture book illustration, [风格 CORE 短词], [完整角色锚点], [本页唯一动作与场景], [镜头], [图文证据短词], wholesome educational scene for ages [年龄], consistent character design, [材质], [色板]
--ar 3:4 --stylize 80 --v 6 --no extra fingers, extra arms, text, watermark, logo, brand, photorealistic child, 3D render, scary, violence, gore, sexual content, copyrighted character
```

封面若要进画标题，把准确书名写进正文，并在生成后逐字检查；不稳就改为无字封面，后期排版。闪卡默认同样加上 `--no text, watermark`。需要更克制的绘本感时，把 `--stylize` 放在约 50–100，不要堆 `masterpiece 16k` 一类空词。

## 逐页提示词：Stable Diffusion / SDXL

强调用 `(word:1.2)`，减弱用 `(word:0.7)`。画幅在界面里设置，例如 3:4。不要写 `--ar` 或 `--no`。

```text
children's picture book illustration, (consistent character:1.2), [完整角色锚点], [本页动作与场景], [风格 CORE], (wholesome educational illustration:1.1), [材质], [色板], clear readable pose, soft age-appropriate lighting
```

```text
Negative prompt: extra fingers, extra arms, fused limbs, mutated hands, text, letters, watermark, logo, brand, photorealistic child, photograph, 3D render, CGI, scary, horror, violence, gore, blood, sexual content, nsfw, copyrighted character, trademark, busy cluttered background, dark gloomy lighting
```

## 组装顺序

1. 页类型和画幅
2. 完整角色锚点（每次原样粘贴）
3. 本页唯一动作、场景、情绪、镜头
4. 图文契约
5. 肢体约束
6. 风格 CORE
7. 连续性要求
8. 文字策略
9. 禁止项（按模型语法书写）

有人物的页面必须写清手的数量和用途。动作太多时拆页，或让一件道具放在地上，不必两只手同时做三件事。

## 建议的项目目录

只使用示例路径，不要写入真实服务器或账号信息：

```text
picture-book/a-chao-rainboots/
  00-brief.md
  01-character-bible.md
  02-page-plan.md
  03-cover-plan.md
  prompts/page-00-cover.md
  prompts/page-01.md
  images/00-cover.png
  images/01.png
```

不要覆盖已通过的旧图；返工保存为 `01-v2.png`。
