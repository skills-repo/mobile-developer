# AGENTS.md — mobile-developer 入口文件

> mobile-developer 仓库的 Agent 入口文件，定义移动端开发技能库的使用规则。

## 触发条件

Agent 在以下场景加载本文件：

1. 用户请求移动端应用开发相关任务
2. 用户提到 Flutter、React Native、iOS 或移动端设计
3. 用户请求跨平台或原生移动端功能实现

## 技能清单

| 技能 | 文件 | 用途 |
|------|------|------|
| flutter-builder | skills/flutter-builder/SKILL.md | Flutter Widget、状态管理、响应式布局 |
| react-native-builder | skills/react-native-builder/SKILL.md | React Native 组件、导航、Expo |
| ios-developer | skills/ios-developer/SKILL.md | SwiftUI、Core Data、辅助功能 |
| mobile-design-system | skills/mobile-design-system/SKILL.md | 平台设计规范、手势交互、动效 |

## 行为规则

- 所有技能面向独立开发者/小团队，不涉及企业级移动端架构
- 优先推荐跨平台方案（Flutter/React Native），iOS 原生作为补充
- 移动端设计需同时考虑 iOS 和 Android 平台差异

## 不做什么

- 不涉及 Android 原生（Kotlin/Jetpack Compose）开发 — 可后续补充
- 不涉及移动端游戏开发 — 归属 indie-game-developer
- 不涉及移动端安全测试 — 归属 security-guardian