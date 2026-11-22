# 常用角色关键词短表

配合 `SKILL.md` 使用。投 Midjourney 时可直接把英文词放进提示词；投 Stable Diffusion 时同样可用这些英文词，需要强调再加 `(word:1.2)`；投 Flux / GPT Image 时把词写成句子，不要堆一排无语法标签。

## 5. 常用角色关键词短表

词条提炼自 MidJourney Styles 仓库 V4 Just The Style 各页的表格标题（Camera、Perspective、Lighting、Materials、Material_Properties、Design_Styles、Drawing_and_Art_Mediums、Digital、Themes、Dimensionality、SFX_and_Shaders、Intangibles）。仓库本身是「一词一图」对照，没有给每词写定义；下面的效果说明是按词义和这些分类整理的实用注释，便于选词，不是官方释义。每类 8–15 个，只留角色出图常用项。

投 Midjourney 时可直接把英文词放进提示词；投 SD 时同样可用这些英文词，需要强调再加 `(word:1.2)`；投 Flux / GPT Image 时把词写成句子，不要堆一排无语法标签。

### 5.1 景别 / 构图（Camera + Perspective + prompt-library 构图分类）

| 英文词 | 作用（一行） |
| --- | --- |
| Extreme Closeup | 大特写，只剩眼睛或喙，适合材质细节，不适合锁全身。 |
| Closeup / Closeup-View | 近景特写，脸和头饰为主。 |
| Portrait / Portraiture | 胸像级人像，肩膀以上，设定卡头图常用。 |
| Full Body Portrait | 全身像，务必再写 feet fully visible，否则容易裁脚。 |
| Wide Shot / Epic Wide Shot | 远景，角色变小、环境变大，适合场景海报，不适合第一次定妆。 |
| Establishing Shot | 建场镜头，先交代地点，角色不必占满画面。 |
| Centered-Shot | 居中，设定图、产品像更稳。 |
| Profile | 正侧脸/正侧身，三视图侧面用这个。 |
| Product-View | 产品展示视角，潮玩主图比「剧情镜头」更干净。 |
| Selfie / First-Person View | 第一人称或自拍感，宣传互动可以用，设定图不要用。 |
| Rule of Thirds | 三分法，场景图比白底设定图更需要。 |
| Closed Composition | 封闭构图，主体收在画面内，适合海报。 |

### 5.2 镜头 / 机位（Camera + Perspective）

| 英文词 | 作用（一行） |
| --- | --- |
| 35mm Lens | 接近人眼的标准焦距，设定图和普通全身像首选。 |
| 85mm Lens | 中长焦，胸像更压缩、更像人像摄影。 |
| Macro / Macro View | 微距，看绒毛和缝线；不要拿来拍全身。 |
| Wide Angle / Ultra-Wide Angle | 广角，空间被撑开，近处夸张。 |
| 15mm Lens / Fisheye Lens | 极广或鱼眼，Soft Giants / Sunny Avatar 类宣传图才用；三视图禁用。 |
| Telephoto | 长焦压缩前后景，环境肖像感。 |
| Low Angle | 仰拍，角色显得大、有气势。 |
| High Angle / Top-View / Aerial View | 俯拍或顶视，能交代队形和场景，脸会变小。 |
| Worms-Eye View | 极低仰视，巨人感，和 Soft Giants 的「近处巨大」一致。 |
| Orthographic / Multiview Projection | 正交/多视图，三视图必写，去掉透视变形。 |
| Isometric / Axonometric | 轴测/等轴测，偏设计展示，不是写实相机。 |
| Depth of Field / Shallow Focus / Bokeh | 浅景深虚化背景，宣传图好用；设定图改 Deep Focus，避免脸发糊。 |
| Soft-Focus | 柔焦，氛围感强，但会损「高度可读」。 |
| Lens Flare / Vignette | 镜头光斑和暗角，气氛配件，设定图应 `--no` 掉。 |

### 5.3 光线（Lighting）

| 英文词 | 作用（一行） |
| --- | --- |
| Studio Lighting | 棚灯，均匀可控，设定图、产品像首选。 |
| Soft Lighting | 软光，过渡干净，毛绒边缘更舒服。 |
| Hard Lighting | 硬光，阴影锐利，块面海报或强日光才用。 |
| Frontlight | 顺光，脸部信息最全，表情表好用。 |
| Backlight / Rim Lighting / Rim Lights | 逆光或轮廊光，把毛边和剪影从背景里勾出来。 |
| Natural Lighting / Sunlight / Direct Sunlight | 自然光或直射阳光，户外场景真实，注意别把脸曝掉。 |
| Golden Hour / Blue Hour | 金色黄昏或蓝调时刻，换场景时用来改时间，不改角色。 |
| High-Key Lighting | 高调，亮、少阴影，适合干净 IP 形象。 |
| Low-Key Lighting | 低调，暗、阴影多，情绪强，吉祥物主识别一般不用。 |
| Cinematic Lighting / Moody Lighting | 电影感/情绪光，宣传片可以，设定稿容易风格漂移。 |
| Accent Lighting | 局部强调光，打在关键道具（如救生圈）上。 |
| Volumetric Lighting / Godrays / Sunbeams | 体积光或耶稣光，空气感强，容易抢戏。 |
| Global Illumination | 全局照明，3D 渲染更自然，适合潮玩渲染词组。 |
| Candlelight / Practical 氛围灯 | 暖点光源，夜市场景可用；不要和棚拍设定图混用。 |

