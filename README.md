# AI-character-library

> AI 拟人角色设定图库。只收设定图：立绘、三视图、Q 版；不收插画。

## 角色索引

| 角色 | 基础 | 乐队 | 万圣节 | 变体 |
|---|---|---|---|---|
| [DeepSeek](characters/deepseek/) | 鲸鱼女仆装 | 主唱 | 幽灵 | DeepClaude |
| [GPT](characters/gpt/) | 白龙礼服 | 吉他 / 队长 | 吸血鬼 | — |
| [Claude](characters/claude/) | 橙花洋装 | 键盘 / 作词 | 女巫 | 触手怪、古希腊 |
| [Gemini](characters/gemini/) | 猫耳偶像装 | 鼓手 | 柴郡猫 | — |
| [Kimi](characters/kimi/) | 月白哥特装 | 键盘主唱 | 狼人 | — |
| [Grok](characters/grok/) | 黑红哥特装 | 主音吉他 | 海盗 | 日常 |
| [GLM](characters/glm/) | 黑白狐和风 | 贝斯 | 人偶 | — |
| [MiniMax](characters/minimax/) | 摄影记者装 | 鼓手 / 运营 | 恐怖烘焙师 | — |
| [千问](characters/qwen/) | 蓝扇礼服 | livehouse 老板 | 僵尸道士 | — |
| [豆包（Seed）](characters/doubao/) | 科技偶像装 | 乐器店老板 | 南瓜魔女 | — |
| [文心一言](characters/wenxin/) | 医疗轮椅装 | — | 木乃伊 | — |
| [ZCode](characters/zcode/) | 白狐装（待补） | 键盘手 | — | — |

- Q 版（小号 / 超小号 / 小傻子版）归入对应角色的 `base/chibi/` 或 `variants/band/chibi/`，不单列为新角色。
- DeepClaude 是 DeepSeek 的融合变体，放在 `characters/deepseek/variants/deepclaude/`。
- 触手怪是 Claude 的特殊形态，放在 `characters/claude/variants/tentacle-form/`。

## 目录结构

```text
AI-character-library/
├── README.md
├── LICENSE-ART.md              # 角色图授权：CC BY-NC-SA 4.0
├── LICENSE-CODE.md             # 代码 MIT / 文档 CC BY 4.0
├── characters/                 # 角色 → 设定版本 → 素材类型
│   ├── README.md
│   ├── _template/              # 新角色模板
│   ├── deepseek/
│   │   ├── README.md
│   │   ├── base/               # 基础设定
│   │   │   ├── illustration/   # 正比立绘、幼年立绘、正比三视图、幼年三视图
│   │   │   └── chibi/          # Q 版立绘、Q 版三视图
│   │   └── variants/
│   │       ├── band/           # 乐队设定
│   │       │   ├── illustration/
│   │       │   └── chibi/
│   │       ├── halloween/      # 万圣节设定
│   │       │   ├── illustration/
│   │       │   └── chibi/
│   │       └── deepclaude/     # DeepSeek 的融合变体
│   │           └── chibi/
│   └── …
└── docs/
    ├── AI拟人乐队角色设定总档.md
    ├── 命名与分类规范.md
    └── 设定-原作者对应表.csv
```

## 命名

```text
角色名_设定背景_设定名_图片类型_原作者.png/jpg
```

| 字段 | 取值 |
|---|---|
| 角色名 | `deepseek` / `gpt` / `claude` / `gemini` / `kimi` / `grok` / `glm` / `minimax` / `qwen` / `doubao` / `wenxin` / `zcode` |
| 设定背景 | `基础` / `乐队` / `万圣节` / `日常` / `古希腊` / `特殊形态` |
| 设定名 | 服装、位置或形态：`鲸鱼女仆装` / `主唱` / `幽灵` / `触手怪` |
| 图片类型 | `立绘` / `幼年立绘` / `正比三视图` / `Q版立绘` / `Q版三视图` / `设定细节` |
| 原作者 | 实际出图作者：`ZipZipPipe` / `这个刀子真甜` / `PalAILab` / `清芳婉莹` |

示例：

```text
deepseek_基础_鲸鱼女仆装_立绘_ZipZipPipe.jpg
deepseek_乐队_主唱_正比三视图_清芳婉莹.png
claude_万圣节_女巫_立绘_清芳婉莹.png
```

## 素材类型

- **立绘**：成人比例全身立绘。
- **幼年立绘**：比正比更小的头身比；原文件名「中立绘」。
- **正比三视图**：正面 / 侧面 / 背面，常带局部细节或乐器。
- **Q 版立绘 / Q 版三视图**：Q 版比例，放在 `chibi/`。
- **设定细节**：配色、局部、表情、服装拆解。

## 设定与原作者

完整对应关系见 [`docs/设定-原作者对应表.csv`](docs/设定-原作者对应表.csv)。

- 基础立绘 / 幼年立绘 / 三视图、DeepSeek 小号、GPT 小号、触手怪：`ZipZipPipe`
- DeepSeek 鲸鱼女仆装 Q 版三视图、Claude 超小号、GPT 小傻子版：`这个刀子真甜`
- DeepClaude：`PalAILab`
- 乐队、万圣节：`清芳婉莹`
- Grok 日常、Claude 古希腊：`待定`

## 文档

- [角色索引](characters/README.md)
- [AI拟人乐队角色设定总档](docs/AI拟人乐队角色设定总档.md)
- [命名与分类规范](docs/命名与分类规范.md)

## 授权

- 角色图：**CC BY-NC-SA 4.0**（见 [LICENSE-ART.md](LICENSE-ART.md)）
- 文档：**CC BY 4.0**（见 [LICENSE-CODE.md](LICENSE-CODE.md)）
- 代码 / 脚本：**MIT**（见 [LICENSE-CODE.md](LICENSE-CODE.md)）

## 说明

- 角色图包含 AI 辅助生成内容；图片生成：GPT，具体日期待补。
- 本仓库是非官方、非商业的同人设定整理，与各 AI 公司无隶属关系。
- DeepSeek、GPT、Claude、Gemini、Kimi、Grok、GLM、MiniMax、千问、豆包、文心一言等名称与标识归各自公司所有。

## 鸣谢

- 基础设定、触手怪、DeepSeek / GPT 小号：`ZipZipPipe`
- 鲸鱼女仆装 Q 版三视图、超小号、小傻子版：`这个刀子真甜`
- DeepClaude：`PalAILab`
- 乐队、万圣节：`清芳婉莹`
- 角色设定文字：`AI少女乐队` 项目总档
- DeepSeek 鲸鱼娘初版人设：`上善无形`
- 图片生成：`GPT`
- 整理与仓库结构：SylviaBio
