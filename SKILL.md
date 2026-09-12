---
name: english-lesson-presentation
description: Use when creating an interactive HTML5 classroom presentation from an English passage or lesson text, featuring sentence-by-sentence slides, CEEC 108 7000-word vocabulary highlighting, dark/light mode, drawing canvas, and reading comprehension quizzes.
---

# 旗艦多模態英語「文本轉互動簡報」技能 (Text to Interactive Presentation Skill)

> 💡 **Designed & Crafted by**: **hsinyuchi (Sylvia)** | 臺灣高中職英語教育 AI 協作專案  
> 📜 **License**: [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)（歡迎教育非商業用途引用、共備與改編，轉載請註明出處）

---

## 🎯 核心定位與教學價值
本技能專門將**任意英文課文、時事新聞、素養短文或考題閱讀篇章**，全自動轉換為「單一檔案、開箱即用、免伺服器」的**旗艦多模態互動教學簡報網頁 (HTML5)**。
專為臺灣普通型高中與技術型高中英文科教師在**智慧大螢幕 (IFP/電子白板)、平板 (iPad/Apple Pencil) 及筆電**上的課堂精讀、大考單字動態教學、心智圖結構導讀與即時素養互動測驗量身打造。

---

## ⚡ 觸發時機 (When to Use)
- 想要將一篇英文文本快速製作為高質感、具備互動功能的單檔 HTML5 課堂簡報。
- 需要逐句精讀（一頁一句）、即時展開 1:1 繁體中文翻譯、播放真人/TTS 原音朗讀。
- 需要大考中心 108 課綱 7000 單動態分級（Level 1~6）高亮與即時單字彈出卡片 (Popover Card)。
- 需要內建課文心智圖（Mission 1）與 5 題大考素養選擇題組（Mission 2）。
- 需要完整的黑板互動工具箱（手寫、物理透光螢光筆、幾何框選、彩色便箋、計時器、抽籤器、講義匯出）。

---

## 🏗️ 互動簡報四大核心架構

```
[Slide 0] 封面頁 (Cover Slide)
   │
   ├── [Slide 1 ~ N] 句子精讀頁 (Sentence Slides • 一頁一句)
   │     ├── 特大英文原句 (2.8rem+ Clamp 自適應) + 7000 單字點擊彈出卡片 (Popover)
   │     ├── 原音播放列 (Play / Pause / 0.75x~1.25x 語速滑桿)
   │     ├── 繁體中文翻譯抽屜 (點擊展開 / 快捷鍵 T 揭曉)
   │     └── 核心單字片語解析標籤 (Note Chips • 標註 L1~L6 級別與詞性中釋)
   │
   ├── [Slide N+1] Mission 1 課文結構心智圖 (Structure Map)
   │     ├── 3~5 張結構摘要卡片 (含 5 個核心概念挖空題)
   │     └── 點擊卡片翻牌揭曉答案 / 一鍵全開按鈕
   │
   └── [Slide N+2 ~ N+6] Mission 2 閱讀素養題組 (Q1 ~ Q5)
         ├── Q1/Q2 單字文意題 + Q3 全篇主旨 + Q4 細節推論 + Q5 語氣目的
         ├── 即時點擊判定 (答對綠色 / 答錯紅色)
         ├── 題幹與選項朗讀語音按鈕
         └── 【考點剖析與干擾項排除】抽屜
```

---

## 🎨 課堂互動黑科技工具箱 (Classroom Teaching Toolbar - v7 旗艦升級)

簡報底部浮動工具箱與智慧大螢幕/平板專屬設計：

