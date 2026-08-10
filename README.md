# AI Persona Skills / 人物思维操作系统

> Thinking frameworks distilled from world-class minds. Installable skills for Claude Code, Codex, and OpenCode — each one is a runnable "cognitive operating system" that lets you think, decide, and express like the person it models.

> 从世界级人物身上蒸馏出的思维框架。可直接安装到 Claude Code / Codex / OpenCode，每个 skill 都是一套可运行的"认知操作系统"，让你像那个人一样思考、决策、表达。

---

## Why This Exists / 为什么做这个

Most "prompts" tell an AI *what* to say. These skills capture **HOW** great minds think:

- Which **mental models** are their lenses on the world?
- Which **decision heuristics** do they apply automatically?
- What is their **expression DNA** (phrasing, rhythm, tone)?
- What do they **absolutely refuse** to do? (anti-patterns)
- What are the **honest boundaries** of the skill?

Each skill was built from deep research: books, talks, interviews, writing, decisions, and external critiques — then distilled into mental models, heuristics, and a complete expression DNA.

大多数提示词只告诉 AI *说什么*。这些 skill 捕捉的是大人物**怎么想**：

- 他用什么**心智模型**看世界？
- 他有哪些**决策启发式**？
- 他的**表达 DNA** 是什么（措辞、节奏、语气）？
- 他**绝对不会**做什么？（反模式）
- 这个 skill 的**诚实边界**在哪？

每个 skill 都基于深度调研（著作、演讲、访谈、写作、决策记录、外部批评），蒸馏成心智模型、决策启发式和完整表达 DNA。

---

## Included Skills / 包含的人物

### 🇨🇳 Chinese Thought Leaders / 中文思想者

| Skill | Person | Focus |
|---|---|---|
| `chendong-perspective` | 辰东 Chen Dong | 网络小说创作、世界观架构 |
| `duan-yongping-perspective` | 段永平 Duan Yongping | 投资、商业本质、本分文化 |
| `hax-perspective` | 贺师俊 Hax | 前端工程、技术判断 |
| `lei-jun-perspective` | 雷军 Lei Jun | 创业、产品、小米方法论 |
| `luqi-perspective` | 陆奇 Qi Lu | AI 趋势、创业、组织变革 |
| `mao-perspective` | 毛泽东 Mao Zedong | 战略、矛盾论、军事思维 |
| `tiancantudou-perspective` | 天蚕土豆 Tian Can Tu Dou | 网文爽点设计、节奏控制 |
| `zhang-xiaolong-perspective` | 张小龙 Zhang Xiaolong | 产品哲学、微信方法论 |
| `zhangwensong-perspective` | 章文嵩 Zhang Wensong | 技术管理、系统架构 |
| `zhangxinxu-perspective` | 张鑫旭 Zhang Xinxu | 前端技术写作 |
| `zhangxuefeng-perspective` | 张雪峰 Zhang Xuefeng | 志愿填报、职业规划 |
| `zhang-yiming-perspective` | 张一鸣 Zhang Yiming | 字节跳动、组织效率、长期主义 |

### 🌍 Global Thinkers / 全球思想家

| Skill | Person | Focus |
|---|---|---|
| `andrej-karpathy-perspective` | Andrej Karpathy | AI/深度学习、技术教育 |
| `elon-musk-perspective` | Elon Musk | 第一性原理、工程执行 |
| `feynman-perspective` | Richard Feynman | 物理学思维、学习方法 |
| `ilya-sutskever-perspective` | Ilya Sutskever | AGI、深度学习 |
| `mrbeast-perspective` | MrBeast | 内容创作、增长 |
| `munger-perspective` | Charlie Munger | 多元思维模型、投资 |
| `naval-perspective` | Naval Ravikant | 财富、杠杆、长期主义 |
| `paul-graham-perspective` | Paul Graham | 创业、写作、科技 |
| `steve-jobs-perspective` | Steve Jobs | 产品、设计、演讲 |
| `sun-yuchen-perspective` | Justin Sun | 加密、营销、增长 |
| `taleb-perspective` | Nassim Taleb | 反脆弱、不确定性 |
| `trump-perspective` | Donald Trump | 谈判、媒体、品牌 |
| `yao-qizhi-perspective` | 姚期智 Andrew Yao | 计算机理论、图灵奖 |
| `x-mastery-mentor` | X/Twitter 运营 | 内容与个人品牌 |

### 📚 Special / 特别款

| Skill | What it is |
|---|---|
| `courage-to-be-disliked-perspective` | 《被讨厌的勇气》/阿德勒心理学框架 |
| `perspective-roundtable` | 多人物视角圆桌讨论工具 |

### 🔨 The Factory / 造人工厂

| Skill | What it is |
|---|---|
| `nuwa-skill` (女娲) | 输入人名/主题，自动深度调研 → 提炼思维框架 → 生成新的人物 Skill |

---

## Installation / 安装

### Codex

```powershell
$CODEX_HOME = "$env:USERPROFILE\.codex"
Copy-Item skills\luqi-perspective "$CODEX_HOME\skills\" -Recurse
```

### Claude Code

```bash
mkdir -p ~/.claude/skills
cp -r skills/luqi-perspective ~/.claude/skills/
```

### OpenCode

```bash
mkdir -p ~/.config/opencode/skills
cp -r skills/luqi-perspective ~/.config/opencode/skills/
```

Install a single skill, or copy the whole `skills/` folder to get all of them.

安装单个 skill，或把整个 `skills/` 文件夹复制到对应目录。

---

## Usage / 使用

Once installed, each skill activates automatically on triggers like:

- 「用陆奇的视角分析」「陆奇会怎么看」「Qi Lu perspective」
- 「用 Naval 的视角」「这份工作有杠杆吗」「切换到 Naval」
- 「用费曼的方法学习」「第一性原理分析」

Or you can explicitly invoke: `请用 <person> 的思维方式分析 <topic>`.

安装后，每个 skill 会自动在触发词下激活，也可以显式要求"用 XX 的思维方式分析 XX"。

---

## Project Structure / 目录结构

```
ai-persona-skills/
├── README.md          # This file / 本文件
├── skills/            # 27 installable perspective skills
│   ├── luqi-perspective/
│   │   ├── SKILL.md        # 主技能定义
│   │   ├── FIDELITY.md     # 忠实度说明 / fidelity notes
│   │   └── test-prompts.json
│   └── ...
└── nuwa-skill/        # 女娲：造人工厂（生成新的人物 Skill）
```

---

## License / 许可

MIT

---

*Skills are educational tools for thinking frameworks — they capture HOW a person thinks, not their copyrighted words. Personas are for analytical/advisory use, not impersonation.*
