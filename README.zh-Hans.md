<div align="center">

<img src="https://raw.githubusercontent.com/ryekee/RuaKey-releases/main/docs/dashboard.png" width="820" alt="RuaKey dashboard" />

# ⌨️ RuaKey

**一款隐私优先的 macOS 键盘统计 App。**
*见你所键，不窥你所言*

[![Download latest](https://img.shields.io/github/v/release/ryekee/RuaKey-releases?label=Download&style=for-the-badge&color=fab387)](https://github.com/ryekee/RuaKey-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/ryekee/RuaKey-releases/total?label=downloads&style=for-the-badge&color=a6e3a1)](https://github.com/ryekee/RuaKey-releases/releases)

macOS 15+ · Apple Silicon 与 Intel · 常驻菜单栏

[English](README.md) | 简体中文 | [繁體中文](README.zh-Hant.md) | [日本語](README.ja.md)

</div>

---

RuaKey 把你的键盘（和鼠标）活动变成清晰、**只存于本机**的统计：你打字有多快、最依赖哪些键和快捷键、击键都花在哪些 app 上，以及这一切随时间的走势。

它只统计**元数据**——按键类别、每键计数、修饰键组合——全部**按天聚合**。它从不保存击键的顺序或时序，因此在物理上**无法重建你输入的任何文本**。

## 🔒 隐私就是全部

- **你的输入永不离开这台 Mac**。没有遥测、没有分析 SDK、没有云同步。
- **绝不记录击键内容**——只有类别和每日每键计数，从不保存（时间，键）序列。
- **按物理键盘统计**，基于 Apple 的 `IOHIDManager`——数据按设备分组，而不是从系统级事件流里捞取。
- App *唯一*的联网行为是向 GitHub 检查更新——而且可以关掉。

> 存储的数据库里没有任何文本字段。从每日类别计数里根本无法还原出词句。

## ✨ 你会得到什么

- **📊 仪表盘**——今日 / 7 天 / 30 天 / 累计总量、实时与峰值 KPM、删除率、连续活跃天数、时段与星期分布，以及全年活动日历。
- **⌨️ 键盘热力图**——把你最常按的键画在一块真实键盘上，多种配列可选：**MacBook · 75% · TKL · Alice · HHKB**。
- **🖱️ 鼠标**——点击与滚动计数，以及平滑的按屏幕点击热力图（坐标在采集时即被量化——原始位置从不落盘）。
- **📱 按应用**——你的击键和点击都花在哪些 app 上。
- **📈 7 日对比**——每项数据都给出今天与最近 7 天的对照。
- **🎉 里程碑彩带**——刷新 7 日纪录时的全屏庆祝。
- **🌐 四种语言**——English、简体中文、繁體中文、日本語。
- **🔄 自动更新**——新版本自动完成安装。

一切都在深色的终端 / 仪表盘美学里——琥珀与绿、Departure Mono、高密度的机器读数面板。

## 📊 数据，两种看法

<img src="https://raw.githubusercontent.com/ryekee/RuaKey-releases/main/docs/popover.png" align="right" width="300" alt="Menu bar popover" />

**主窗口**用来深挖——总量、速度、热力图、按应用拆解与长期趋势，都在一块终端风格的仪表盘上。

**菜单栏**用来一瞥：点一下图标，就能看到今天的击键与点击、峰值 KPM、删除率，以及最常用的键 / 组合键 / 键盘 / app——还有 HUD、KPM 模式与暂停的快捷开关——全程不必打开主窗口。

<br clear="all"/>

## 🎚️ 实时 HUD

一条小小的悬浮条，浮在你手头的任何工作之上——**实时 KPM**、**刚按下的键**、**今日累计**，随你的敲击实时更新：

<div align="center">
<img src="https://raw.githubusercontent.com/ryekee/RuaKey-releases/main/docs/hud.gif" width="600" alt="RuaKey live HUD" />
</div>

- 开始打字的瞬间**自动出现**，空闲时**淡出**。
- **会躲开光标**——光标一靠近就自动让开，绝不挡住下面的内容（可在设置里关闭）。
- 可固定在屏幕六个位置之一，空闲超时可调。
- **按自己的习惯来**——各模块可显示、隐藏、拖拽排序，还有一只随 KPM 升高越敲越快的**打字猫**。

## 📥 安装

1. **[下载最新的 `.dmg`](https://github.com/ryekee/RuaKey-releases/releases/latest)**，把 **RuaKey** 拖进「应用程序」。
2. 首次启动：**右键 → 打开**以通过 Gatekeeper（App 为 ad-hoc 签名，未经公证）。
3. 按提示授予**输入监听**权限，然后**退出并重启**——macOS 要求重启 App 才能生效。

0.3 之后，更新会自动完成安装。一个注意点：由于 App 是 ad-hoc 签名（未经公证），更新后 macOS 可能会忘记**输入监听**授权——**设置 ▸ 隐私**里有一步到位的恢复指引。

---

<div align="center">
<sub>RuaKey 只记录次数，不记录内容。你的文字只属于你。</sub>
</div>
