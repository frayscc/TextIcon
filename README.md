<div align="center">

# ✦ TextIcon

**灵动、极简且纯前端驱动的文字与汉字图标生成工坊**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Pure Frontend](https://img.shields.io/badge/Stack-HTML5%20%7C%20Canvas%20%7C%20JS-brightgreen)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Platform](https://img.shields.io/badge/Platform-Web%20%7C%20Cross--Platform-lightgrey)](#)
[![No Dependencies](https://img.shields.io/badge/Dependencies-Zero%20Backend-orange)](#)

[快速上手](#-快速上手) · [功能特性](#-功能特性) · [排版规则](#️-排版规则说明) · [开源协议](#-开源协议)

</div>

---

## 📖 简介 (Introduction)

**TextIcon** 是一款专为中文文本、学科标签与个性化字标设计的轻量级图标生成工具。采用 Apple 风格的拟态毛玻璃与大圆角设计语言，纯前端单页架构。

无需安装 Python、Node.js 或任何运行环境，**双击单个 HTML 文件即可在现代浏览器中即开即用**，支持批量导出 Windows 标准 `.ico` 图标及 `.zip` 压缩包。

---

## ✨ 功能特性 (Features)

- **🧩 智能汉字排版引擎**：
  - **单字**：200px 巨幅居中排版，大气醒目。
  - **双字 / 三字**：采用多倍宽画幅渲染后非等比横向压缩（压扁紧凑），字体饱满张力十足。
  - **四字**：经典田字格（2×2 网格）紧凑排布，规整平稳。
  - **多字自适应**：5 字及以上自动降级单行自适应缩放。
- **🍎 苹果级视觉质感 (Apple-inspired UI)**：
  - 多层动态渐变光晕背景、深度高斯模糊（Glassmorphism）、超椭圆圆角（Squircle）与细腻交互微动效。
- **🔤 深度字体生态**：
  - **内置中文字体优先**：预设微软雅黑、苹方、楷体、仿宋、宋体、黑体、隶书、幼圆等常用中文字体。
  - **字体直观预览**：下拉菜单项直接以对应字形渲染“永”字，所见即所得。
  - **扫描本机系统字体**：支持通过 `Local Font Access API` 一键枚举加载系统已安装字体。
  - **自定义字体文件导入**：支持一键拖入 `.ttf` / `.otf` / `.woff2` 等外部字体文件（如霞鹜文楷等）。
- **🎨 精准色彩调节体系**：
  - 10 组精选色盘，支持实时明度（Brightness）与饱和度（Saturation）微调滑块。
  - 色卡随滑块调节实时变化，支持直接输入精准 RGB 色值。
- **📦 原生 ICO 打包与批量下载**：
  - 纯前端二进制流封装标准 Windows 256×256 规格的 `.ico` 图标。
  - 集成 JSZip 实现多词条一键打包为 `.zip` 导出。

---

## 🚀 快速上手 (Quick Start)

### 方式 1：直接双击运行（推荐）

1. 下载仓库中的 [`index.html`](index.html)。
2. 双击文件，即可在 Chrome、Edge、Safari 或 Firefox 等现代浏览器中打开使用。

### 方式 2：使用 Git 快速克隆

```bash
git clone https://github.com/your-username/TextIcon.git
cd TextIcon
# 在浏览器中直接打开 index.html 即可
```

### 方式 3：部署到静态网页托管

你可以直接将仓库部署至 **GitHub Pages**、**Vercel** 或 **Cloudflare Pages**：
- 进入仓库 `Settings` -> `Pages` -> 选择 `main` 分支作为部署源，即可快速获得公网在线工具站。

---

## 🛠️ 排版规则说明 (Typography Layout)

| 字数 | 排版示意 | 处理逻辑 |
| :---: | :---: | :--- |
| **1 字** | `[ 语 ]` | 200px 巨幅居中排版 |
| **2 字** | `[ 语文 ]` | 512×256 双倍宽画幅绘制后，压缩至 256×256 紧凑扁平化字形 |
| **3 字** | `[ 物理化 ]`| 768×256 三倍宽画幅绘制后，压缩至正方形，紧凑排列 |
| **4 字** | `[ 政治 / 历史 ]` | 2×2 田字格象限排布，精致紧凑 |
| **5+ 字** | `[ 综合实践活动 ]` | 自动降级为单行缩放自适应 |

---

## 🧭 浏览器支持 (Browser Compatibility)

| 浏览器特性 | Chrome / Edge | Safari | Firefox |
| :--- | :---: | :---: | :---: |
| 基础渲染 & ICO 打包 | ✅ 支持 | ✅ 支持 | ✅ 支持 |
| 外部 `.ttf` 字体导入 | ✅ 支持 | ✅ 支持 | ✅ 支持 |
| 扫描本机全部系统字体 | ✅ 支持 (需授权) | ⚠️ 依赖系统策略 | ⚠️ 依赖系统策略 |

> **提示**：如浏览器不支持系统字体枚举，可直接点击「导入 .ttf/.otf 字体文件」选入本地字体使用。

---

## 📄 开源协议 (License)

本项目基于 [MIT License](LICENSE) 协议开源。

---

<div align="center">
  <sub>Designed with craftsmanship by <b>fray</b></sub>
</div>
