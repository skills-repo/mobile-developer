---
name: flutter-builder
description: Flutter 分层架构（UI/Logic/Data）、MVVM 模式、项目结构、响应式布局
source:
  type: derived
  repo: skills-repo/mobile-developer
  path: skills/flutter-builder/SKILL.md
  version: 1.0.0
  updated: 2026-07-26
  url: https://skills.sh/flutter/skills/flutter-apply-architecture-best-practices
metadata:
  category: 跨平台
  platform: Mobile
  difficulty: 进阶
---

# Flutter 架构与布局

> 使用 Flutter 推荐的分层架构（UI/Logic/Data）和响应式布局模式构建可扩展的跨平台应用。

## 能力

- **分层架构**：UI 层（MVVM）、Logic 层（UseCase）、Data 层（Repository/Service）分离
- **响应式布局**：LayoutBuilder + constraints.maxWidth 自适应，不锁屏幕方向
- **项目结构**：按功能分组的 UI + 按类型分组的 Data/Domain 混合组织
- **状态管理**：ViewModel 继承 ChangeNotifier，暴露不可变状态快照
- **大屏优化**：ConstrainedBox 限制宽度、Expanded/Flexible 分配空间、ListView.builder 懒渲染

## 使用方式

```
/flutter-builder 为我的应用设计分层架构和项目目录结构
/flutter-builder 这个页面需要适配手机和平板，帮我写响应式布局
/flutter-builder 重构这个 Widget，把业务逻辑从 UI 层抽到 ViewModel
```

## 工作流

1. 识别需要自适应行为的 Widget
2. 用 LayoutBuilder 包裹，提取 constraints.maxWidth
3. 定义断点（如 largeScreenMinWidth = 600）
4. maxWidth > 断点 → 返回大屏布局（Row + 侧栏）
5. maxWidth ≤ 断点 → 返回小屏布局（Column 或标准导航）

## 适用场景

- 新 Flutter 项目架构搭建
- 已有项目重构为分层架构
- 手机→平板→桌面多屏幕适配
- ViewModel/Repository 模式迁移

## 限制

- 不涉及 Flutter 引擎和原生插件开发
- 不涉及设计稿到代码的自动转换
- 复杂动画建议配合 design-studio 的 motion-design