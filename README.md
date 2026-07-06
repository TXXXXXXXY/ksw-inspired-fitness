# KSW Fitness Coach Skill / 凯圣王健身教练 Skill

<div align="center">

**A QoderWork Agent Skill that turns AI into a professional fitness coach, based on the teaching methodology of [凯圣王 (Kai Sheng Wang)](https://www.douyin.com/user/MS4wLjABAAAAjnKGbRiPmA8tqEn8WAWSqr89M7HQhpxsJdXdgM6bebf2c9pxX4GRBWG9I6GmppEA), a top Chinese fitness educator with 1M+ followers.**

**一个基于抖音百万粉丝健身博主凯圣王教学体系的 QoderWork 智能体技能，让 AI 变身专业健身教练。**

[![Skill Files](https://img.shields.io/badge/Skill_Files-6-blue)](#-file-structure)
[![Exercises](https://img.shields.io/badge/Exercise_DB-1324-green)](#-data-sources)
[![QoderWork](https://img.shields.io/badge/Platform-QoderWork-orange)](https://docs.qoder.com/qoderwork/introduction)
[![Languages](https://img.shields.io/badge/Languages-CN%20%7C%20EN-yellow)](#-overview)

</div>

---

## What This Does / 这是什么

This is a **QoderWork Agent Skill** — a structured knowledge package that teaches AI how to coach fitness like a professional trainer. Once installed, the AI can:

这是一个 **QoderWork 智能体技能** —— 一套结构化的健身知识包，教会 AI 像专业教练一样指导训练。安装后，AI 可以：

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

### Prerequisites / 前提条件

- [QoderWork](https://docs.qoder.com/qoderwork/introduction) desktop app installed

### Steps / 步骤

1. Download or clone this repository
2. Copy the entire folder to your QoderWork skills directory:

```
# Windows
%USERPROFILE%\.qoderworkcn\skills\ksw-fitness-skill\

# macOS / Linux
~/.qoderworkcn/skills/ksw-fitness-skill/
```

3. Restart QoderWork — the skill will auto-load when you mention fitness-related topics
4. 重启 QoderWork，当你提到健身相关话题时，技能会自动加载

---

## Usage Examples / 使用示例

Once installed, just chat naturally. The skill activates automatically when you mention fitness topics:

安装后，直接用自然语言对话即可。提到健身话题时技能自动激活：

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
- [QoderWork](https://docs.qoder.com/qoderwork/introduction) — The platform that makes this skill possible / 支撑此技能运行的平台
