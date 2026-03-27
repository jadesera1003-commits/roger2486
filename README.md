# ⚔️ RO 專業裝備模擬器 (RO Equipment Simulator) v2.4 

這是一個專為《仙境傳說 (Ragnarok Online)》玩家打造的輕量化網頁版裝備模擬器。無需安裝任何軟體或連接資料庫，只要打開網頁即可快速計算特定裝備組合的綜合能力加成。

## 🌟 功能特色 (Features)

* **純前端運算**：使用 HTML, CSS 與原生 JavaScript 開發，無後端依賴，載入速度極快。
* **精煉與階級系統**：完整支援 +9 至 +12 的精煉能力計算，以及 D 級至 A 級的裝備階級能力解鎖。
* **套裝效果自動判定**：內建智能判定邏輯，當裝備特定組合時 (例如：雪花套裝、冰晶飾品對、黯淡三件套) 會自動結算額外的 Set Bonus。
* **即時數據面板**：裝備變更時，右側面板會即時更新 ATK, MATK, POW, CON, 延遲/固詠減少等關鍵戰鬥數值。

## 🎮 線上直接使用 (Live Demo)

👉 **[點我開啟 RO 裝備模擬器](https://jadesera1003-commits.github.io/roger2486/)** *(請確保已在 GitHub Pages 設定中開啟此連結)*

## 🛠️ 支援的裝備系列 (Supported Equipment)

目前資料庫內建以下最新熱門裝備系列：
* **雪花系列** (Snow Series)：鎧甲、外袍、斗篷、圍巾、戰靴、長靴及飾品。
* **冰晶系列** (Ice Series)：涵蓋完整的物理/魔法防具與飾品，支援階級突破。
* **黯淡冰晶系列** (Dim Ice Series)：支援根據精煉總和計算動態加成能力。

## 💻 本機開發與執行 (Local Development)

如果您想下載原始碼進行修改或擴充裝備庫，可以透過以下指令在本地端運行：

1. 複製此儲存庫：
   ```bash
   git clone [https://github.com/jadesera1003-commits/roger2486.git](https://github.com/jadesera1003-commits/roger2486.git)
