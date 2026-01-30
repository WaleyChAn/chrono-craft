# CLAUDE.md

本文件为 Claude Code (claude.ai/code) 提供项目指导。

---

## 项目信息

**项目名称**: ChronoCraft (数字时钟)

**项目描述**: 基于 Raspberry Pi + 废弃笔记本显示器的可定制、可交互的智能数字时钟系统

**核心特性**:

- 时钟显示（12/24小时制、圆盘样式、农历）
- 天气信息（和风天气 API）
- 动态背景（日夜自动切换）
- 屏幕方向控制（横向/竖向，支持重力感应）
- 闹钟、倒计时、番茄钟
- 自定义小组件

**硬件规格**:

- Raspberry Pi 4B (4GB)
- 联想小新13Pro 屏幕 (2560×1600, 2.5K, IPS)
- 电池供电 + WiFi 连接
- 可选重力感应传感器 (MPU6050)

---

## 文档语言规范

**重要**: 本项目所有文档（PRD、Spec、设计文档、注释等）**必须使用中文编写**。

例外情况：

- 代码文件中的变量名、函数名使用英文
- API 端点路径使用英文
- 配置文件（YAML/JSON）的键名使用英文

---

## 开发工作流

本项目采用 SpecKit (SDD) + Pencil.dev 工作流：

1. **PRD** (`prd/prd.md`) → 产品需求文档（中文）✅ 已完成
2. **Spec** → 使用 `speckit.specify` 生成规格文档（中文）⏳ 待执行
3. **Design** → 使用 Pencil 在 `design/` 创建 UI 设计 ⏳ 待执行
4. **Plan** → 使用 `speckit.plan` 生成实施计划（中文）⏳ 待执行
5. **Tasks** → 使用 `speckit.tasks` 生成任务列表（中文）⏳ 待执行
6. **Implement** → 使用 `speckit.implement` 执行实施 ⏳ 待执行

---

## Pencil 工具使用规范

当使用 Pencil MCP 工具时：

- 使用 `mcp__pencil__get_editor_state` 了解当前活动文件
- 使用 `mcp__pencil__open_document` 打开或创建 `.pen` 文件
- 使用 `mcp__pencil__batch_get` 读取 `.pen` 文件内容
- 使用 `mcp__pencil__batch_design` 进行设计操作
- **禁止**使用 Read 或 Grep 工具读取 `.pen` 文件

---

## 技术栈

| 层级   | 技术                    |
| ------ | ----------------------- |
| 前端   | SvelteKit + TailwindCSS |
| 后端   | Node.js (Express)       |
| 部署   | PM2 + Kiosk Mode        |
| 设计   | Pencil.dev (.pen)       |
| 工作流 | SpecKit (SDD)           |

---

## PRD 当前状态

| 章节       | 状态                    |
| ---------- | ----------------------- |
| 项目概述   | ✅ 完成                 |
| 功能清单   | ✅ 完成                 |
| 用户故事   | ✅ 完成                 |
| 功能需求   | ✅ 完成                 |
| 非功能需求 | ✅ 完成                 |
| 硬件规格   | ✅ 完成                 |
| 软件架构   | ✅ 完成                 |
| 约束与限制 | ✅ 完成                 |
| 风险与应对 | ✅ 完成                 |
| 里程碑     | ✅ 完成（并行开发模式） |
| 附录       | ✅ 完成                 |

**版本**: v0.2
**状态**: 待用户确认后定稿

---

## 下一步

1. 使用 `speckit.specify` 生成技术规格文档
2. 使用 Pencil 设计主页面原型
3. 搭建 SvelteKit 项目框架
