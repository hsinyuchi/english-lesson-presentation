---
name: english-lesson-presentation
description: Use when creating an interactive HTML5 classroom presentation from an English passage or lesson text, featuring sentence-by-sentence slides, CEEC 108 7000-word vocabulary highlighting, dark/light mode, drawing canvas, and reading comprehension quizzes.
---

# 旗艦多模態英語課程互動簡報技能 (English Lesson Presentation Skill)

## 🎯 核心定位與教學價值
本技能專門將任意英文課文、素養短文或時事新聞，自動轉換為「單一檔案、開箱即用、免伺服器」的**旗艦多模態互動教學簡報網頁 (HTML5)**。
專為高中職英文教師課堂精讀、大考單字教學、心智圖結構導讀與即時素養測驗設計。

---

## ⚡ 觸發時機 (When to Use)
- 想要將一篇英文課文或短文，快速製作成可在電子白板、大螢幕或平板上互動教學的簡報網頁。
- 需要逐句精讀（一頁一句）、即時切換中文翻譯、播放原音朗讀。
- 需要大考中心 108 課綱 7000 單動態分級（L1~L6）高亮與即時單字彈出卡片。
- 需要內建課文心智圖（Mission 1）與 5 題素養選擇題組（Mission 2）。

---

## 🏗️ 互動簡報四大核心架構

```
[Slide 0] 封面頁 (Cover Slide)
   │
   ├── [Slide 1 ~ N] 句子精讀頁 (Sentence Slides • 一頁一句)
   │     ├── 特大英文原句 (2.8rem Bold) + 單字點擊彈出卡片 (Popover Card)
   │     ├── 真人原音播放列 (Play / Pause / 0.75x~1.25x 語速滑桿)
   │     ├── 繁體中文翻譯抽屜 (點擊展開 / 快捷鍵 T 揭曉)
   │     └── 核心單字片語解析標籤 (Note Chips • 標註 L1~L6 級別)
   │
   ├── [Slide N+1] Mission 1 課文結構心智圖 (Structure Map)
   │     ├── 3~5 張結構摘要卡片 (含 5 個挖空題)
   │     └── 點擊卡片翻牌揭曉答案 / 一鍵全開按鈕
   │
   └── [Slide N+2 ~ N+6] Mission 2 閱讀素養題組 (Q1 ~ Q5)
         ├── Q1/Q2 單字文意題 + Q3 主旨題 + Q4 細節題 + Q5 推論題
         ├── 即時點擊判定 (答對綠色 / 答錯紅色)
         ├── 題幹與選項朗讀語音按鈕
         └── 【考點剖析與干擾項排除】抽屜
```

---

## 🎨 課堂互動黑科技工具箱 (Classroom Teaching Toolbar - v4 旗艦升級)

簡報底部浮動工具箱與智慧大螢幕/平板專屬設計：
1. **🚫 零滾動單頁自適應 (Zero-Scroll Auto-Fit Screen)**：保證任何智慧大螢幕 (86" IFP)、投影機或 iPad 螢幕絕不產生垂直捲軸，字體依視窗自動等比放大 (`clamp`)。
2. **🌓 深淺色主題 (Theme Toggle • 快捷鍵 D)**：曜石深黑 (護眼沉浸) ⇄ 晨光純白 (紙本質感)，螢光筆混合模式智慧聯動（深色 Screen 加色 / 淺色 Multiply 高亮）。
3. **🎨 iPad Freeform 無邊際畫布**：支援 60% ~ 300% 縮放與畫布平移，可在兩側延伸黑板空白處自由板書。
4. **✏️ 繪圖手寫與觸控雷射 (Touch Pointer & Apple Pencil)**：支援指尖/手寫筆觸控拖曳雷射光軌、原子筆 (P)、柔光螢光筆 (H)、便箋 (N)、復原 (Ctrl+Z)、清除。
5. **⏱️ 課堂活動計時器 (Classroom Timer • 快捷鍵 M)**：內建 1 分、3 分、5 分、10 分快速預設、+30秒微調與叮咚響鈴提示音，隨時引導小組討論。
6. **🎲 課堂隨機抽籤 (Lucky Draw • 快捷鍵 R)**：內建自訂座號抽籤轉盤，點名學生回答問題。
7. **🧲 工具箱智慧拖曳與靠邊快捷 (Docking Presets)**：底部工具列支援順暢拖拉定位，並提供 `[左靠]`、`[中靠]`、`[右靠]` 一鍵吸附，完美適應站位。
8. **🗂️ 全覽九宮格跳頁 (Slide Grid Overview • 快捷鍵 G)**。
9. **⌨️ 完整鍵盤快捷鍵**：←/→ 或 Space 翻頁、F 全螢幕、T 揭曉翻譯、M 計時器、D 切換主題。
10. **📦 講義與板書一鍵匯出 (Export Engine)**：完整擷取全頁投影片與板書筆記，一鍵匯出為 PDF 講義或 PNG 圖檔 ZIP。

---

## 📝 製作規範與資料規格

### 1. 文本拆句規則
* 依標點符號 (`.`、`?`、`!`) 將課文切割為完整單句，每句獨立為一個 `sentence-slide`。
* 句子中的單字必須用 `<span class="dict-word l{lvl}" data-word="{word}" onclick="inspectWord('{word}', event)">{word}</span>` 包裹。

### 2. 7000 單詞庫 (WORD_DB) 格式
```javascript
const WORD_DB = {
  "apple": { "lvl": 1, "kk": "/ˈæp.əl/", "pos": "n.", "def": "蘋果", "colloc": "an apple a day", "ex": "I eat an apple daily." },
  "embarrassing": { "lvl": 3, "kk": "/ɪmˈber.ə.sɪŋ/", "pos": "adj.", "def": "令人尷尬的", "colloc": "an embarrassing moment", "ex": "It was an embarrassing situation." }
};
```

### 3. Mission 1 結構圖解格式
* 3~5 張卡片，包含標題、學生版挖空、教師版解答與考點提示。

### 4. Mission 2 素養題目規範
* 嚴格 5 題：Q1/Q2 單字理解、Q3 全篇主旨 (Main Idea)、Q4 細節推論 (Detail)、Q5 寫作語氣/目的 (Tone/Purpose)。
* 每題必須包含：題型 Badge、題幹、四個選項 `(A)(B)(C)(D)`、正確答案、詳細中文解析與干擾項排除說明。

---

## 🚫 常見錯誤與守門員原則 (Anti-Patterns)
1. ❌ **嚴禁繁中翻譯漏句或合併**：翻譯必須與英文句子 1:1 精準對應。
2. ❌ **嚴禁單字級別誤標**：基礎字（如 still, poor, animal）嚴禁誤歸入 Level 5/6。
3. ❌ **嚴禁使用外部繁重框架**：全部使用原生 Vanilla HTML5/CSS3/JavaScript，單一檔案即刻運行。
