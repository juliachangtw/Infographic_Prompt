# 📊 AI 資訊圖表萬能提示詞生成器 (AI Infographic Prompt Generator)

這是一個強大的網頁工具，專為 **Midjourney**、**DALL-E 3** 等生成式 AI 設計。它能協助使用者快速生成結構嚴謹、風格統一的「資訊圖表 (Infographic)」提示詞 (Prompts)。

內建 **100 種以上** 的專業排版架構，並具備 **圖片視覺分析功能**，能自動從參考圖中提取色票與風格關鍵字。

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

## ✨ 主要功能 (Key Features)

- **🎨 智慧圖片風格分析 (Smart Image Analysis)**
  - 上傳參考圖片，系統透過 Canvas API 自動分析像素。
  - **自動提取色票**：找出圖片中最主要的 5 種顏色。
  - **風格偵測**：自動推算亮度、對比度、飽和度，生成如 "High Contrast"、"Minimalist"、"Warm Tone" 等風格標籤。
- **📚 100+ 專業圖表架構**
  - 收錄 9 大類別（時序、比較、層級、流程、數據視覺化、地理、隱喻、列表、儀表板）。
  - 包含從基本的「甘特圖」、「心智圖」到進階的「桑基圖」、「瑞士刀隱喻」等詳細佈局。
- **📝 支援資料導入**
  - 可直接貼上數據文本。
  - 支援上傳 `.txt`, `.csv`, `.json` 等文件，將內容自動讀入提示詞 Context 中。
- **🛠 高度客製化**
  - **視覺風格**：提供 12 種預設風格（如：孟菲斯風格、等距 3D、霓虹賽博龐克）。
  - **比例設定**：支援 16:9, 3:2, 1:1, 9:16 及 A4 尺寸。
  - **色調管理**：可選預設色系或使用從圖片分析出的客製化色票。
- **🚀 極速體驗**
  - 單頁應用 (SPA)，無須後端，瀏覽器打開即用。
  - 響應式設計 (RWD)，支援手機與桌面操作。
  - 一鍵複製 Prompt，並自動隨機生成靈感。

## 🚀 如何使用 (Usage)

1.  **開啟工具**：直接使用瀏覽器打開 `index.html`。
2.  **(選用) 上傳參考圖**：
    - 點擊左上角的上傳區塊，選擇一張你喜歡的風格圖片。
    - 系統會自動分析並勾選「應用視覺屬性」。
3.  **設定圖表參數**：
    - 輸入 **主題** (例如：生成式 AI 的發展歷史)。
    - 選擇 **排版類別** 與 **圖表類型**。
    - 選擇 **視覺風格** 與 **比例**。
4.  **提供數據 (Context)**：
    - 在文字框輸入想要呈現的數據，或點擊「讀取文字檔」上傳資料。
5.  **生成與輸出**：
    - 點擊「**生成提示詞**」按鈕。
    - 右側面板將顯示完整的 Markdown 格式提示詞。
    - 點擊「**複製提示詞**」並貼上至 Midjourney 或 ChatGPT/DALL-E 3。

## 💻 技術架構 (Tech Stack)

本專案採用純前端技術構建，無需安裝 Node.js 或任何依賴包即可運行（需連網以讀取 Tailwind CDN）。

- **核心語言**：HTML5, CSS3, Vanilla JavaScript (ES6+)
- **樣式框架**：[Tailwind CSS](https://tailwindcss.com/) (透過 CDN 引入)
- **字體**：Google Fonts (Noto Sans TC)
- **圖像處理**：HTML5 Canvas API (用於像素級色彩與亮度分析)

## 📂 檔案結構

```text
.
├── index.html       # 包含所有邏輯、樣式與結構的單一檔案
└── README.md        # 說明文件
```
