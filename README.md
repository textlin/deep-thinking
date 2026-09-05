## deep-thinking · 深度思考引导技能
通过层层审慎的递进式提问，帮助你理清问题或决策背后的本质脉络，挖掘隐藏假设、明确真实目标、权衡潜在代价，最终自己得出答案。当你被想法、决策与困惑困住，难以做出判断、不知如何推进时，不妨体验这款技能。

> Guide a user through careful questioning that helps them uncover the underlying shape of a problem or decision.When you are stuck with ideas, decisions or puzzles and struggle to judge or move forward, give this skill a try.

本项目同时提供 **Codex 技能文件** 。

## ✨ 核心特性
- **苏格拉底式引导**：不直接给出结论，通过精准提问推动你自主思考
- **分层递进逻辑**：从澄清问题 → 拆分事实 → 挖掘假设 → 溯源本质，逐层深入
- **少而精的提问**：每轮只问少量问题，每个问题只完成一个思考目标
- **情绪友好适配**：面对情绪化话题先复述梳理，再平稳推进，不说教、不武断
> ## ✨ Core Features
> - **Socratic Guidance**: Instead of giving direct answers, it drives you to think independently through targeted questions.
> - **Hierarchical Progressive Logic**: Dig deeper step‑by‑step: clarify the problem → break down facts → uncover assumptions → trace back to > the essence.
> - **Concise Questioning**: Only a small number of questions per round, with each question serving one single thinking goal.
> - **Emotion‑friendly Adaptation**: Restate and sort out emotional topics first before moving forward calmly, without preaching or arbitrary > judgment.
-  **Dual‑platform Compatibility**: Supports both the Codex skill system and Doubao custom assistants.


## 📦 项目结构
```
deep-thinking/
├── SKILL.md          # Codex 标准技能文件（YAML 头部 + 执行逻辑）
├── agents/
│   └── openai.yaml   # 可选：技能展示元数据
└── README.md         # 项目说明与使用指南
```

## 🚀 快速开始

### 方式一：在 Codex 中使用
1. **创建技能目录**
   在 Codex 技能目录下新建文件夹，推荐使用全局路径：
   ```bash
   mkdir -p ~/.codex/skills/deep-thinking
   ```
   也可仅在单个项目中生效，在项目根目录创建 `.codex/skills/deep-thinking/`。

2. **放入技能文件**
   将仓库中的 `SKILL.md` 复制到上述目录中。
   > ⚠️ 注意：文件名必须保持全大写 `SKILL.md`，否则无法被识别。

3. **生效与测试**
   重启 Codex 或新建会话，系统会自动扫描并加载技能。
   输入一个需要思考的问题（如「帮我深度思考要不要换工作」），如果 AI 开始反问你的目标、顾虑、约束条件而非直接给结论，即为触发成功。


## 💡 使用示例
```
用户：我要不要辞职去创业？

deep-thinking：
1. 你现在想辞职的核心原因是什么？是对现状不满，还是被创业的某个机会吸引？
2. 你心目中的“创业成功”，具体是指达到什么状态？
3. 如果尝试创业但没有达到预期，你能接受的底线是什么？
```

## 🧠 引导逻辑框架
技能默认遵循四层思考递进路径：
1. **澄清层**：锁定真实问题，区分事实、感受与观点
2. **拆解层**：拆分问题要素，暴露隐含的前提与约束
3. **溯源层**：追问底层动机与第一性原则
4. **复盘层**：总结已有结论，标记剩余开放问题

## ⚙️ 自定义调整
- **修改触发词**：编辑 `SKILL.md` 顶部 YAML 中的 `trigger.patterns`，添加你习惯的触发语
- **调整提问风格**：修改正文的风格描述，可切换为更犀利、更温和或更偏向商业分析的语气
- **增加专用场景**：可基于核心逻辑扩展出「决策复盘」「创意发散」「自我反思」等专用分支

## 📄 许可证
MIT License - 可自由使用、修改与分发。

## 🤝 贡献
欢迎提交 Issue 或 PR 来优化引导逻辑、补充更多平台适配版本。
