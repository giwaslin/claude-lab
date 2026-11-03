# LIN Studio · 平面設計作品集 Landing Page

一個單頁式（Landing Page）的平面設計師作品集網站，以深夜藍搭配金色點綴的視覺風格，呈現品牌識別、編輯設計與包裝設計作品。

## 網站功能

- **導覽列**：固定於頁面頂端（sticky），帶有毛玻璃效果，可快速跳至「作品」與「聯絡」區塊。
- **英雄區塊（Hero）**：主標題、簡介、接案狀態標籤、行動按鈕（CTA）與成果數據。
- **精選作品**：以卡片網格展示三件作品——
  - 星曜咖啡｜品牌識別
  - 《留白》｜季刊編輯設計
  - 山嵐茶事｜禮盒包裝
- **聯絡區塊（Footer）**：合作邀請文案、聯絡按鈕與社群連結，版權年份自動更新。
- **視覺效果**：動態星空背景、卷動時區塊淡入、按鈕與連結的 hover 動畫。
- **RWD 響應式設計**：
  - 平板（≤ 960px）：作品改為兩欄排列。
  - 手機（≤ 720px）：單欄排列、縮小標題與間距、觸控目標至少 44px、避免橫向捲動。
- **無障礙**：鍵盤聚焦外框（`:focus-visible`），並支援「減少動態效果」（`prefers-reduced-motion`）設定。

## 使用技術

- **HTML5**：語意化標籤（`header`、`main`、`section`、`footer`）。
- **CSS3**：CSS 變數、Flexbox、Grid、漸層、`backdrop-filter`、`clamp()`、Media Queries、動畫（`@keyframes`）。
- **Google Fonts**：Inter、Cormorant Garamond、Noto Serif TC。
- 少量原生 JavaScript（無任何框架）：產生星空背景、卷動淡入效果、自動顯示當前年份。

整個網站只有一個檔案 `index.html`，不需要安裝任何套件或建置工具。

## 如何用瀏覽器開啟

**方法一：直接開啟檔案**

1. 下載或 clone 此專案：
   ```bash
   git clone https://github.com/giwaslin/claude-lab.git
   ```
2. 進入資料夾，用滑鼠雙擊 `index.html`，即會以預設瀏覽器開啟。
   - 或在終端機執行（macOS）：`open index.html`
   - Windows：`start index.html`

**方法二：使用本機伺服器（選用）**

```bash
cd claude-lab
python3 -m http.server 8000
```

接著在瀏覽器開啟 <http://localhost:8000>。

> 提示：想預覽手機版效果，可在 Chrome 按 `F12`（macOS 為 `Cmd + Option + I`）開啟開發者工具，再點選「裝置工具列」圖示切換成手機尺寸。

## 檔案結構

```
claude-lab/
├── index.html   # 網站主頁（HTML + CSS + JS）
├── note.txt     # 筆記
└── README.md    # 專案說明
```
