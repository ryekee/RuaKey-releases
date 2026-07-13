<div align="center">

<img src="https://raw.githubusercontent.com/ryekee/RuaKey-releases/main/docs/zht-dashboard.png" width="820" alt="RuaKey dashboard" />

# ⌨️ RuaKey

**一款隱私優先的 macOS 鍵盤統計 App。**
*見你所鍵，不窺你所言*

[![Download latest](https://img.shields.io/github/v/release/ryekee/RuaKey-releases?label=Download&style=for-the-badge&color=fab387)](https://github.com/ryekee/RuaKey-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/ryekee/RuaKey-releases/total?label=downloads&style=for-the-badge&color=a6e3a1)](https://github.com/ryekee/RuaKey-releases/releases)

macOS 15+ · Apple Silicon 與 Intel · 常駐選單列

[English](README.md) | [简体中文](README.zh-Hans.md) | 繁體中文 | [日本語](README.ja.md)

</div>

---

RuaKey 把你的鍵盤（和滑鼠）活動變成清晰、**只存於本機**的統計：你打字有多快、最依賴哪些鍵和快捷鍵、擊鍵都花在哪些 app 上，以及這一切隨時間的走勢。

它只統計**元資料**——按鍵類別、每鍵計數、修飾鍵組合——全部**按天彙總**。它從不保存擊鍵的順序或時序，因此在物理上**無法重建你輸入的任何文字**。

## 🔒 隱私就是全部

- **你的輸入永不離開這台 Mac**。沒有遙測、沒有分析 SDK、沒有雲端同步。
- **絕不記錄擊鍵內容**——只有類別和每日每鍵計數，從不保存（時間，鍵）序列。
- **按實體鍵盤統計**，基於 Apple 的 `IOHIDManager`——資料按裝置分組，而不是從系統級事件流裡撈取。
- App *唯一*的連網行為是向 GitHub 檢查更新——而且可以關掉。

> 儲存的資料庫裡沒有任何文字欄位。從每日類別計數裡根本無法還原出詞句。

## ✨ 你會得到什麼

- **📊 儀表板**——今日 / 7 天 / 30 天 / 累計總量、即時與峰值 KPM、刪除率、連續活躍天數、時段與星期分布，以及全年活動日曆。
- **⌨️ 鍵盤熱力圖**——把你最常按的鍵畫在一塊真實鍵盤上，多種配列可選：**MacBook · 75% · TKL · Alice · HHKB**。
- **🖱️ 滑鼠**——點擊與滾動計數，以及平滑的按螢幕點擊熱力圖（座標在擷取時即被量化——原始位置從不落盤）。
- **📱 按應用**——你的擊鍵和點擊都花在哪些 app 上。
- **📈 7 日對比**——每項數據都給出今天與最近 7 天的對照。
- **🎉 里程碑彩帶**——刷新 7 日紀錄時的全螢幕慶祝。
- **🌐 四種語言**——English、简体中文、繁體中文、日本語。
- **🔄 自動更新**——新版本自動完成安裝。

一切都在深色的終端機 / 儀表板美學裡——琥珀與綠、Departure Mono、高密度的機器讀數面板。

## 📊 資料，兩種看法

<img src="https://raw.githubusercontent.com/ryekee/RuaKey-releases/main/docs/zht-popover.png" align="right" width="300" alt="Menu bar popover" />

**主視窗**用來深挖——總量、速度、熱力圖、按應用拆解與長期趨勢，都在一塊終端機風格的儀表板上。

**選單列**用來一瞥：點一下圖示，就能看到今天的擊鍵與點擊、峰值 KPM、刪除率，以及最常用的鍵 / 組合鍵 / 鍵盤 / app——還有 HUD、KPM 模式與暫停的快捷開關——全程不必打開主視窗。

<br clear="all"/>

## 🎚️ 即時 HUD

一條小小的懸浮條，浮在你手頭的任何工作之上——**即時 KPM**、**剛按下的鍵**、**今日累計**，隨你的敲擊即時更新：

<div align="center">
<img src="https://raw.githubusercontent.com/ryekee/RuaKey-releases/main/docs/v2-hud-darkbg.gif" width="600" alt="RuaKey live HUD" />
</div>

- 開始打字的瞬間**自動出現**，閒置時**淡出**。
- **會躲開游標**——游標一靠近就自動讓開，絕不擋住下面的內容（可在設定裡關閉）。
- 可固定在螢幕六個位置之一，閒置逾時可調。
- **按自己的習慣來**——各模組可顯示、隱藏、拖曳排序，還有一隻隨 KPM 升高越敲越快的**打字貓**。

## 📥 安裝

1. **[下載最新的 `.dmg`](https://github.com/ryekee/RuaKey-releases/releases/latest)**，把 **RuaKey** 拖進「應用程式」。
2. 首次啟動：**右鍵 → 打開**以通過 Gatekeeper（App 為 ad-hoc 簽名，未經公證）。
3. 依提示授予**輸入監控**權限，然後**結束並重啟**——macOS 要求重啟 App 才能生效。

0.3 之後，更新會自動完成安裝。一個注意點：由於 App 是 ad-hoc 簽名（未經公證），更新後 macOS 可能會忘記**輸入監控**授權——**設定 ▸ 隱私**裡有一步到位的恢復指引。

---

<div align="center">
<sub>RuaKey 只記錄次數，不記錄內容。你的文字只屬於你。</sub>
</div>