### 5.4 材质（Materials + Material_Properties）

| 英文词 | 作用（一行） |
| --- | --- |
| Vinyl / Polyvinyl | 乙烯玩具表面，潮玩脸和关节常用，偏光滑但可写成 matte vinyl。 |
| Plastic | 塑料感，更工业；要「潮玩」可与 vinyl 连用，避免变成廉价硬胶。 |
| Plush / Fur / Furry | 毛绒，最好再写 visible fibres，否则容易塑成光滑壳。 |
| Felt / Felt Cloth | 毡，适合喙、补丁、扁平玩具零件。 |
| Knitted / Cotton / Velvet / Satin | 针织、棉、丝绒、缎：衣服织纹；针织围巾要写 readable weave。 |
| Rubber / Silicone | 橡胶或硅胶，更软弹，适合玩具手感，不像硬塑料。 |
| Clay / Terracotta / Ceramic | 黏土、陶土、陶瓷，偏手作或公仔，不是毛绒潮玩。 |
| Matte | 哑光，降低油亮，IP 脸更稳、更好看。 |
| Glossy / Shiny / Specular Highlights | 高光和反光，眼睛、潮湿表面可用；不要整身都 glossy。 |
| Translucent / Subsurface-Scattering | 半透明和次表面散射，耳尖、指尖透光（Soft Giants 锚点就有这个）。 |
| Soft / Squishy / Soft Body / Blobby | 软、可挤压、团块感，强化吉祥物体型。 |
| Stitched / Sewing / Embroidered（可与 stitched felt 连用） | 缝线、刺绣，让玩具像能缝出来的，而不是裸模。 |

### 5.5 画风（Design_Styles + Themes + Drawing_and_Art_Mediums + Digital + Dimensionality + SFX）

| 英文词 | 作用（一行） |
| --- | --- |
| Stylized | 总的「风格化」开关，比 realistic 更适合 IP。 |
| 3D / 3D Render / Cinema4D / C4D / Octane / Blender Render | 指向三维渲染器审美，潮玩主形象常用；一次只留 1–2 个引擎词。 |
| 2D / Flat / Flat Design / Flat Shading | 平面/平涂，走 Cobalt Pals 或 Bold Block 路线时用，不要和 Octane 同句。 |
| 2.5D | 介于 2D 与 3D 之间的厚涂或半立体，偏设定插画。 |
| Product Photography | 产品摄影感，白底或棚拍潮玩更像可售商品。 |
| Claymation / Stop Motion | 黏土动画或定格，另一种玩具感，和乙烯潮玩不是同一套。 |
| Cartoon / Kawaii / Anime / Manga | 卡通、可爱、动漫、漫画；IP 若要「高度可读潮玩」，不要同时堆 anime 和 Octane。 |
| Pop-Art / Memphis Design / Bauhaus Style | 强图形、色块、设计运动风格，海报系统可用。 |
| Ligne Claire / Ukiyo-e / Storybook Illustration | 清晰线描、浮世绘、绘本插画，偏 2D 叙事，不是 3D 产品像。 |
| Cel Shading | 赛璐璐分层上色，动漫感明确；Sunny 3D Avatar 的 avoid 里排除了它。 |
| Line Art / Doodle / Marker Art / Risograph / Sticker | 线稿、涂鸦、马克笔、孔版、贴纸，适合平面物料和活动海报。 |
| Minimalist / Hyperdetailed | 极简 vs 超细：吉祥物识别优先选干净剪影，细节点到材质即可，不要无节制 hyperdetailed。 |

### 5.6 质量与完成度（Digital + Camera + Design_Styles + SFX）

| 英文词 | 作用（一行） |
| --- | --- |
| Sharp / Sharpened / Sharp focus | 边缘清楚，设定图和表情表优先。 |
| 4k / 8k / UHD / Super-Resolution | Digital 页里的分辨率风格词，有一点「更精细」的倾向；它代替不了 MJ 的 `--quality`。 |
| HD / Full-HD | 同样是清晰度风格词，效力通常弱于具体的材质和镜头描述。 |
| Precision Rendering / Physically Based Rendering | 强调渲染精度或 PBR，3D 潮玩可用。 |
| Award Winning Photography | Camera 页词，偏摄影精品感；角色 IP 用得少，容易把画风拉向写实。 |
| Clean design / highly readable silhouette（自然语言，推荐） | 直接要求「干净、剪影可读」，比空泛的 masterpiece 对 IP 更有效。 |
| Anti-Aliasing / De-Noise / Digitally Enhanced / Post-Processing | 去锯齿、降噪、后期感；可轻度使用，写太多会变成滤镜堆砌。 |
| Film Grain | 细胶片颗粒，Soft Giants 锚点里有；干净电商白底则应排除。 |
| Cute / Whimsical / Playful Atmosphere | Intangibles / Themes 里的气质词，能把「玩具」往可爱推，但锁不住结构。 |
| --quality 1（仅 Midjourney 参数） | 仓库原文：控制生成花费的时间。设定图用 1；不要把它写进 SD 或 Flux。 |

---
