<div align="center">

# 🎲 The Tale-Weaver's Dice
### 3D 故事骰子靈感寫作平台 (3D Story Dice Writing Platform)

[![License: MIT](https://img.shields.io/badge/License-MIT-ff69b4.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-Zero-success?style=for-the-badge)](#)

> **「轉動粉甜骰子，喚醒創作靈感。一鍵開啟無限想像的浪漫冒險！」**

[📖 專案介紹](#-專案介紹-introduction) •
[💡 緣由與動機](#-緣由與動機-motivation) •
[✨ 核心特色](#-核心特色-key-features) •
[🚀 開發歷程](#-開發歷程-development-journey) •
[📊 專案分析](#-專案分析與差異比較-project-analysis) •
[📦 快速開始](#-快速開始-quick-start)

</div>

---

## 📖 專案介紹 (Introduction)

**The Tale-Weaver's Dice** 是一款結合 **CSS 3D 擬真物理視角骰子** 與 **一站式創作畫布** 的網頁互動應用程式。透過隨機擲出的多面圖示組合與情境提示，協助小說創作者、語文教育工作者、桌遊（TRPG）玩家以及腦力激盪團隊，在數秒內打破思維僵局，建構出充滿驚喜的故事劇情轉折。

---

## 💡 緣由與動機 (Motivation)

在寫作教學、創意發想或日常創作的過程中，「面對空白畫面的靈感枯竭」是許多創作者最常遭遇的痛點。傳統的實體故事骰子（Story Cubes）雖然能激發聯想，卻受限於**攜帶不便、圖案無法修改、缺乏即時文字記錄工具**；而市面上的線上隨機抽卡工具多半僅為生硬的 2D 圖片切換，缺乏互動的溫度與儀式感。

本專案基於以下三大核心動機而誕生：

1. **賦予數位工具「實體儀式感」**：運用原生 CSS 3D 立體空間變換與 Web Audio API 程式化合成音效，模擬真實骰子在桌面滾動碰撞的聽覺與視覺體驗。
2. **打造「靈感至產出」的無縫閉環**：將擲骰器、關鍵字意涵解析（Hint）與文字編輯器整合於同一視窗，實現「擲骰 ➔ 聯想 ➔ 撰寫 ➔ 匯出」的流暢工作流。
3. **極致輕量與零門檻分享**：採用單一 HTML 檔案架構（Single-File Architecture），無需後端伺服器或繁瑣的環境安裝，任何人透過瀏覽器即可秒開即玩。

---

## ✨ 核心特色 (Key Features)

* 🎲 **CSS 3D 立體旋轉引擎**：支援 1 至 4 顆骰子同時獨立或一鍵滾動，具備多圈翻轉與擬真減速動畫。
* 🔊 **Web Audio 原生合成音效**：無需載入任何外部 `.mp3` 音訊檔案，透過瀏覽器底層音訊介面即時生成清脆的撞擊聲響（支援一鍵靜音）。
* 🎨 **四大精選故事主題庫**：內建 **🌦️ 天氣與自然**、**⚔️ 奇幻冒險**、**❤️ 情感與生活**、**🦉 角色與遭遇** 共 24 種專屬圖示與意涵。
* 🛠️ **高度彈性自訂六面**：提供視覺化自訂面板，允許使用者自由修改骰子六面的名稱、FontAwesome 圖示代碼與故事引導提示。
* ✍️ **一站式故事創作畫布**：內建無干擾寫作區，完成創作後支援「一鍵複製全文」與「下載 `.txt` 純文字檔」。
* 🌸 **馬卡龍粉色系玻璃擬態 UI**：採用溫馨亮麗的粉櫻漸層與 Glassmorphism 設計語言，減輕長時間思考與寫作的視覺疲勞。

---

## 🛠️ 技術架構 (Tech Stack)

| 技術領域 | 採用技術 / 工具 | 應用說明 |
| :--- | :--- | :--- |
| **核心結構** | HTML5 (Single-File) | 單一檔案整合結構、樣式與邏輯，便於攜帶與部署 |
| **3D 視覺與動畫** | CSS3 (`preserve-3d`, `perspective`) | 構建六面體立體空間與多軸向隨機旋轉過渡動畫 |
| **介面樣式設計** | Tailwind CSS (CDN) | 響應式排版（RWD）、玻璃擬態卡片與粉色漸層視覺 |
| **圖示系統** | FontAwesome 6 | 提供豐富且清晰的向量圖示作為骰面視覺元素 |
| **互動與音效** | Vanilla JS (ES6+) / Web Audio API | 控制狀態機、自訂表單邏輯與即時振盪器音效合成 |

---

## 🚀 開發歷程 (Development Journey)

本專案從概念發想到完整展示平台的演進分為四個主要階段：

* **Phase 1：核心原型驗證 (Core Prototype)**
  * 完成 CSS 3D 立方體六面定位算式，解決 3D 空間翻轉角度計算問題。
  * 導入 Web Audio API 振盪器，實現零外部資源的擲骰碰撞音效。
* **Phase 2：寫作體驗與自訂功能 (UX & Customization)**
  * 擴充至 4 大主題卡組，並為每個圖示撰寫「故事意涵解讀（Hint）」。
  * 加入右側創作畫布與 `.txt` 匯出功能，並開發「自訂六面」彈出視窗。
* **Phase 3：產品評估與社群企劃 (Product Analysis & Polls)**
  * 系統性盤點產品的優缺點與市場差異化優勢。
  * 規劃 5 大社群互動票選題目，確立未來功能迭代方向。
* **Phase 4：全功能展示平台與視覺升級 (V2.0 Showcase Platform)**
  * 整合產品封面、遊戲主體、專案分析報告與票選看板為一頁式網站，並全面升級為高親和力的「粉紅馬卡龍」亮色系主題。

---

## 📊 專案分析與差異比較 (Project Analysis)

### 1. 優缺點評估 (Pros & Cons)

| 評估維度 | 具體項目說明 |
| :--- | :--- |
| **✅ 核心優勢**<br>*(Advantages)* | • **沉浸式感官體驗**：3D 空間翻轉搭配即時音效，大幅提升創作樂趣。<br>• **寫作閉環整合**：擲骰與寫作無縫銜接，支援一鍵匯出成果。<br>• **高度客製化**：可依教學或遊戲需求自由替換骰面圖示與提示詞。<br>• **零門檻高效能**：單一檔案架構，無外部大型依賴，跨裝置秒開即用。 |
| **⚠️ 改進空間**<br>*(Limitations)* | • **圖示輸入門檻**：自訂面板目前需手動輸入 FontAwesome 類別名稱（如 `fa-dragon`）。<br>• **擬真物理限制**：採用角度動畫算式而非完整物理引擎（如 Cannon.js），落點較規律。<br>• **本地暫存機制**：草稿目前僅存於當前分頁記憶體，重整前需手動下載保存。 |

### 2. 與常見線上隨機工具之差異 (Differentiation)

| 比較項目 | 一般線上骰子 / 抽卡工具 | The Tale-Weaver's Dice |
| :--- | :--- | :--- |
| **視覺呈現動態** | 多為 2D 平面圖片瞬間切換 | **原生 CSS 3D 立體空間翻轉與光影質感** |
| **創作功能整合** | 僅顯示抽籤結果，需另開筆記軟體 | **內建靈感解讀卡與寫作畫布，支援一鍵匯出** |
| **新手引導機制** | 僅給出抽象圖案，容易無從下筆 | **自動提供圖示意涵提示（Hint）輔助構思** |
| **系統資源負載** | 依賴大型 3D 繪圖庫或外部音訊檔 | **純原生程式碼實現 3D 與音效，零外部多媒體負擔** |

---

## 🗳️ 未來發展與社群票選規劃 (Roadmap & Polls)

為持續傾聽使用者聲音並優化產品，專案規劃了以下 5 大社群投票方向作為後續版本迭代指標：

1. **新主題擴充**：賽博龐克與科幻未來 / 校園青春日常 / 神話怪談懸疑 / 職場冒險
2. **核心功能優先級**：AI 故事開頭產生器 / 視覺化點選式圖示庫 / 瀏覽器自動存檔 (`localStorage`) / 自訂圖片上傳
3. **遊戲化寫作模式**：3 分鐘限時極速挑戰 / 指定結局大反轉 / 每日全網同題寫作牆 / 雙人故事接龍
4. **多樣化視覺面板 (Skins)**：粉紅馬卡龍（現有預設） / 復古羊皮紙 / 溫暖手繪木質 / 8-Bit 像素風
5. **社群創作活動**：人氣故事首頁展示 / 實體紀念骰子周邊 / 寫作點評與成就徽章系統

---

## 📦 快速開始 (Quick Start)

本專案無需任何 Node.js 環境、套件管理器或編譯步驟（Zero-Build）：

1. **取得專案檔案**：點擊本儲存庫右上角的 `Code` ➔ `Download ZIP`，或直接下載 `index.html` 檔案。
2. **啟動應用程式**：雙擊 `index.html`，使用任一現代網頁瀏覽器（Chrome、Edge、Safari、Firefox）開啟。
3. **開始創作**：
   * 在上方選擇喜歡的主題與骰子數量（1~4 顆）。
   * 點擊 **「擲出故事骰子 !」** 或直接點擊單顆 3D 骰子進行滾動。
   * 參考下方的元素解讀卡片，在右側畫布寫下您的故事並匯出保存！

---

## 📄 授權條款 (License)

本專案採用 [MIT License](https://opensource.org/licenses/MIT) 開放原始碼授權。歡迎自由使用、修改、教學演示或進行二次開發。
