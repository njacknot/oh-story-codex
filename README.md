# oh-story

网络小说创作工具箱。7 个 Claude Code skill，覆盖长篇与短篇网文的扫榜、拆文、写作全流程。

**当前版本：v1.0.0**

## 如何安装

#### Claude Code

```bash
claude plugin marketplace add worldwonderer/oh-story-claudecode
claude plugin install story@oh-story-skills
```

#### 通用安装方式

```bash
npx skills add worldwonderer/oh-story-claudecode
```

## 如何更新

#### Claude Code 插件市场安装的用户

```bash
claude plugin marketplace update oh-story-skills
claude plugin update story@oh-story-skills
/reload-plugins
```

#### 通过 `npx skills add` 安装的用户

重新运行一次同样的命令即可：

```bash
npx skills add worldwonderer/oh-story-claudecode
```

---

## 工具箱

### 长篇工具

| Skill | 做什么 |
|---|---|
| `/story` | 主入口，自动路由到对的工具 |
| `/story-long-scan` | 长篇扫榜。分析起点/番茄/晋江排行榜数据，提炼市场趋势 |
| `/story-long-analyze` | 长篇拆文。深度拆解黄金三章、人设架构、爽点设计、节奏控制 |
| `/story-long-write` | 长篇写作。从大纲到正文，辅助长篇网文创作全流程 |

### 短篇工具

| Skill | 做什么 |
|---|---|
| `/story-short-scan` | 短篇扫榜。分析知乎盐言/番茄短篇数据，捕捉风口题材 |
| `/story-short-analyze` | 短篇拆文。拆解爆款叙事结构、情绪曲线、反转技巧 |
| `/story-short-write` | 短篇写作。从构思到成稿，聚焦情绪拉扯与节奏把控 |

### 工具路径图

#### 长篇主线

```text
long-scan（什么题材火）
    ↓
long-analyze（拆一本爆款学结构）
    ↓
long-write（开书写作）
```

#### 短篇主线

```text
short-scan（什么情绪火）
    ↓
short-analyze（拆一篇爆款学反转）
    ↓
short-write（动笔写稿）
```

#### 快速通道

```text
已有方向，直接写 → /story-long-write 或 /story-short-write
已有作品，想拆解 → /story-long-analyze 或 /story-short-analyze
```

---

## 知识库

每个 skill 背后有对应的知识库文件提供方法论支撑：

| 知识包 | 内容 |
|---|---|
| `long-scan_网文市场数据` | 各平台数据、题材趋势、分析方法论 |
| `long-analyze_拆文方法论` | 黄金三章理论、爽点设计、节奏控制 |
| `long-write_长篇写作框架` | 大纲体系、世界观构建、人物管理 |
| `short-scan_短篇市场数据` | 短篇平台格局、情绪市场、风口识别 |
| `short-analyze_短篇拆文方法论` | 反转设计、情绪曲线、结构模型 |
| `short-write_短篇写作框架` | 写作流程、平台适配、精修技巧 |

---

## 适用平台

### 长篇
起点中文网、番茄小说、晋江文学城、七猫小说、刺猬猫

### 短篇
知乎盐言故事、番茄短篇、七猫短篇、小红书故事

---

## 使用示例

### 示例 1：长篇从零开始

```
用户：我想写一本长篇网文，但不知道写什么
→ /story → 路由到 /story-long-scan
→ 扫榜分析后推荐方向
→ /story-long-analyze 拆一本同类型爆款
→ /story-long-write 开始写大纲和正文
```

### 示例 2：短篇快速出稿

```
用户：帮我写一篇知乎盐言风格的短篇
→ /story → 路由到 /story-short-write
→ 确定情绪目标 → 设计反转 → 写初稿 → 精修
```

### 示例 3：拆解学习

```
用户：帮我拆一下《XX》的黄金三章
→ /story-long-analyze → 逐章拆解
```

---

## License

MIT
