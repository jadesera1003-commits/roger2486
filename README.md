# ⚔️ Ragnarok Online Equipment Simulator (v2.4)

[![Live Demo](https://img.shields.io/badge/Live-Demo-success?style=for-the-badge)](https://jadesera1003-commits.github.io/roger2486/)

A lightweight, front-end only web calculator for Ragnarok Online. 
[ 繁體中文 (TwRO) ](#-twro-裝備模擬器) | [ English (iRO) ](#-iro-equipment-simulator) | [ 한국어 (kRO) ](#-kro-장비-시뮬레이터)

---

## 🇹🇼 TwRO 裝備模擬器

這是一個純前端寫的 RO 裝備計算機，主要用來計算 EP19 之後的裝備加成。不需要安裝任何環境或連線資料庫，點開網頁就能直接算。

### 📌 核心功能
* **純靜態網頁**：無後端依賴，掛在 GitHub Pages 上讀取速度極快。
* **精煉與階級計算**：內建 +9 ~ +12 的精煉能力計算，以及 D 階級 ~ A 階級的能力解鎖判斷。
* **套裝效果 (Set Bonus)**：自動判斷組合，例如雪花套、冰晶飾品套，甚至包含「黯淡三件套」這種吃精煉總和的複雜加成，都會自動算進面板。
* **實時面板**：右側面板即時更新，點選裝備直接看 ATK、MATK、延遲 (Delay)、固詠 (FCT)、變詠 (VCT) 等總和。

### 🛠️ 如何自行擴充裝備？
資料全部寫死在 `index.html` 的 `itemDB` 物件裡面。如果你想自己加新裝備（例如未來的 EP20 裝備），只要照著現有的 JSON 格式，把裝備 ID、能力值丟進去就能直接動了。

---

## 🇺🇸 iRO Equipment Simulator

A lightweight, browser-based equipment calculator for Ragnarok Online (focused on EP19+ gear). No backend required.

### 📌 Features
* **Zero Setup**: Runs entirely in the browser using HTML/JS. 
* **Refine & Grade System**: Automatically calculates stat bonuses for Refine levels (+9 to +12) and Equipment Grades (D to A).
* **Smart Set Bonuses**: Automatically applies combo effects (e.g., Snow set, Ice accessories, Dim Ice combo based on total refine levels).
* **Real-time Stat Panel**: Instantly updates ATK, MATK, VCT, FCT, Skill Delay, and other key combat stats as you change gear.

### 🛠️ How to Add New Items
All equipment data is stored in the `itemDB` object inside `index.html`. You can easily fork this repo and add new gear using the existing JSON structure.

---

## 🇰🇷 kRO 장비 시뮬레이터

라그나로크 온라인(EP19 이후) 장비 세팅을 위한 가벼운 웹 시뮬레이터입니다. 데이터베이스나 백엔드 없이 브라우저에서 바로 실행됩니다.

### 📌 주요 기능
* **웹 기반 (No 설치)**: 순수 프론트엔드로 제작되어 로딩이 빠릅니다.
* **제련 및 등급 시스템**: +9 ~ +12 제련도 및 D ~ A 등급(Grade) 옵션을 완벽히 계산합니다.
* **세트 옵션 자동 적용**: 설화(Snow) 세트, 글레시어(Ice) 액세서리, 희미한 글레시어(Dim Ice) 세트(제련도 합산) 효과가 자동으로 반영됩니다.
* **실시간 스탯 확인**: 장비를 변경할 때마다 ATK, MATK, 고캐(FCT), 변캐(VCT), 스후딜(Skill Delay) 등 총합 스탯을 즉시 확인할 수 있습니다.

### 🛠️ 장비 데이터 추가 방법
모든 장비 데이터는 `index.html` 파일 내 `itemDB`에 저장되어 있습니다. JSON 형식에 맞춰 새로운 장비를 쉽게 추가하거나 수정할 수 있습니다.
