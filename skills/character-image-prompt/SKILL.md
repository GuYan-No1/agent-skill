---
name: character-image-prompt
description: 写或修改角色、吉祥物、潮玩 IP、设定图、三视图、表情表的文生图提示词时使用。
---

# 角色出图提示词

按下面步骤写提示词，不要把不同模型的语法写在同一条里。细节模板见 [references/templates.md](references/templates.md)，词表见 [references/keywords.md](references/keywords.md)。需要锁海报画风时，改用同仓库的 `image-style-lock`；出图失败要改词时，用 `image-prompt-fix`。

## 1. 先选模型，语法不要混用

同一套画面结构可以共用，参数写法必须按模型分开。

| 模型 | 怎么写约束 | 不要混入 |
| --- | --- | --- |
| Midjourney / Niji | 正文用逗号或自然语言，参数放末尾：`--ar 3:4 --stylize 100 --v 6`。排除用 `--no extra fingers, text, watermark`。强调用短词加权：`vinyl::1.5`。 | 不要写 `(hand:1.4)`，也不要另起一行 `Negative prompt:`。 |
| Stable Diffusion / SDXL | 强调用 `(word:1.2)`，减弱用 `(word:0.7)`。负面词必须单独放在 Negative prompt 里。 | 不要写 `--ar`、`--stylize`、`--v`、`--no`。画幅用界面宽高。 |
| Flux / GPT Image / DALL·E / Nano Banana Pro | 用完整自然语言写清要什么、不要什么。画幅写成 “Create a 3:4 image”，禁止项写成 “Do not include…”。 | 不要把 `--ar 16:9` 或 `(plastic:1.3)` 塞进自然语言段。 |

还要记住：词序会改画面，重要主体放前面；锁材质用 `made of vinyl and plush`，锁画风用 `in the style of flat design`。

## 2. 写角色锚点，之后每次原样粘贴

先锁「角色 + 造型 + 画风」，再改姿势、景别和场景。锚点固定，只替换镜头和场景。换自己的 IP 时只改锚点这一段，后面所有模板都引用它。

锚点必须写清：物种/名字、头身比、脸和标志特征、服装与固定色板（最好补十六进制）、材质（写到能摸到）、不是真人、不是现有商业 IP。

示例（虚构海边潮玩「盐仔」，可直接试，也可整段替换）：

```text
一只原创海边潮玩吉祥物「盐仔」：圆滚滚的海鸥雏鸟体型，头身比约 1:2，奶油色哑光乙烯脸，盐白色密绒身体（可见短纤维），珊瑚橙毡喙，巨大光泽眼睛，每只眼睛里只有一颗清晰的四点星形高光。穿芥末黄连帽风衣，戴青绿针织围巾（可见织纹），背后一个迷你红白救生圈背包，胸口有小小浪花刺绣。短翼像连指手套，粗短腿，剪影圆润清晰，五官极简、高度可读。不是真人，不是现有商业 IP。
固定色板：奶油 #F6EAD2，盐白 #F8F4E7，珊瑚橙 #E26A4A，芥末黄 #E2B23A，青绿 #2BAEC6，救生圈红 #E0263C。
```

英文锚点（投 Midjourney / Flux / 英文模型时用）见 [references/templates.md](references/templates.md) 开头的已填示例。

## 3. 按 12 个槽位填空

```text
【主体】谁：物种 / 名字 / 体型 / 年龄感 / 是吉祥物还是真人
【造型】头身比、脸、眼睛、标志特征（每次原样粘贴）
【姿势】站、坐、走、挥手；设定图要写 “neutral standing pose, arms slightly away from body”
【服饰与配色】衣服、配饰、固定色板（写颜色名，最好补十六进制）
【景别 / 构图】特写、胸像、半身、全身、三视图、表情表；是否居中、留白、白底
【镜头】焦距、机位、透视
【光线】棚灯、阳光、rim light 等
【材质】乙烯、毛绒、针织、毡、塑料等，写到能摸到的程度
【风格】2D 平涂 / 3D 潮玩 / 扁平面 / 产品海报；只选一种，不要同时写互斥风格
【画幅】3:4 设定图、16:9 场景、1:1 头像、3:2 或 16:9 三视图/表情表
【质量】按模型填写（见下）
【禁止项】多余手指、脸漂、水印、现有 IP、真实品牌、混风格、设定图里的文字
```

质量槽：

- Midjourney：设定图用 `--quality 1 --stylize 50-100 --chaos 0`；宣传图可将 `--stylize` 提到 250–500。正文可加 `3D render, product photography, sharp focus`。不要既写 `--quality 1` 又堆 `16k 32k masterpiece`。`--quality` 控制生成花费，不是清晰度本身。
- Stable Diffusion：正词写 `sharp focus, clean design, highly readable silhouette`；手和脸的问题放进 Negative prompt。
- Flux / GPT Image：写成完整句子。若要锁海报风格，把整个 `style.json` 喂给模型，不要只摘一句形容词。

## 4. 按出图类型选模板

先贴角色锚点，再打开 [references/templates.md](references/templates.md) 复制对应模型的模板，只改花括号里的内容：

- 胸像 / 角色设定卡：立脸、材质和配色；白底或浅底，画面内不要字
- 全身站立设定图：写 `full body portrait, feet fully visible`，手臂离开身体
- 三视图 / 周转图：正交、同一比例、同一套服装；不要用鱼眼或 16mm
- 表情表：写明 “only the expression changes”；失败就拆成单张再拼
- 潮玩 IP 宣传形象：可提高 stylize，仍不要混 2D/3D
- 同一角色换场景：只改地点和动作，锚点整段保留

选词时查 [references/keywords.md](references/keywords.md)。一条提示词只保留一个渲染体系。

## 5. 输出要求

- 按用户指定的模型各给一组完整、可直接复制的提示词；未指定时先问或同时给出 MJ / SD / 自然语言三套，并标明模型。
- 多组提示词必须各自写全，不要写「沿用上方」。
- 设定图、三视图、表情表默认禁止画面内文字。
- 不要把真实公司地址、密钥或未公开项目名写进提示词。
