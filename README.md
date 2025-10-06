# TheraNotes

<div align="center">

![TheraNotes Logo](static/logo.png)

**安全、本機優先的個人諮商紀錄系統**

A secure, local-first personal counseling record system

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/yourusername/TheraNotes/releases)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Tauri](https://img.shields.io/badge/Tauri-2.0-brightgreen.svg)](https://tauri.app/)
[![Svelte](https://img.shields.io/badge/Svelte-5.0-orange.svg)](https://svelte.dev/)

[官方網站](https://filedn.eu/lnMPQu6qnE709ro96qxK1tR/TheraNotes.html) • [下載](https://github.com/yourusername/TheraNotes/releases) • [贊助支持](https://portaly.cc/TheraNotes/support)

</div>

---

## 📖 關於 TheraNotes

TheraNotes 是一款專為心理諮商師設計的**個案管理系統**，提供安全的本機資料儲存、自動儲存功能，以及便捷的諮商紀錄管理。

### 💡 開發初衷

> 嗨，我是開發 TheraNotes 的製作者 Ori_Lee，
>
> 我現在是一名碩三實習中的諮商心理師。在實習過程中，我發現當案量提升時，我們的大腦已經無法隨時記得每個案主的狀況。這對助人者是認知的耗竭、對案主是損害到接受有效晤談的權益、對學習而言也是進入無效能感。
>
> 一開始我嘗試用 Google Sheets 記錄，但雲端儲存有資安風險；改用 Excel 後，又發現不適合儲存長篇文字。因此，**TheraNotes 誕生了**——一個本機優先、注重資料安全的個案管理系統。

---

## ✨ 主要功能

### 🔐 資料安全
- **本機加密儲存**：使用 SQLCipher 加密資料庫
- **無雲端同步**：所有資料完全儲存在本機
- **密碼保護**：首次啟動時設定資料庫密碼

### 📝 個案管理
- **完整的個案資料**：姓名、代號、性別、出生日期、證號等基本資料
- **風險評估**：風險等級、通報狀態追蹤
- **個案狀態**：晤談中、結案、暫停等狀態管理
- **定期晤談設定**：記錄固定晤談時段（如每週三下午 2:00）
- **備註欄位**：彈性記錄其他重要資訊

### 📋 諮商紀錄
- **晤談紀錄撰寫**：包含晤談內容、評估、後續計畫
- **心理師札記**：記錄對晤談的想法、困惑、督導意見
- **預設模板**：提供結構化的紀錄模板，提升記錄效率
- **紀錄編輯與刪除**：完整的 CRUD 操作

### 🔍 搜尋與排序
- **快速搜尋**：支援姓名、代號、狀態、證號等多欄位搜尋
- **智慧排序**：依下次晤談時間、建立日期、姓名排序
- **即時過濾**：搜尋結果即時顯示，並統計符合筆數

### 💾 自動儲存
- **表單自動儲存**：所有表單內容自動儲存至 localStorage
- **意外保護**：即使意外關閉，下次開啟會詢問是否恢復
- **獨立儲存空間**：每個表單/個案有獨立的自動儲存空間

### ⌨️ 鍵盤快捷鍵
- **Ctrl + 滾輪**：縮放畫面（50%-200%）
- **Ctrl + S**：快速儲存表單
- **Alt + 1**：回到個案總覽
- **Alt + N**：跳轉到新增個案
- **Alt + F**：搜尋個案
- **F1 或 Ctrl + /**：顯示快捷鍵說明
- **Esc**：關閉彈窗/取消操作

### 🎨 使用者介面
- **響應式設計**：適應不同螢幕尺寸
- **溫暖配色**：舒適的米色和暖灰色調
- **清晰的視覺層次**：卡片式設計，資訊一目了然
- **無障礙支援**：鍵盤操作友善

---

## 📥 下載安裝

### 系統需求
- **作業系統**：Windows 10/11 (64-bit)
- **硬碟空間**：約 50 MB
- **記憶體**：建議 4 GB 以上

### 安裝選項

#### 🎯 推薦：NSIS 安裝版（5.2 MB）
```
TheraNotes_1.0.0_x64-setup.exe
```
- ✅ 自動建立開始選單和桌面捷徑
- ✅ 完整的安裝與解除安裝程式
- ✅ 資料庫儲存在安全的 AppData 位置
- ✅ 內建所有必要運行庫

#### 🏢 企業版：MSI 安裝檔（7.2 MB）
```
TheraNotes_1.0.0_x64_en-US.msi
```
- ✅ Windows 標準企業安裝格式
- ✅ 支援靜默安裝和群組原則
- ✅ 適合企業環境部署

#### 🎒 攜帶版：ZIP 壓縮檔（6.9 MB）
```
TheraNotes_1.0.0_Portable.zip
```
- ✅ 免安裝，解壓即用
- ✅ 適合 USB 隨身碟攜帶
- ✅ 無需管理員權限
- ⚠️ 資料庫儲存在程式目錄，請勿隨意移動

---

## 🚀 快速開始

### 首次使用

1. **安裝/解壓縮**應用程式
2. **啟動 TheraNotes**
3. **設定資料庫密碼**（請妥善保管，遺失無法復原）
4. 開始使用！

### 基本操作

#### 新增個案
1. 在個案總覽頁面，點擊「新增個案」區塊
2. 填寫個案基本資料
3. 按 **Ctrl + S** 或點擊「送出」儲存

#### 編輯個案
1. 點擊個案卡片
2. 在個案詳細頁面點擊「編輯個案資料」
3. 修改後按 **Ctrl + S** 儲存

#### 新增諮商紀錄
1. 進入個案詳細頁面
2. 點擊「新增諮商紀錄」
3. 填寫晤談內容和心理師札記
4. 按 **Ctrl + S** 儲存

#### 搜尋個案
- 按 **Alt + F** 快速聚焦搜尋框
- 輸入關鍵字（姓名、代號、狀態、證號）
- 即時顯示符合的個案

---

## 🛠️ 技術架構

### 前端
- **框架**：[SvelteKit 2.9](https://kit.svelte.dev/) + [Svelte 5](https://svelte.dev/)
- **樣式**：[TailwindCSS 3.4](https://tailwindcss.com/)
- **狀態管理**：Svelte Stores + Svelte 5 Runes
- **建置工具**：[Vite 6](https://vitejs.dev/)

### 後端
- **桌面框架**：[Tauri 2.0](https://tauri.app/)
- **程式語言**：Rust 2021
- **資料庫**：[SQLite](https://www.sqlite.org/) + [SQLCipher](https://www.zetetic.net/sqlcipher/)（加密）
- **資料庫連接**：[rusqlite 0.31](https://github.com/rusqlite/rusqlite)

### 安全性
- **資料加密**：使用 SQLCipher 的 AES-256 加密
- **本機儲存**：所有資料儲存在本機，不經過網路傳輸
- **密碼保護**：資料庫層級的密碼驗證

---

## 🔒 隱私與安全

### 資料儲存
- **完全本機化**：所有資料儲存在您的電腦上
- **無網路連線**：應用程式不會連接網路（除了開啟外部連結）
- **加密保護**：使用業界標準的 SQLCipher AES-256 加密

### 資料位置
- **安裝版**：`%APPDATA%\com.orilee.theranotes\` 或 `P:\[90]TheraNotes\`（若 P 槽存在）
- **攜帶版**：程式執行檔所在目錄

### 資料備份建議
1. 定期複製資料庫檔案（`TheraNotes.db`）
2. 將備份存放在安全的位置（加密硬碟、USB 等）
3. **重要**：請記住您的資料庫密碼，遺失無法復原

--

## 📄 授權

本專案採用 MIT 授權條款 - 詳見 [LICENSE](LICENSE) 檔案。

---

## 💖 支持專案

TheraNotes 是完全免費的開源軟體。如果這個專案對您有幫助，歡迎：

- ⭐ 給這個專案一個 Star
- 🐛 回報問題或建議功能
- 💝 [贊助支持](https://portaly.cc/TheraNotes/support) - 請我喝杯咖啡 ☕

---

## 📮 聯絡方式

- **開發者**：Ori_Lee
- **Email**：lee2952000@gmail.com
- **官方網站**：[https://filedn.eu/lnMPQu6qnE709ro96qxK1tR/TheraNotes.html](https://filedn.eu/lnMPQu6qnE709ro96qxK1tR/TheraNotes.html)
- **贊助支持**：[https://portaly.cc/TheraNotes/support](https://portaly.cc/TheraNotes/support)

---

## 🙏 致謝

感謝所有使用 TheraNotes 的心理師和實習生們。你們的回饋讓這個專案持續進步。

特別感謝以下開源專案：
- [Tauri](https://tauri.app/) - 讓桌面應用開發變得簡單
- [Svelte](https://svelte.dev/) - 優雅的前端框架
- [SQLCipher](https://www.zetetic.net/sqlcipher/) - 提供安全的資料加密

---

## 📝 更新日誌

### V1.0.0 (2025-10-06)

#### 新功能
- ✨ 完整的個案管理系統
- ✨ 諮商紀錄撰寫與管理
- ✨ 自動儲存功能
- ✨ 鍵盤快捷鍵支援
- ✨ 畫面縮放功能（50%-200%）
- ✨ 搜尋與排序功能
- ✨ 資料庫加密保護

#### 技術
- 🔧 使用 Tauri 2.0 + Svelte 5
- 🔧 SQLCipher 加密資料庫
- 🔧 完整的安裝檔打包（MSI、NSIS、攜帶版）

---

<div align="center">

**用心製作 | Made with ❤️ by Ori_Lee**

如果這個專案對您有幫助，請考慮給它一個 star⭐

</div>
