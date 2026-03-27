# ⚔️ RO 專業裝備模擬器 (RO Equipment Simulator)

[![Version](https://img.shields.io/badge/Version-2.4-blue.svg)](#)
[![Status](https://img.shields.io/badge/Status-Active-success.svg)](#)

> 專為《仙境傳說 Ragnarok Online》打造的輕量化網頁版裝備計算機。無須安裝後端環境、純前端運算，點開網頁即可即時檢視面板數值。

👉 **[點我開啟 RO 裝備模擬器 (Live Demo)](https://jadesera1003-commits.github.io/roger2486/)**

---

## 🌟 系統特色

* **極致輕量**：採用 HTML + 原生 JavaScript 開發，運算邏輯全在本地瀏覽器執行，零延遲。
* **動態數值面板**：切換裝備的瞬間，右側面板即時結算 ATK、MATK、延遲、固詠等關鍵戰鬥數值。
* **深度機制支援**：
  * 完整對應 **精煉 (+9 ~ +12)** 與 **裝備階級 (Grade D ~ A)** 系統。
  * 內建智能 **套裝判定 (Set Bonus)**（如：雪花套、冰晶飾品對）。
  * 支援特殊動態加成（如：黯淡三件套依「精煉總和」計算額外數值）。

---

## 🚀 未來開發藍圖 (Roadmap)

這裡記錄了專案未來的擴充方向，將視開發進度陸續實裝：

- [x] **v2.0+**：建立核心計算引擎與 UI 介面。
- [x] **v2.4**：實裝 EP19 雪花、冰晶、黯淡系列裝備與階級邏輯。
- [ ] **v3.0**：整合「角色基礎素質 (Status Calculator)」系統，將人物 STR/AGI/VIT 等配點納入總面板計算。
- [ ] **v3.x**：擴充卡片 (Card) 與附魔 (Enchant) 插槽系統。
- [ ] **v4.0**：實裝各職業主流技能的傷害公式試算。

---

## 📝 版本紀錄 (Changelog)

維持專案的更新透明度，最新版本請見最上方：

* **[v2.4] - 2026-03**
  * 新增：黯淡冰晶系列裝備。
  * 更新：優化 `checkSetBonuses` 邏輯，修復套裝效果判定。
  * 調整：UI 介面升級，新增獨立的總計加成能力面板。

* **[v2.0] - 早期版本**
  * 建立基礎裝備選擇器與精煉下拉選單。
  * 導入雪花與冰晶系列基礎資料。

---

## 🛠️ 開發者指南：如何擴充資料庫？

本專案將所有的裝備資料結構化並統一管理於 `index.html` 中的 `itemDB` 物件。
若需新增裝備（如未來的 EP20），只需依照以下 JSON 格式新增物件，系統將自動套用計算邏輯，無須修改核心程式碼：

```javascript
// 擴充範例格式
{ 
    id: 'item_id', 
    name: '裝備名稱', 
    series: '系列標籤', 
    base: { atk: 100, mhp_p: 10 }, // 基礎能力
    refine_rules: [{ interval: 2, stats: { atk: 15 } }], // 規律性精煉加成
    milestones: { 7: { aspd_p: 10 }, 9: { p_atk: 2 } }, // 特定精煉門檻加成
    grades: { // 階級加成
        D: { base: { pow: 3 } }, 
        C: { base: { atk_p: 3 } } 
    } 
}
