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

## 家長分享內容

家長自訂嘅圖卡、詞彙可以用 App 入面「備份同分享」匯出 JSON。
想分享俾其他家長用，可以去 repo 嘅 Discussions「家長分享區」貼上檔案，
版主睇過之後會加入教材包。分享內容只可以係你自己整嘅圖卡，唔好放小朋友相片或個人資料。
