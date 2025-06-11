# 🧑‍💻 Astro 個人網站 | Portfolio

這是一個使用 [Astro](https://astro.build/) 打造的現代化個人網站，聚焦於個人品牌展示與內容分享。支援響應式設計、深色模式切換與波浪動畫效果，並整合作品集、筆記、推薦資源與聯絡表單，方便訪客快速了解你並建立聯繫。

---

## ✨ 功能介紹

- **首頁**：漸層背景設計，快速導航卡片，展示個人品牌與核心功能。
- **關於我**：包含自我介紹、專業技能展示、學習經歷時間線。
- **作品集**：展示 6 個代表性作品，含圖片、技術標籤與連結，支援 3D 卡片效果。
- **推薦資源**：書籍推薦 + 影片課程，建立專業形象與內容延伸。
- **我的筆記**：技術文章分享，包含開發流程與 AI 應用經驗。
- **聯絡我**：Email 表單、社群連結與 FAQ，提供多元聯絡管道。
- **深色模式切換**：波浪擴散動畫效果，平滑切換亮/暗色主題。
- **導覽列動畫**：滑動底線效果，hover 時優雅的視覺回饋。
- **RWD 響應式設計**：手機、平板、桌機皆適配，流暢的互動體驗。
- **現代化 UI**：卡片 hover 效果、技能標籤動畫、3D 變換等豐富視覺效果。

---

## 🛠 技術棧

| 分類 | 技術            | 備註                 |
| ---- | --------------- | -------------------- |
| 框架 | Astro v4        | 極速靜態站點生成器   |
| 樣式 | Tailwind CSS v3 | 支援 RWD 與暗黑模式  |
| 語言 | TypeScript      | 類型安全與開發體驗   |
| 動畫 | CSS3 Animation  | 波浪效果、3D 變換    |
| 部署 | Netlify         | 雲端快速部署         |
| 圖示 | Heroicons / SVG | 內聯 SVG 圖標系統    |
| 表單 | Netlify Forms   | 含 honeypot 防護機制 |

---

## 📁 專案結構

```
personal-website/
├─ public/                # 靜態資源
│  ├─ Portfolio1-5.png    # 作品集圖片
│  ├─ Headsticker.png     # 個人照片
│  ├─ course1-2.*         # 課程推薦圖片
│  ├─ movie1-2.*          # 影片推薦圖片
│  └─ testimonials1-6.png # 書籍推薦圖片
├─ src/
│  ├─ components/         # UI 元件
│  │  ├─ Layout.astro     # 主要佈局
│  │  ├─ Navbar.astro     # 導航列（含主題切換）
│  │  └─ Footer.astro     # 頁尾
│  ├─ pages/              # 路由頁面
│  │  ├─ index.astro      # 首頁
│  │  ├─ about.astro      # 關於我
│  │  ├─ portfolio.astro  # 作品集
│  │  ├─ notes.astro      # 我的筆記
│  │  ├─ recommendations.astro # 推薦資源
│  │  └─ contact.astro    # 聯絡我
│  ├─ layouts/            # 佈局模板
│  └─ styles/             # 全域樣式
│     └─ global.css       # 動畫效果與主題
├─ astro.config.mjs       # Astro 設定
├─ tailwind.config.cjs    # Tailwind 設定
├─ package.json           # 專案依賴
└─ netlify.toml           # 部署設定
```

---

## 🚀 快速開始

### 本地開發

1. **克隆倉庫**

   ```bash
   git clone https://github.com/dianyike/personal-website.git
   cd personal-website
   ```

2. **安裝依賴**

   ```bash
   npm install
   ```

3. **啟動開發服務器**

   ```bash
   npm run dev
   ```

   預設在 `http://localhost:4321` 打開

4. **建立生產版本**
   ```bash
   npm run build
   npm run preview
   ```

### 部署到 Netlify

#### 自動部署（推薦）

1. Fork 此倉庫到你的 GitHub 帳戶
2. 登入 [Netlify](https://netlify.com) 並連接 GitHub
3. 選擇你的倉庫，Netlify 會自動偵測設定：
   - **Build command**: `npm run build`
   - **Publish directory**: `dist`
4. 點擊 "Deploy" 完成！

#### 手動部署

```bash
# 建立生產版本
npm run build

# 安裝 Netlify CLI
npm install -g netlify-cli

# 登入並部署
netlify login
netlify deploy --prod --dir=dist
```

### 表單設定

聯絡表單使用 **Netlify Forms**，部署後會自動啟用：

- 📧 提交內容會出現在 Netlify 管理面板的 "Forms" 頁籤
- 🛡️ 內建 honeypot 防護機制，有效防止垃圾郵件
- 📨 可設定通知信箱接收表單提交

---

## 📄 授權條款

本專案採用 [MIT License](LICENSE)。您可自由使用、修改與散佈本專案，但請保留原作者資訊。

---

## 🤝 貢獻指南

歡迎任何形式的貢獻！請依循以下流程進行：

1. Fork 本倉庫
2. 建立分支：`git checkout -b feat/your-feature`
3. 提交修改：`git commit -m "feat: 新增某某功能"`
4. 推送分支：`git push origin feat/your-feature`
5. 發起 Pull Request

請遵循 [Conventional Commits](https://www.conventionalcommits.org/) 命名規範。

---

## 📬 聯絡方式

- GitHub: [你的用戶名](https://github.com/dianyike)
- Email: dianyike1013@gmail.com

感謝您的使用與支援！

📄 本專案 README 內容由 ChatGPT 協助生成，根據實際功能與原始程式碼進行整理與撰寫，並經作者審閱修正。

🧠 部分功能模組使用 [Cursor](https://www.cursor.com/cn) 編輯器進行撰寫與調整，其 AI 輔助功能有效提升開發效率與程式碼品質。
