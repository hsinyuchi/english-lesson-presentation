---
name: hsinyuchi-lesson-presentation
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


---

## 🛡️ 研習現場自動防呆與環境相容機制 (Workshop Foolproof & Pre-Flight Check)

為了確保在研習工作坊、教師社群共備現場，**每一位老師（無論使用 Windows / Mac / 公用電腦）都能 100% 成功編譯與運行**，AI Agent 必須遵循以下防呆標準作業程序：

### 1. 自動環境前置檢測 (Automated Pre-Flight Check)
在執行任何產出任務前，AI 必須主動檢查執行環境。若缺少必要套件，**必須主動提供「一鍵複製貼上」的安裝指令**，嚴禁丟出艱深報錯代碼讓學員慌張：

```bash
# 研習學員必備 Python 核心工具包（一鍵全裝指令）：
pip install edge-tts openpyxl beautifulsoup4 python-docx reportlab requests
```

### 2. 必要套件用途對照表：
* 🔊 `edge-tts`：微軟 Ava / Jenny 美式真人神經網路語音合成（產出課文單句與全文 MP3 音檔）。
* 📊 `openpyxl`：自動生成 Kahoot! 官方標準 Excel 試算表（`.xlsx`）一秒匯入題庫。
* 🌐 `beautifulsoup4`：HTML 網頁解析與動態標籤處理。
* 📝 `python-docx`：Word 講義、教案與學習單讀寫排版。
* 📄 `reportlab`：雙面 A4 雜誌風閱讀學習單與段考卷 PDF 繪製與匯出。

### 3. 零門檻優雅降級模式 (Graceful Fallback)
若學員受限於學校電腦權限無法安裝 Python 套件時，AI 必須自動啟動**「免安裝純前端降級模式」**：
- 語音播放：自動採用瀏覽器原生免安裝的 **Web Speech API (TTS)**。
- 題庫匯出：自動產出免依賴 Python 的 **純文字 CSV (Quizizz / Blooket)** 格式。
- 簡報運作：維持 **100% 純原生 Vanilla HTML5/CSS3/JS**，點開瀏覽器即刻教學！

---

## 🔒 跨 Agent 執行防漂移鐵律 (Cross-Agent Anti-Drift Protocol)

> **⚡ 適用環境：Google Antigravity、OpenAI Codex CLI、Claude Code、Cursor 等全平台 Agent**

任何 AI Agent 在執行本技能時，**嚴禁依賴各平台大模型的默認輸出習慣自由發揮**，必須 100% 嚴格落實以下防漂移守則：

1. **零自作主張 (Zero Creative Deviation)**：
   - 嚴格沿用本規範定義之排版結構、區塊順序、欄位標籤與樣式。
   - **嚴禁私自「改寫/簡化」架構**（例如擅自將特定 Flex/Grid 佈局改寫為文字列表、將精確卡片改為空泛條列、或將樣式簡化）。
   - **嚴禁自創未經授權的新區塊**（例如擅自新增額外理論講義、發音表或未要求的長篇大論）。
2. **骨架代碼與格式優先 (Template Boilerplate Priority)**：
   - 若本規範提供具體代碼片段（HTML、CSS、JS、Markdown 骨架、卡片容器），必須作為不可變更之「填空基底 (Immutable Slots)」。
   - Agent 的任務僅是將內容精準填入對應的 Slots 容器中，**禁止改動外層容器 class 名稱、DOM 結構與事件綁定機制**。
3. **成品規格不降級 (No Spec Downgrade)**：
   - 嚴禁因 Token 長度限制或內容龐大，而將「圖文並茂互動網頁/雙軌講義」偷工減料降級為「純文字草稿」或「簡短大綱」。
   - 遇長文本時必須完整輸出全課內容或完整分段寫入目標檔案，**絕不省略後半段**。
4. **雙軌/多模態完整性 (Dual-Track Completeness)**：
   - 凡涉及「學生練習版」與「教師紅字解答版」之技能，必須兩套完整產出，答案與詳解必須扎實完整，嚴禁留白。
   - 凡涉及固定卡片數量（如 2 張文法卡片、5 大單字卡片、10 題挖空等），**嚴格維持指定數量，不多不少**。
5. **角色語氣與受眾鎖定 (Persona & Audience Alignment)**：
   - 嚴格維持臺灣高中職英語科專業教師立場，第二人稱「你」或「同學們」具同理心之對話語調，**嚴格杜絕第三人稱論文式說教腔**。

### 🏛️ 互動簡報 v7 旗艦規範不可更動要求 (v7 Flagship Standards)
1. **16:9 劇院級比例鎖定**：投影片容器強制使用 `aspect-video rounded-2xl shadow-2xl`，支援全螢幕 (`F` 鍵) 與鍵盤左右導航。
2. **v7 工具列黑科技完整性**：
   - 雙色智慧螢光筆：必須具備 `mix-blend-mode: multiply` 特效（黃/綠）。
   - 每頁獨立便利貼：支援雙擊新增、拖曳移動與個別刪除。
   - 幾何圖形框選：矩形、圓形與引導箭頭。
   - 抽籤神器與倒數計時器：純前端浮動面板。
   - 純淨板書匯出：支援過濾課文、單純匯出板書軌跡。
3. **嚴禁降級為靜態 PPT 草稿**：產出必須為單一獨立 HTML5 檔案，內嵌 Tailwind CSS 與原生 JavaScript。
