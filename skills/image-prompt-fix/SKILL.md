---
name: image-prompt-fix
description: 出图失败或质量差、需要改提示词时使用，例如手崩、脸漂、多余手指、风格不一致、语法混用、裁头裁脚。
---

# 出图提示词修正

先判断是哪类失败，再按下面改词。不要一上来继续往上堆词。某一部位反复崩时，先删互斥词和过高 stylize，做减法。

改词时仍要遵守模型语法分界，并尽量完整保留角色锚点。完整模板和词表见 `character-image-prompt`；锁风格问题见 `image-style-lock`。

## 修正表

| 问题 | 常见原因 | 怎么改 |
| --- | --- | --- |
| 手/翼崩坏、多余手指 | 没写清「连指翼」或「手离开身体」；或在 Midjourney 里误用了 SD 的 `(hand:1.5)` | 设定图写 `arms slightly away from the body, mitten-like wings, no extra fingers`。MJ 用 `--no extra fingers, extra limbs`；SD 把这些放进 Negative prompt，不要把 `--no` 贴进 SD。 |
| 脸漂移、换场面孔不像 | 只写了「同一只角色」，没有重复锚点；或同时换了光线、风格和服装 | 每次完整粘贴角色锚点。换场景只改地点和动作。表情表写明 “only the expression changes”。能图生图时，用已通过的设定图作参考。 |
| 多手指、多眼睛、多腿 | 广角/鱼眼把肢体拆碎；或 grid 表情表/三视图合成失败 | 设定类禁用 `Fisheye`、`16mm`。三视图、表情表写 `same scale`、`do not merge bodies/faces`，失败就拆成单张再拼。SD 加重 `(same character:1.4)` 并负面排除 `mutated hands, extra eyes`。 |
| 画风不稳定、忽 2D 忽 3D | 一句里同时写了 `Octane, anime, flat design, watercolor` | 一条提示词只保留一个渲染体系。3D 潮玩：`stylized 3D toy-mascot render, vinyl, plush, Octane`。2D IP：`flat 2D cartoon, thick black outline, pure flat fills, no shading`。把互斥项写进禁止里。 |
| 语法混用导致模型不理部分词 | 在 MJ 写 `Negative prompt:` 和 `(word:1.2)`；在 SD 写 `--ar 3:4 --v 6`；在 Flux 末尾加 `--stylize 200` | 按模型重写。画幅：MJ 用 `--ar`，SD 用界面宽高，Flux/GPT Image 用 “Create a 3:4 image”。排除项：MJ 用 `--no`，SD 用 Negative prompt，自然语言模型用 “Do not include…”。 |
| 想锁风格却越写越散 | 每张图重写全部形容词，色板和镜头也不固定 | 固定材质、色板、线宽、渲染模式；只换动作和地点。直接加载风格 JSON，不要从记忆里改写色值。 |
| 三视图变成三个不同角色 | 模型把「三视图」理解成「三个角色」；或画幅太方导致挤压 | 用 16:9，写 `one character, three views, same scale, same costume`。明确左右顺序。仍失败就分三次生成正面/侧面/背面，保持同一套锚点和种子（MJ 加 `--chaos 0`）。 |
| 裁头、裁脚、只出胸像 | 写了 portrait 却想要全身；或 stylize / 广角过强 | 明确 `full body portrait, feet fully visible, margin above the head`，并排除 `cropped feet, cropped head, closeup`。设定图把 Midjourney `--stylize` 降到 50–80。 |
| 画面里出现乱字、水印、假 logo | 宣传风格默认会要标题 | 设定图、三视图、表情表一律禁止文字。海报类把标题写死，并要求 spelled letter by letter；不要让模型自己编品牌名。 |
| 毛绒变成光滑塑料，或反之 | 材质词太少，或和互斥风格混用 | 毛绒：`dense plush, visible fibres, stitched, matte`。乙烯脸：`matte vinyl face` 和毛身分开写。不要在 Cobalt Pals 这类平涂风格里写 plush fibres。 |
| 吉祥物看起来像真人儿童或现有 IP | 缺 “not a human / not an existing commercial IP”，或风格锚点不够 | 锚点写物种和玩具材质。禁止项加上 `photoreal human, realistic child, existing IP characters`。 |
| Midjourney 词权重不明显 | `::` 加在整段长句后面，或和 SD 权重混写 | 把**短词**加权：`vinyl::1.5 plush::1.5`。不要写成 `(vinyl:1.5)`。重要主体放最前面。 |

## 输出要求

- 先用一两句话指出失败类型和原因，再给出改好的完整提示词，不要只给补丁碎片。
- 按用户正在用的模型输出；如果原词已经混用语法，先拆开再重写。
- 能做减法就不要加长。改完后检查：锚点是否还在、是否仍只剩一种画风、禁止项是否写成了该模型的语法。
