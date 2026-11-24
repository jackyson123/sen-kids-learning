# 教材包（Content Packs）

SEN 兒童學習嘅教材唔再只係痴喺 `index.html` 入面，而係分拆成呢度嘅 JSON 檔案。
App 會讀呢啲檔案嚟顯示內容；加新教材包，只需要喺 `packs/` 加一個新檔案。

## 檔案格式

每個教材包係一個 JSON 檔案，結構如下：

```json
{
  "id": "transport",
  "version": 1,
  "title": { "yue": "交通篇", "en": "Transport" },
  "description": { "yue": "簡介", "en": "Short description" },
  "words": [
    { "zh": "巴士", "en": "bus", "emoji": "🚌" }
  ],
  "cards": [
    { "zh": "我要搭巴士", "en": "I want to take the bus", "emoji": "🚌" }
  ],
  "story": {
    "title": { "yue": "搭巴士守則", "en": "Bus rules" },
    "steps": [
      { "zh": "排隊等巴士，唔好推人。", "en": "Queue for the bus. Do not push.", "emoji": "🧍" }
    ]
  }
}
```

## 欄位說明

| 欄位 | 意思 |
| --- | --- |
| `id` | 教材包代號，英文細階，唔可以有空格 |
| `version` | 版本號，改內容就加 1 |
| `title.yue` / `title.en` | 粵語名 / 英文名 |
| `description` | 簡介，粵語同英文 |
| `words` | 識字遊戲詞彙：中文字、英文、emoji |
| `cards` | 溝通圖卡：中文句、英文、emoji |
| `story` | 社交故事：標題 + 步驟（每步中文、英文、emoji） |

## 現有教材包

| 檔案 | 內容 |
| --- | --- |
| `packs/transport.json` | 交通篇 — 巴士、的士、地鐵、搭車守則 |
| `packs/food.json` | 食物篇 — 蘋果、飯、麵、食飯禮儀 |
| `packs/school.json` | 學校篇 — 書包、老師、上堂守則 |
| `packs/animals.json` | 動物篇 — 狗、貓、獅子、去動物園守則 |
| `packs/body.json` | 身體篇 — 頭、手、腳、眼、認識身體 |
| `packs/colors.json` | 顏色篇 — 紅、黃、藍、綠、顏色遊戲 |
| `packs/family.json` | 家庭篇 — 爸爸、媽媽、哥哥姐姐、我的一家 |
| `packs/jobs.json` | 職業篇 — 醫生、老師、警察、長大想做咩 |
| `packs/weather.json` | 天氣篇 — 太陽、雨、風、天氣點著衫 |
| `packs/festivals.json` | 節日篇 — 新年、聖誕、中秋、過節要做咩 |
| `packs/numbers.json` | 數字篇 — 一、二、三、數數遊戲 |
| `packs/fruits-veg.json` | 水果蔬菜篇 — 蘋果、香蕉、蘿蔔、食得健康 |
| `packs/vehicles.json` | 交通工具篇 — 巴士、地鐵、電車、搭車守則 |

## 家長分享內容

家長自訂嘅圖卡、詞彙可以用 App 入面「備份同分享」匯出 JSON。
想分享俾其他家長用，可以去 repo 嘅 Discussions「家長分享區」貼上檔案，
版主睇過之後會加入教材包。分享內容只可以係你自己整嘅圖卡，唔好放小朋友相片或個人資料。
