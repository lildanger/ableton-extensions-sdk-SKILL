# Danjuan Ableton Extension Skill

**Danjuan Ableton Extension Skill** 是一套专为 **大模型 AI 助手** 定制的系统级技能（System Prompt/Skill），旨在赋能 AI 成为一名**无代码 Ableton Live 插件开发专家**。

通过引入本技能，搭载 AI 的任何开发助手都能完美跨越技术壁垒，让完全不懂编程的**音乐人**仅凭自然语言沟通，即可在几分钟内构建出专属的 Ableton Extensions 插件，并一键完成离线编译打包与极简交付。

## 🎯 核心使命

隐藏一切晦涩的底层技术细节（如 TypeScript, esbuild, package.json, Transaction 事务等），将原本面向程序员的 Ableton Extensions SDK 开发工作转化为极度友好的音乐术语交流流程。AI 负责包揽从初始化、代码生成到编译打包的全链路，为音乐人提供“零门槛、零调试、即插即用”的神级开发体验。

## ✨ 主要特色

- **零代码音乐人交互规范**
  - AI 严格禁用开发专业词汇，全方位采用音乐术语（如：“音轨”、“剪辑槽（ClipSlot）”、“时间选区”）与用户对话。
  - 标准化的三阶段互动模型：**【第 1 阶段：需求共创】 -> 【第 2 阶段：后台静默开发】 -> 【第 3 阶段：极简交付部署】**。
- **环境安全预检机制**
  - **第 0 阶段**：在接受需求前，系统会自动检测工作区是否包含官方的 `extensions-sdk`，避免因环境问题导致的后续开发与打包失败。
- **全自动离线编译打包**
  - 技能内包含完美的离线依赖引用的 `package.json` 模板与包含了 HTML Text Loader 的 `build.ts` esbuild 构建方案，断网也能在后台飞速完成出包。
- **严格沉淀的 SDK 防错规约**
  - 自身包含了极其详细的 API 最佳实践（ContextMenuScope 映射全覆盖、Handle 强类型安全转换、Progress 对话框长任务调用范式等）。
  - **Transaction 同步铁律**：从源头屏蔽了大模型生成插件代码时常犯的“事务块内 await”等致命错误。
  - **模态弹窗通信规范**：内建兼容 macOS/Windows (WebView2) 宿主的 Webview 注入与闭环通信标准。

## 🚀 如何使用

1. **装载技能**：将本仓库中的 `SKILL.md` 注入为您的 AI 助手的 System Prompt（系统指令），或者将其添加至智能体（Agent）的专有技能库。
2. **准备环境**：将 Ableton 官方提供的包含 `extensions-sdk` 名称的文件夹或相关 `.tgz` 依赖压缩包放置于当前的协作开发目录中。
3. **发起对话**：对 AI 说：“*我想做一个能够在右键选中 Clip 时，一键将其切换为 Complex Pro 模式的插件！*”
4. **获取插件**：跟随 AI 亲切无痛的引导，您只需拿到最终它为您在后台打包好的 `.ablx` 文件，将其拖入 Ableton Live -> Preferences -> Extensions 页面中，大功告成！

## 📄 文件构成

- `SKILL.md`: 核心的系统级智能体技能说明文档，全面规定了交互语言、构建模板以及 SDK 开发的铁律规则。
- `README.md`: 本项目的使用介绍说明（当前文件）。
