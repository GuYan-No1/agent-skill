# 角色出图提示词 Skills

把角色 / 吉祥物 / 潮玩 IP 的文生图提示词写法拆成三个可复用 Skill：写提示词、锁画风、修失败图。

可以直接在 Cursor、Claude Code 或其他兼容 [Agent Skills](https://docs.claude.com/en/docs/agents-and-tools/agent-skills) 的环境里当技能目录用，也可以只复制其中一份 `SKILL.md`。

## 三个 Skill

| 目录 | 什么时候用 |
| --- | --- |
| [skills/character-image-prompt](skills/character-image-prompt) | 写或修改角色、设定图、三视图、表情表提示词 |
| [skills/image-style-lock](skills/image-style-lock) | 把同一套画风跨图稳住，或使用 `style.json` 出海报 |
| [skills/image-prompt-fix](skills/image-prompt-fix) | 手崩、脸漂、风格不一致、语法混用等失败后改词 |

用法提要：先按模型分语法（Midjourney 用 `--ar` / `--no`，Stable Diffusion 用权重和独立负面词，Flux / GPT Image 用自然语言），再按 12 个槽位填空；角色锚点固定，只改镜头和场景。`image-style-lock` 里的 5 个 JSON 更适合海报和潮玩宣传图，白底设定图不要硬套。

完整长文说明在 [docs/角色出图提示词写法.md](docs/角色出图提示词写法.md)。

## 怎么用

把本仓库放到项目里后，指向 `skills/` 下的子目录即可。例如在 Cursor 中，可将某个 Skill 目录复制到项目的 `.cursor/skills/` 或个人技能库。每个 Skill 的入口都是该目录下的 `SKILL.md`，相对路径引用同目录的 `references/` 或 `styles/`。

示例角色「盐仔」是虚构的海边潮玩吉祥物，只作填空示范，换成自己的角色时只改锚点那一段。

## 来源与许可

本仓库的技能正文和整理说明以 MIT 许可发布，见 [LICENSE](LICENSE)。

内容提炼自（请保留署名）：

- [MidJourney Styles and Keywords Reference](https://github.com/willwulfken/MidJourney-Styles-and-Keywords-Reference)（willwulfken）：关键词分类与参数对照。该仓库体积极大，本项目只吸收了整理后的短词表，没有复制样例图。
- [AI Visual Prompt Cookbook](https://github.com/VigoZhao/AI-Visual-Prompt-Cookbook)（@VigoCreativeAI）：锁风格方法和 `style.json` 结构。`skills/image-style-lock/styles/` 下 5 个 `style.json` 为原件复制，按 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 使用，复用请注明 AI Visual Prompt Cookbook / [@VigoCreativeAI](https://x.com/VigoCreativeAI)。
- [prompt-library](https://github.com/Nihilist-ZIO/prompt-library)（Nihilist-ZIO）：只参考了人物 / 构图分类和「语法不能混用」的纪律，没有复制其词条正文。

详见 [NOTICE](NOTICE)。
