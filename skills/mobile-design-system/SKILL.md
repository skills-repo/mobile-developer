---
name: mobile-design-system
description: 移动端设计规范：平台适配、触控交互、手势、动效、无障碍
source:
  type: original
  repo: skills-repo/mobile-developer
  path: skills/mobile-design-system/SKILL.md
  version: 1.0.0
  updated: 2026-07-26
metadata:
  category: 设计
  platform: Mobile
  difficulty: 进阶
---

# 移动端设计规范

> 为移动应用制定和实现设计规范，覆盖 iOS/Android 平台差异、触控交互、手势和动效。

## 能力

- **平台适配**：Material Design 3 vs Human Interface Guidelines 差异对照
- **触控交互**：点击区域、手势冲突、触觉反馈（Haptics）
- **手势设计**：滑动、长按、捏合、拖拽的手势规范与实现
- **动效设计**：转场动画、微交互、加载状态、骨架屏
- **无障碍设计**：色彩对比度、可缩放文字、屏幕阅读器适配

## 使用方式

```
/mobile-design-system 为我的应用制定一套移动端设计规范
/mobile-design-system 这个页面在 iOS 和 Android 上表现不一致，帮我统一
/mobile-design-system 设计一个符合 HIG 的下拉刷新动效
```

## 工作流

1. 描述应用类型和目标用户群
2. AI 分析 iOS/Android 平台差异需求
3. 生成设计规范文档（色彩/字体/间距/圆角/阴影）
4. 输出关键交互的动效规格（时长/曲线/触发条件）
5. 提供无障碍检查清单

## 适用场景

- 从零建立移动端设计规范
- iOS/Android 平台一致性审查
- 手势交互方案设计
- 动效规范制定

## 限制

- 不涉及设计工具（Figma/Sketch）的具体操作
- 不涉及品牌视觉设计（Logo/插画/品牌色）
- 复杂动效实现建议配合 flutter-builder 或 react-native-builder