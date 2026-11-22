# 角色与儿童绘本提示词 Skills

把两类文生图提示词拆成可复用 Skill：角色 / 吉祥物 / 潮玩 IP 的设定图与海报，以及儿童启蒙绘本、分页插画和闪卡。

可以直接在 Cursor、Claude Code 或其他兼容 [Agent Skills](https://docs.claude.com/en/docs/agents-and-tools/agent-skills) 的环境里当技能目录用，也可以只复制其中一份 `SKILL.md`。

## 五个 Skill

| 目录 | 什么时候用 |
| --- | --- |
| [skills/character-image-prompt](skills/character-image-prompt) | 写或修改角色、设定图、三视图、表情表提示词 |
| [skills/image-style-lock](skills/image-style-lock) | 把同一套画风跨图稳住，或使用 `style.json` 出海报 |
| [skills/image-prompt-fix](skills/image-prompt-fix) | 手崩、脸漂、风格不一致、语法混用等失败后改词 |
| [skills/children-picture-book](skills/children-picture-book) | 把识字、拼音、习惯、情绪、科普等儿童启蒙内容做成插画绘本、分页提示词或闪卡 |
| [skills/children-illustration-styles](skills/children-illustration-styles) | 把儿童绘本、启蒙插画或闪卡的画风跨页锁定，或套用绘本风格配方 |

用法提要：先按模型分语法（Midjourney 用 `--ar` / `--no`，Stable Diffusion 用权重和独立负面词，Flux / GPT Image 用自然语言），再锁主体锚点，只改镜头和场景。角色向技能按 12 个槽位填空；儿童绘本则先定年龄与安全边界，再锁角色圣经和一种画风，逐页只改动作与场景。`image-style-lock` 里的 5 个 JSON 更适合海报和潮玩宣传图，不要硬套到白底设定图或低龄绘本内页。

角色向技能的完整长文说明在 [docs/角色出图提示词写法.md](docs/角色出图提示词写法.md)。

## 怎么用

把本仓库放到项目里后，指向 `skills/` 下的子目录即可。例如在 Cursor 中，可将某个 Skill 目录复制到项目的 `.cursor/skills/` 或个人技能库。每个 Skill 的入口都是该目录下的 `SKILL.md`，相对路径引用同目录的 `references/` 或 `styles/`。

示例角色「盐仔」是虚构的海边潮玩吉祥物，只作填空示范，换成自己的角色时只改锚点那一段。儿童绘本里的示例角色「阿潮」是虚构的海边小镇小朋友，同样只作填空示范。

## 来源与许可

本仓库的技能正文和整理说明以 MIT 许可发布，见 [LICENSE](LICENSE)。

内容提炼自（请保留署名）：

- [MidJourney Styles and Keywords Reference](https://github.com/willwulfken/MidJourney-Styles-and-Keywords-Reference)（willwulfken）：关键词分类与参数对照。该仓库体积极大，本项目只吸收了整理后的短词表，没有复制样例图。
- [AI Visual Prompt Cookbook](https://github.com/VigoZhao/AI-Visual-Prompt-Cookbook)（@VigoCreativeAI）：锁风格方法和 `style.json` 结构。`skills/image-style-lock/styles/` 下 5 个 `style.json` 为原件复制，按 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 使用，复用请注明 AI Visual Prompt Cookbook / [@VigoCreativeAI](https://x.com/VigoCreativeAI)。
- [prompt-library](https://github.com/Nihilist-ZIO/prompt-library)（Nihilist-ZIO）：只参考了人物 / 构图分类和「语法不能混用」的纪律，没有复制其词条正文。
- [picture-skills](https://github.com/kart-io/picture-skills)（kart-io）：儿童双语绘本的年龄分档、学习领域、场景可观察性和风格关键词。该仓库 README 写明 MIT License，但公开检索时没有 LICENSE 文件；本项目只蒸馏方法，并改编了短关键词，没有复制其角色设定或大段正文。
- [storybook-generator-skill](https://github.com/weaiw/storybook-generator-skill)（Storybook Generator Skill contributors，MIT）：故事分页、角色圣经、图文契约、拼音—中文—英文版式和质检流程。
- [companion-picture-book](https://github.com/892041548/companion-picture-book)（MIT；方法上亦参考 MIT 许可的 [kangqiang1996-bot/picture-book-generator](https://github.com/kangqiang1996-bot/picture-book-generator)）：适龄创作起点、习惯 / 情绪 / 家庭等主题分支，以及五张绘本风格卡。
- [hand-drawn-styles](https://github.com/threerocks/hand-drawn-styles)（liulei，MIT）：儿童绘本相关画风的材料、色板和互斥项，主要包括 `STYLES.md` 第 12、13、14、16、17、18、23 号，以及蜡笔相关条目。本项目写成中文风格卡，没有整段复制其英文验证模板。
- [picture-book](https://github.com/weivea/picture-book)：仅作为「经典水彩、蜡笔、拼贴、北欧、扁平图形等常见绘本画材分类」的对照。该仓库在公开检索时没有 LICENSE 文件或许可声明，因此没有复制其提示词模板、示例页或代表作列表。
- [ai-coloring-book-prompts](https://github.com/gunjchhetri/ai-coloring-book-prompts)（InkChamps，提示词与文案为 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)）：只指向字母、数字、习惯、情绪、科普等主题分类，没有复制提示词正文。若转载其提示词本身，须注明 “AI Coloring Book Prompts by InkChamps” 并链接该仓库。

详见 [NOTICE](NOTICE)。
