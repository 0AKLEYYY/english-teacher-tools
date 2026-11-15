# English Teacher Tools (英文教學工具庫)

這是一個專為英文老師打造的教學工具與課堂資源網站。

網站旨在整理英文教學中實用的工具與資源，讓老師在備課與課堂教學時能快速找到需要的輔助功能。

---

## 專案目的

1. **集中資源**：將常用教學工具集中在同一個網站，方便快速取用。
2. **操作直覺**：介面乾淨、簡單，方便老師操作，部分工具亦可直接在課堂投影供學生互動。
3. **持續擴充**：維持一致的版面風格與結構，方便未來持續新增多元的教學工具。
4. **輕量維護**：採用純靜態網頁技術（HTML / CSS / JavaScript），可直接透過 GitHub Pages 發布與瀏覽。

---

## 目前工具

- **English Word Match Game（英文單字配對遊戲）**：
  透過單字與圖片配對，讓學生複習基礎生活英文單字。
  [立即體驗遊戲](https://0akleyyy.github.io/english-word-match-game/)
- **Teaching Activities（課堂活動）**：
  整理適合課堂互動、破冰、文法與句型練習的教學活動。
- **Worksheets（學習單）**：
  提供可列印或線上使用的英文學習單與測驗練習資源整理。

---

## 專案資料夾結構

```text
english-teacher-tools/
│
├── AGENTS.md                   # 專案規範與 AI 開發規則
├── README.md                   # 專案說明文件
├── index.html                  # 網站首頁
│
├── css/
│   └── style.css               # 全站共用樣式表
│
├── pages/                      # 各教學工具正式頁面
│   ├── word-match-game.html    # 英文單字翻牌配對遊戲介紹頁
│   ├── teaching-activities.html # 課堂教學活動整理頁
│   └── worksheets.html         # 英文學習單分類整理頁
│
├── templates/
│   └── tool-page-template.html # 新工具頁面範本
│
└── assets/
    └── images/                 # 網站圖片素材
```

---

## 開發與擴充規範

新增工具或修改本專案時，請務必遵循 [AGENTS.md](AGENTS.md) 規範：
- 優先使用純原生 HTML、CSS 與 JavaScript，不引入大型前端框架。
- 所有工具頁面置於 `pages/` 目錄，檔名一律使用小寫英文與 `-` 連接號。
- 優先使用 `css/style.css` 共用樣式與既有 class。
- 每個工具內頁均需包含清晰的「回首頁」連結。
- 每新增一個正式工具頁面，需同步於 `index.html` 更新卡片入口。
