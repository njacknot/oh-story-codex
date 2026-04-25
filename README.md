# oh-story-claudecode

网文写作 skill 包。6 个 skill 覆盖长篇与短篇网文的扫榜、拆文、写作、润色全流程。

v2.0.0

---

## 安装

```bash
npx skills add worldwonderer/oh-story-claudecode
```

支持 Claude Code、OpenClaw、Cursor、Copilot 等兼容 `npx skills` 协议的工具。

更新时重新执行同一条命令。

---

## Skill 列表

| Skill | 触发方式 | 功能 |
|---|---|---|
| `story-long-write` | `/story-long-write` `/story` `/网文` | 长篇写作。大纲搭建、人物设定、正文输出 |
| `story-long-analyze` | `/story-long-analyze` | 长篇拆文。黄金三章、爽点设计、节奏分析 |
| `story-long-scan` | `/story-long-scan` | 长篇扫榜。起点/番茄/晋江市场趋势 |
| `story-short-write` | `/story-short-write` | 短篇写作。情绪设计、反转构思、精修出稿 |
| `story-short-analyze` | `/story-short-analyze` | 短篇拆文。叙事结构、情绪曲线、钩子拆解 |
| `story-short-scan` | `/story-short-scan` | 短篇扫榜。知乎盐言/番茄短篇风口数据 |
| `story-deslop` | `/story-deslop` `/去AI味` | 去AI味。检测并清除AI写作痕迹 |

自然语言同样可触发：「帮我开书」→ `story-long-write`，「这篇太AI了」→ `story-deslop`。

---

## 典型流程

```
长篇：scan（什么火）→ analyze（拆爆款学结构）→ write（开书）
短篇：scan（什么情绪火）→ analyze（拆爆款学反转）→ write（出稿）
写作后：deslop（去AI味）
```

有明确方向时直接跳到对应的 write skill。

---

## 知识体系

v2.0 采用分层知识架构，核心方法论集中管理，各 skill 按需引用。

**共享知识**（`story-long-write/references/`，带元数据头标记消费 skills）

| 主题 | 涵盖 |
|---|---|
| 人物设计与分析 | 角色设定 + 拆文视角的人物提取/关系映射/动机链 |
| 钩子技法 | 章尾钩子 + 段落级钩子 + 悬念构建 + 分层策略 |
| 对话技法 | 节奏/潜台词/信息控制 + 对话模式数据库 |
| 去AI味 | 预防 + 三遍去AI法 + 改写范例库 |
| 质量检查 | 通用 + 长篇专项 + 短篇专项 |
| 情绪弧线 | 6 种弧形模板 + 期待感管理 |
| 反转工具箱 | 类型 + 时机 + 误导路径 |
| 题材框架 | 长篇（8 节点）+ 短篇（压缩三幕）双视角 |

**专属知识**（各 skill 自行维护）

大纲排布、八节点结构、连续性管理、风格模块（长篇）；21 大题材写作公式、知乎盐言格式（短篇）；禁用词表（去AI味）；拆文案例（短篇拆文）；市场数据（扫榜）。

---

## 适用平台

**长篇**：起点中文网、番茄小说、晋江文学城、七猫小说、刺猬猫

**短篇**：知乎盐言故事、番茄短篇、七猫短篇、小红书故事

---

## License

MIT
