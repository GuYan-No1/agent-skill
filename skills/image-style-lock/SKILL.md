---
name: image-style-lock
description: 需要把同一套画风跨图稳住，或使用 style.json / Visual Prompt Cookbook 风格包出角色海报时使用。
---

# 画风锁定

Cookbook 的核心不是再写一句 `in the style of`，而是把一种视觉系统写成可复用的 `style.json`：**锚点固定，只换变量**。本技能附带 5 个角色向原件，路径在 [styles/](styles/)。

白底设定图、三视图、表情表不要用这些海报风格，改走 `character-image-prompt` 里的中性棚拍模板。

复用这些 `style.json` 时按 CC BY 4.0 注明 [AI Visual Prompt Cookbook](https://github.com/VigoZhao/AI-Visual-Prompt-Cookbook) / [@VigoCreativeAI](https://x.com/VigoCreativeAI)。

## 1. 锁风格的 7 步

1. **先定风格锚点 `style_fidelity_anchors`**  
   把必须每次出现的东西写成 6–12 条：渲染方式、材质、色板、线宽、镜头、构图层级。标成 CORE 的不要改；FLEX 的（物种、动作、标题位置）才按张替换。
2. **只替换 `environment_variables`**  
   常见变量：`SUBJECT`、`SUBJECT_ACTION`、`PRODUCT_OR_PROP`、`LOCATION`、`BACKGROUND_ELEMENTS`、`WARDROBE_STYLE`、`MAIN_TEXT`、`ASPECT_RATIO`。角色锚点相当于不可变的 `SUBJECT` 描述。
3. **固定色板 `color_palette`**  
   写准主色、点缀色和「哪些颜色必须同时出现」。例如 Cobalt Pals 要求钴蓝、白、黑、蛋黄、泡泡糖粉五色每张都可见。
4. **写清 `source_content_to_avoid`**  
   这不是普通负面词，而是「不要抄原参考的角色、文案、构图故事」。换主题时必须换主体、道具、文字，但保住锚点。
5. **用 `design_rules` / `do` / `avoid` 管构图纪律**  
   例如 Soft Giants 明确禁止「中性站立吉祥物」；做设定图就不要用这个风格。
6. **画幅原生生成，不要裁切**  
   9:16 和 16:9 要按同一角色和标题重新构图，禁止从竖图裁出横图。
7. **有字就要逐字核对准**  
   标题写进 `MAIN_TEXT`，并要求 spelled letter by letter。角色设定图建议画面内不要字。

## 2. 怎么用附带的 style.json

1. 按下一节选一个风格，打开对应 `styles/<slug>/style.json`。
2. 把**完整 JSON** 放进 ChatGPT Images、Nano Banana Pro 或其他能读长 JSON 的图像模型，不要只复制一句话 summary。
3. 在 `examples` 里新增一个 case，或直接改变量：把 `SUBJECT` 换成角色锚点，再填动作、场景、标题。
4. 不要改 `style_fidelity_anchors`、`color_palette`、`design_rules`。画幅按 JSON 说明选 9:16 或 16:9。
5. 这些 JSON 是海报系统，不是设定稿系统。

投 Midjourney 或 Stable Diffusion 时，不要把整份 JSON 生贴进去。应把锚点里的材质、色板、镜头改写成该模型语法，仍保持「锚点固定、只换变量」。

## 3. 五份风格各适合什么图

- **Soft Giants**（`styles/soft-giants/`）  
  3D 潮玩巨型海报。哑光乙烯脸 + 密绒可见纤维；眼睛里固定一颗四点星高光；16mm 广角；角色必须和画框或重力玩，禁止中性站姿。适合主视觉和尺度反差海报，不适合三视图、表情表、白底设定图。
- **Cobalt Pals**（`styles/cobalt-pals/`）  
  平面活动海报。整张钴蓝平涂底，白色团块动物，粗黑马克笔轮廓，无阴影；固定五色（钴蓝 #1466D8、白、黑、蛋黄 #FFE100、泡泡糖粉 #F26BB5）。适合高识别度 2D IP 主视觉和贴纸感物料，不适合写实棚拍或立体毛绒产品特写。
- **Sunny 3D Avatar Campaign Style**（`styles/sunny-3d-avatar-campaign-style/`）  
  晴天户外 3D 头像海报。光滑玩偶感 3D、烈日高饱和、广角近景裁切、巨大白色标题。适合社交投放和活动预热，不适合扁平矢量、写实真人或白底设定图。
- **Plush Comic Toy Product Poster Style**（`styles/plush-comic-toy-product-poster-style/`）  
  毛绒玩具产品海报。奶油纸底 + 青绿大圆、软棚影、倾斜漫画标题。适合潮玩产品主图和周边上市海报，不适合极简奢侈品风或没有绒毛的光滑塑料。
- **Bold Block Mascot Poster Style**（`styles/bold-block-mascot-poster-style/`）  
  粗块面吉祥物海报。巨型黑体标题、圆滚白吉祥物、极粗黑线、青/薄荷色大色板、米白印刷纸感。适合高度可读的贴纸/网印/社交海报，不适合写实 3D 或精细绘画。

## 4. 输出要求

- 先说明选了哪个风格、为什么适合当前用途，以及它不适合什么。
- 给出改好变量后的完整用法：能读 JSON 的模型就输出完整 JSON 或明确的变量表；MJ / SD 则改写成对应语法的完整提示词。
- 不要改写原件中的色值和 CORE 锚点；不要把未公开的项目内部名称写进标题。