1. **🚫 零滾動單頁自適應 (Zero-Scroll Auto-Fit Screen)**：保證任何智慧大螢幕 (86" IFP)、投影機或 iPad 螢幕絕不產生垂直捲軸，字體依視窗自動等比放大 (`clamp`)。
2. **🌓 深淺色主題 (Theme Toggle • 快捷鍵 D)**：曜石深黑 (護眼沉浸) ⇄ 晨光純白 (紙本質感)，所有畫布圖層自動智慧聯動。
3. **🖍️ 物理透光不遮字螢光筆 (Highlighter • 快捷鍵 H)**：
   - 淺色模式採用 `mix-blend-mode: multiply`（正片疊底），黑色文字永遠維持 100% 極致純黑，英文字永不被顏料遮蔽！
   - 深色模式採用 `mix-blend-mode: screen`（透光濾色），白色文字維持 100% 亮白，背景呈現柔光光暈。
   - 內建 5 色透光色系：螢光黃 (`#facc15`)、螢光綠 (`#4ade80`)、柔光藍 (`#38bdf8`)、櫻花粉 (`#f472b6`)、活力橘 (`#fb923c`)。
4. **✏️ 繪圖手寫與觸控雷射 (Touch Pointer & Apple Pencil)**：支援指尖/手寫筆觸控拖曳霓虹雷射光軌、原子筆 (P)、橡皮擦 (E)、復原、清除。
5. **🔲 幾何形狀框選標記 (Geometric Shapes • 快捷鍵 S)**：
   - 支援 4 大核心板書幾何形狀：長方形 (🔲 Rectangle)、圓形/橢圓 (⭕ Circle/Ellipse)、指向箭頭 (➡️ Arrow)、分隔直線 (➖ Line)。
   - 內建 5 色調色盤（經典紅、螢光黃、活力綠、天空藍、純淨白）與即時拖曳預覽 (Live Geometry Drag Preview)。
6. **📝 重點彩色便箋 (Floating Sticky Notes • 快捷鍵 N)**：
   - 提供 4 款高對比柔和粉彩：檸檬黃 🟡、清新綠 🟢、天空藍 🔵、櫻花粉 🌸。
   - 支援頂部拖曳把手自由擺放、即時點擊編輯板書內容 (`contenteditable`)、右上角快速刪除鈕 (`✕`)。
   - 具備各頁獨立記憶功能（Per-Slide Sticky Memory），並自動納入講義與圖片匯出合成！
7. **⏱️ 課堂活動計時器 (Classroom Timer • 快捷鍵 M)**：內建 1 分、3 分、5 分、10 分快速預設、+30秒微調與響鈴提示音，右上角及底部均附有醒目 `✕` 實體觸控關閉按鈕。
8. **🎲 課堂隨機抽籤 (Lucky Draw • 快捷鍵 R)**：內建自訂座號抽籤轉盤，點名學生回答問題，附有醒目 `✕` 關閉按鈕（免鍵盤直接觸控關閉）。
9. **🧲 工具箱智慧拖曳與靠邊快捷 (Docking Presets)**：底部工具列支援順暢拖拉定位，並提供 `[左靠]`、`[中靠]`、`[右靠]` 一鍵吸附，完美適應站位。
10. **🗂️ 全覽九宮格跳頁 (Slide Grid Overview • 快捷鍵 G)**：一覽全課架構，支援點擊直接跳轉。
11. **⌨️ 完整鍵盤快捷鍵**：←/→ 或 Space 翻頁、F 全螢幕、T 揭曉翻譯、P 畫筆、H 螢光筆、S 形狀、N 便箋、M 計時器、D 切換主題、R 抽籤。
12. **📦 講義與自選板書匯出引擎 (Advanced Selective Export)**：
    - 支援自由勾選要匯出的頁面（提供 `[✓ 全選]`、`[✕ 全不選]`、`[✏️ 僅有筆記頁面]`、`[📖 僅課文句]`）。
    - 具有手寫筆記或便箋的頁面會自動標註 `✏️ 含有手寫筆記` 金色徽章。
    - 精準合成課文畫面、手寫筆記與彩色便箋，匯出為高畫質 PDF 講義或 PNG 圖片壓縮包 (ZIP)。

---

## 📝 製作規範與資料規格 (Data Specification)

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

## 🌐 雲端部署規範 (Cloudflare Pages Standard)
* 一律統一發布至 **Cloudflare Pages**（避免使用 Workers，以享有無限請求次數與高速靜態 CDN）。
* 專案名稱一律遵循 **`hsinyuchi-[專案名稱]`** 統一前綴格式（例如 `hsinyuchi-b1-english-hub`、`hsinyuchi-songs-hub`）。
* 網址規範：`https://hsinyuchi-[專案名稱].pages.dev`。

---

## 🚫 常見錯誤與守門員原則 (Anti-Patterns)
1. ❌ **嚴禁繁中翻譯漏句或合併**：翻譯必須與英文句子 1:1 精準對應。
2. ❌ **嚴禁單字級別誤標**：基礎字（如 still, poor, animal）嚴禁誤歸入 Level 5/6。
3. ❌ **嚴禁使用外部繁重框架**：全部使用原生 Vanilla HTML5/CSS3/JavaScript，單一檔案即刻運行。
