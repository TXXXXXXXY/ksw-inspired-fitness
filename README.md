# KSW Inspired Fitness / 凯圣王启发的健身教练 Skill

<div align="center">

**An AI Agent Skill that turns any LLM into a professional fitness coach, based on the teaching methodology of [凯圣王 (Kai Sheng Wang)](https://www.douyin.com/user/MS4wLjABAAAAjnKGbRiPmA8tqEn8WAWSqr89M7HQhpxsJdXdgM6bebf2c9pxX4GRBWG9I6GmppEA), a top Chinese fitness educator with 1M+ followers. Works with QoderWork, Claude, ChatGPT, or any AI agent that supports custom instructions.**

**一个基于抖音百万粉丝健身博主凯圣王教学体系的 AI 智能体技能，让任意大模型变身专业健身教练。适用于 QoderWork、Claude、ChatGPT 等所有支持自定义指令的 AI 工具。**

[![Skill Files](https://img.shields.io/badge/Skill_Files-6-blue)](#-file-structure)
[![Exercises](https://img.shields.io/badge/Exercise_DB-1324-green)](#-data-sources)
[![Platform](https://img.shields.io/badge/Platform-Agnostic-lightgrey)](#-installation--安装方法)
[![Languages](https://img.shields.io/badge/Languages-CN%20%7C%20EN-yellow)](#-overview)

</div>

---

## What This Does / 这是什么

This is a **structured knowledge package** that teaches any AI how to coach fitness like a professional trainer. Once loaded, the AI can:

这是一套**结构化的健身知识包**，教会任意 AI 像专业教练一样指导训练。加载后，AI 可以：

- **Generate training plans** — Push/Pull/Legs splits, beginner progressions, customized to your goals, experience, and injuries
- **编排训练计划** — 推/拉/腿三分化、新手进阶路径，根据你的目标、经验和伤病定制

- **Query exercise knowledge** — Step-by-step instructions, common mistakes, regression/progression variants for 50+ exercises
- **查询动作知识** — 50+ 动作的详细指导、常见错误、退阶/进阶变体

- **Design carb-cycling diets** — Complete formulas, meal plans, and food recommendations for fat loss
- **设计碳循环饮食方案** — 完整的减脂计算公式、饮食计划和食物推荐

- **Handle injuries safely** — Substitution exercises for shoulder, lower back, knee, and wrist injuries
- **安全处理伤病** — 肩/腰/膝/腕四大常见伤病的替代动作方案

- **Validate training logic** — Muscle synergy analysis ensures plans account for indirect muscle fatigue
- **校验训练逻辑** — 肌肉协同关系分析，确保计划考虑到肌群的间接疲劳消耗

---

## Who Is 凯圣王? / 凯圣王是谁？

凯圣王 is a certified sports nutritionist trainer at the Chinese Society of Food Science and Technology, and one of China's most influential fitness educators on Douyin (Chinese TikTok) with over 1 million followers. He is known for his rigorous, science-based teaching style and co-developed the **Functional 3-Split Training System** with Tan Chengyi (谭成义).

凯圣王是中国食品科学技术学会运动营养师课程培训师，抖音粉丝超百万的健身博主。他以逻辑严密、信息密度高的教学风格著称，与谭成义合作开发了**功能性三分化训练体系**。

His content covers: exercise technique breakdowns (48M+ views), follow-along workouts (54M+ views), nutrition guidance (7.3M+ views), and training unit theory (5.16M+ views).

他的内容涵盖：动作详解（4800万+播放）、第三视角跟练（5480万+播放）、饮食讲解（730万+播放）、训练单位讲解（516万+播放）。

---

## File Structure / 文件结构

```
ksw-fitness-skill/
├── SKILL.md                        # Main skill file / 主技能文件
├── exercise-library.md             # Core exercises with detailed cues / 凯圣王核心动作详解
├── exercise-library-expanded.md    # 50+ exercises from 1,324 DB with Chinese instructions / 扩展动作库
├── muscle-synergy.md               # Muscle synergy & fatigue chain analysis / 肌肉协同关系
├── injury-substitutions.md         # Injury-safe exercise substitutions / 伤病替代方案
├── programming-decision-tree.md    # 7-step plan generation logic / 训练编排决策树
├── README.md                       # This file
└── LICENSE
```

### What Each File Does / 各文件职责

| File / 文件 | Purpose / 用途 |
|------|------|
| **SKILL.md** | Core knowledge: training philosophy, 3-split plan, carb cycling, warm-up, safety rules / 核心知识：训练理念、三分化、碳循环、热身、安全规则 |
| **exercise-library.md** | Detailed exercise guide: form cues, common mistakes, regressions / 核心动作详解：发力要点、常见错误、退阶变体 |
| **exercise-library-expanded.md** | 50+ curated exercises per muscle group with Chinese instructions from ExerciseDB / 按肌群精选的50+动作，附中文指导 |
| **muscle-synergy.md** | Data-driven analysis of which muscles are indirectly fatigued by each exercise / 基于数据的肌肉连锁消耗分析 |
| **injury-substitutions.md** | Forbidden exercises & safe alternatives for shoulder/back/knee/wrist injuries / 四大伤病的禁忌动作与安全替代 |
| **programming-decision-tree.md** | Complete 7-step workflow: assess → select split → choose exercises → validate synergy → output plan / 完整7步排计划流程 |

---

## Installation / 安装方法

This skill is **platform-agnostic** — it works with any AI agent that supports custom instructions or knowledge loading.

本技能**不绑定任何平台** —— 适用于所有支持自定义指令/知识加载的 AI 智能体。

### Step 1: Get the files / 获取文件

```bash
git clone https://github.com/TXXXXXXXY/ksw-inspired-fitness.git
```

Or click **Code → Download ZIP** on the GitHub page.

或点击 GitHub 页面上的 **Code → Download ZIP**。

### Step 2: Load into your AI agent / 加载到你的 AI 工具

<details>
<summary><b>QoderWork</b></summary>

Copy the folder to your skills directory:

```
# Windows
%USERPROFILE%\.qoderworkcn\skills\ksw-inspired-fitness\

# macOS / Linux
~/.qoderworkcn/skills/ksw-inspired-fitness\
```

Restart QoderWork. The skill auto-loads when you mention fitness topics.

重启 QoderWork，提到健身话题时自动加载。

> Folder name must match the `name` field in SKILL.md (`ksw-inspired-fitness`).
> 文件夹名必须与 SKILL.md 的 `name` 字段一致。
</details>

<details>
<summary><b>Claude (Projects)</b></summary>

1. Open a Claude Project → **Project Settings** → **Project Instructions**
2. Paste the content of `SKILL.md` as project instructions
3. Upload `exercise-library.md`, `muscle-synergy.md`, `injury-substitutions.md`, `exercise-library-expanded.md`, `programming-decision-tree.md` as **Project Knowledge** files

打开 Claude Project → **Project Settings** → **Project Instructions**，将 `SKILL.md` 内容粘贴为项目指令，其余 `.md` 文件上传为项目知识文件。
</details>

<details>
<summary><b>ChatGPT (Custom Instructions / GPTs)</b></summary>

**Custom Instructions:** Paste the content of `SKILL.md` into your Custom Instructions.

**GPTs:** Upload all `.md` files as Knowledge in your GPT configuration.

将 `SKILL.md` 内容粘贴到自定义指令中，或将所有 `.md` 文件上传为 GPT 知识文件。
</details>

<details>
<summary><b>Other AI Agents / 其他 AI 工具</b></summary>

Use `SKILL.md` as a **system prompt** or context document. The reference files (`exercise-library.md`, `muscle-synergy.md`, etc.) can be loaded as RAG knowledge or appended to the prompt as needed.

将 `SKILL.md` 用作系统提示词或上下文文档，其余文件按需加载为知识库。
</details>

---

## Usage Examples / 使用示例

Once loaded into your AI tool, just chat naturally:

加载到你的 AI 工具后，直接用自然语言对话即可：

| You say / 你说 | AI does / AI 做 |
|------|------|
| "帮我排个减脂计划" | Generates a full training + carb cycling plan / 生成完整的训练+碳循环方案 |
| "我肩膀疼，还能练什么？" | Checks injury substitutions, suggests safe alternatives / 查伤病替代方案，推荐安全动作 |
| "卧推怎么做？" | Provides step-by-step form cues and common mistakes / 提供详细的动作要领和常见错误 |
| "碳循环怎么算？" | Explains the formula and generates a personalized meal plan / 解释计算公式，生成个性化饮食方案 |
| "练完背二头很酸正常吗？" | Explains muscle synergy — biceps are indirect movers in all pulling exercises / 解释肌肉协同——二头是所有拉类动作的辅助肌 |

---

## Data Sources / 数据来源

| Source | Description |
|------|------|
| **凯圣王 Douyin/Bilibili** | Training methodology, exercise cues, carb cycling formulas, warm-up protocols / 训练方法论、动作要领、碳循环公式、热身方案 |
| **[ExerciseDB Dataset](https://github.com/hasaneyldrm/exercises-dataset)** | 1,324 exercises with muscle synergy data (target, synergist, secondary muscles) and Chinese instructions / 1,324个动作的肌肉协同数据和中文指导 |
| **Baidu Baike** | Biographical information / 人物背景信息 |
| **Community notes (SMZDM, Zhihu, Bilibili)** | User-generated training logs and summaries / 用户整理的训练笔记 |

---

## Knowledge Architecture / 知识架构

This skill covers four layers of fitness coaching knowledge:

本技能覆盖健身教练知识的四个层次：

1. **Muscle Synergy** — Which muscles are indirectly fatigued by each exercise (data-driven, from 1,324 exercises) / **肌肉协同** — 每个动作间接消耗哪些肌群（数据驱动）
2. **Split Logic** — Why Push/Pull/Legs works, optimal arrangement, recovery intervals / **分化逻辑** — 推拉腿为什么有效、最优排列、恢复间隔
3. **Exercise Sequencing** — Which combinations synergize (1+1>2) vs. interfere / **动作编排** — 哪些组合协同增强、哪些互相干扰
4. **Individual Adaptation** — Injury substitutions, experience-based progressions, goal-specific adjustments / **个体适配** — 伤病替代、经验分级进阶、目标定制调整

---

## Content Attribution / 内容来源说明

This skill is **inspired by** 凯圣王's teaching methodology, but is not exclusively his content. Here's the breakdown:

本技能的**核心方法论**来自凯圣王的教学体系，但并非全部内容都源自他。具体构成如下：

| Source / 来源 | Proportion / 占比 | Content / 内容 |
|------|------|------|
| **凯圣王's methodology** | ~25-35% | 3-split training system, carb cycling formulas (223 method), 3-stage warm-up, training philosophy, posture correction, exercise cues from his videos / 三分化训练体系、碳循环223公式、三阶段热身、训练理念、体态纠正、视频中的动作要领 |
| **[ExerciseDB Dataset](https://github.com/hasaneyldrm/exercises-dataset)** | ~45-55% | 1,324 exercises with muscle synergy data, injury-safe substitutions, expanded exercise library with Chinese instructions / 1,324个动作的肌肉协同数据、伤病替代方案、扩展动作库 |
| **General exercise science** | ~15-25% | Programming logic, progressive overload principles, split arrangement theory, recovery protocols / 训练编排逻辑、渐进超负荷原则、分化排列理论、恢复方案 |

> **Note / 说明:** 凯圣王's content forms the **soul** of this skill — his unique training philosophy, diet system, and methodology distinguish it from generic fitness apps. The ExerciseDB data and exercise science knowledge provide the **backbone** that makes the coaching logic work.
>
> 凯圣王的内容是这个技能的**灵魂** —— 他独特的训练理念、饮食体系和方法论是区别于通用健身工具的关键。ExerciseDB 数据和通用运动科学知识则提供了让教练逻辑运转的**骨架**。

---

## Contributing / 贡献

This skill is a living document. If you watch 凯圣王's videos and find new techniques, cues, or principles not yet covered, feel free to submit a PR!

这个技能是持续更新的。如果你在看凯圣王视频时发现了尚未收录的新技巧、要领或原则，欢迎提交 PR！

Areas especially welcome:
- More exercise form cues from his video content / 更多视频中的动作要领
- Specific case studies or client examples / 具体案例或学员反馈
- Advanced periodization methods / 进阶周期化方法
- Rehabilitation-specific protocols / 康复专项方案

---

## License / 许可

MIT License. The exercise data originates from [ExerciseDB v1](https://oss.exercisedb.dev). The fitness methodology are based on publicly available content by 凯圣王.

MIT 许可证。动作数据来源于 [ExerciseDB v1](https://oss.exercisedb.dev)。健身方法论基于凯圣王公开发布的教学内容。

---

## Acknowledgments / 致谢

- [凯圣王](https://www.douyin.com/user/MS4wLjABAAAAjnKGbRiPmA8tqEn8WAWSqr89M7HQhpxsJdXdgM6bebf2c9pxX4GRBWG9I6GmppEA) — Original fitness methodology / 原始健身教学方法
- [谭成义](https://www.douyin.com/zhuanti/7626152142012811310) — Co-developer of the Functional 3-Split System / 功能性三分化训练体系联合开发者
- [ExerciseDB Dataset](https://github.com/hasaneyldrm/exercises-dataset) — 1,324 exercises with multilingual instructions / 1,324个多语言动作数据
- [QoderWork](https://docs.qoder.com/qoderwork/introduction) — One of the supported platforms for this skill / 本技能支持的平台之一
