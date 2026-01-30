# ChronoCraft

> 基于 Raspberry Pi + 废弃笔记本屏幕的可定制、可交互智能数字时钟系统

---

## 项目简介

ChronoCraft 是一款功能完整的桌面数字时钟系统，利用废弃的笔记本屏幕和树莓派打造，提供美观、实用的时钟显示和信息服务。

### 核心特性

- **时钟模块**: 12/24小时制、圆盘样式、农历显示（含节日/节气）
- **天气信息**: 和风天气 API，显示当前天气和未来 2-3 天预报
- **动态背景**: 根据日出日落自动切换日夜主题
- **屏幕方向**: 横向/竖向切换，支持重力感应自动切换
- **实用工具**: 闹钟、倒计时器、番茄钟
- **自定义小组件**: 动态像素小人、信息轮播

---

## 硬件规格

| 组件 | 规格 |
| --- | --- |
| 主控板 | Raspberry Pi 4B (4GB) |
| 屏幕 | 联想小新13Pro, 2560×1600 (2.5K), 16:10, IPS |
| 驱动板 | HDMI 转 eDP，12V 供电 |
| 重力感应 | MPU6050/MPU9250（可选） |
| 电池 | 18650×3, 5000mAh+, 11.1V |
| 连接 | WiFi 无线网络 |

---

## 技术栈

| 层级   | 技术                    |
| ------ | ----------------------- |
| 前端   | SvelteKit + TailwindCSS |
| 后端   | Node.js (Express)       |
| 部署   | PM2 + Kiosk 模式        |
| 设计   | Pencil.dev (.pen)       |
| 工作流 | SpecKit (SDD)           |

---

## 开发工作流

本项目采用 SpecKit (SDD) + Pencil.dev 工作流：

```text
PRD → Spec → Design → Plan → Tasks → Implement
```

当前进度：

| 阶段 | 状态 |
| --- | --- |
| PRD | ✅ 已完成 |
| Spec | ⏳ 待执行 |
| Design | ⏳ 待执行 |
| Plan | ⏳ 待执行 |
| Tasks | ⏳ 待执行 |
| Implement | ⏳ 待执行 |

---

## 项目文档

- **PRD**: [prd/prd.md](prd/prd.md) - 产品需求文档 v0.2
- **项目指令**: [CLAUDE.md](CLAUDE.md) - Claude Code 项目指导

---

## 许可证

[License](LICENSE)
