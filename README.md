# SEN 兒童學習

免費、開源嘅特殊教育需要（SEN）兒童學習網頁應用程式，畀家長、老師同治療師免費使用。

Free and open-source learning web app for children with special educational needs (SEN), for parents, teachers and therapists.

## 即刻用 / Try it now

- 🌐 主站：https://sen-kids-learning.vercel.app
- 📄 備份站（GitHub Pages）：https://jackyson123.github.io/sen-kids-learning/

## 版本 / Versions

- **v2.0**（2026-11-23）— 新增「教材包」頁：交通篇、食物篇、學校篇（生字、圖卡、社交故事）；教材分拆做獨立檔案即場載入，有內置後備；家長自訂內容加「家長共享內容庫」（匯出／匯入分享檔案）；家長專區加意見箱、家長交流區連結、版本紀錄、推廣分享；GitHub Pages 自動部署；意見範本
- **v1.0.0**（2026-11-23）— 首個版本：18 個學習活動、多語言、本地保存、離線安裝、匯入／匯出、打印圖卡、家長專區

## 用法 / How to use

直接喺瀏覽器開 `index.html`，或者用上面嘅網址，唔使安裝、唔使開帳戶、唔會上傳任何資料。

Open `index.html` in a browser, or use the links above. No install, no account, no data uploaded.

## 功能 / Features

18 個學習活動，包括：

- 認情緒、日常流程卡、識字遊戲、數數遊戲、社交故事、冷靜角落
- 溝通圖卡、情緒日記、專注力訓練、生活自理教學、獎勵貼紙簿、語言仿說
- 安全教學、感覺統合遊戲、時間概念、睡眠故事、家長自訂內容、進度報告

其他功能：

- **多語言**：粵語、普通話、英文介面同朗讀
- **本地保存**：星星、進度、日記、自訂內容儲存喺裝置瀏覽器
- **離線安裝**：可以加到手機主畫面，冇網絡都用到
- **匯入／匯出**：備份同分享自訂內容
- **打印圖卡**：將溝通圖卡、流程卡印出嚟做實體卡
- **家長專區**：進度統計、能力對應、陪玩貼士、常見問題

## 教材包 / Content packs

教材唔再只係痴喺 `index.html` 入面，而係分拆成 `data/packs/` 嘅 JSON 檔案，app 會讀取佢哋。
現有教材包：交通篇、食物篇、學校篇（每個包有識字詞彙、溝通圖卡同社交故事）。
加新教材包只需要喺 `data/packs/` 加一個檔案，格式睇 `data/README.md`。

## 意見同分享 / Feedback & sharing

- 🐛 有 bug 或者有嘢唔 work：開 [Issue](../../issues/new?template=bug_report.md) 話我哋知
- 💡 想加新功能、新教材：開 [Issue](../../issues/new?template=feature_request.md)
- 💬 家長交流、分享自訂圖卡：去 [Discussions](../../discussions) 嘅「家長分享區」
- 分享內容只可以係你自己整嘅圖卡，唔好放小朋友相片或個人資料。

## 貢獻 / Contributing

歡迎家長、老師、治療師幫手加生字、故事、活動建議。開 Issue 或者 Pull Request 就得。

Contributions are welcome — new words, stories, activities and suggestions via Issues or Pull Requests.

## 授權 / License

MIT License — 免費使用、修改同分享。
