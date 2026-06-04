# 🤖 OpenClaw AI Agent

> 「AI 不再只是聊天機器人，而是一個能幫你做事的數位員工。」

---

## 一、OpenClaw 是什麼？

OpenClaw 是一個開源的 AI Agent 框架，由奧地利開發者 **Peter Steinberger** 創建。截至 2026 年 1 月，GitHub 已超過 **45,000 顆星**，社群技能市集 ClawdHub 有超過 **2,300 個**可重用的工作流。

**核心理念**：AI 不只是回答問題，而是能「讀取檔案、執行指令、操作 API、瀏覽網頁、管理排程」的**自主代理人**。

### 🔗 重要連結

- 📖 [官方文件](https://docs.openclaw.ai)
- 🐙 [GitHub](https://github.com/openclaw/openclaw)
- 🛒 [技能市集 ClawHub](https://clawhub.com)
- 🇹🇼 [台灣開放資料工具](https://hub.twinkleai.tw/skills/tw-opendata-tools)
- [風險：API金鑰遭竊「2天噴掉260萬」](https://tw.stock.yahoo.com/news/%E4%BB%96api%E9%87%91%E9%91%B0%E9%81%AD%E7%AB%8A-2%E5%A4%A9%E5%99%B4%E6%8E%89260%E8%90%AC-3%E4%BA%BA%E5%B0%8F%E5%85%AC%E5%8F%B8%E9%9D%A2%E8%87%A8%E7%A0%B4%E7%94%A2%E5%8D%B1%E6%A9%9F-102100094.html)

---

## 二、創始人的故事

Peter Steinberger 認為：

> 「以前學編程，你得看書、看教程、做練習題，枯燥得要命。但現在有了 AI，你想做個網站、做個小工具，你直接就去做。不懂的你就邊做邊問 AI，做着做着你就懂了。」

這就是 OpenClaw 的精神——**降低技術門檻，讓每個人都能用自然語言驅動自動化**。

- 📖 [文字版介紹](https://www.binance.com/zh-TC/square/post/298256668078434)
- 🎬 [影片版介紹](https://www.facebook.com/watch/?v=1608171953553214)

---

## 三、跟傳統 AI 有什麼不同？

| 特性 | 傳統 AI (ChatGPT) | OpenClaw AI Agent |
|------|-------------------|-------------------|
| 互動方式 | 你問它答 | 你說它做，主動執行 |
| 工具使用 | 只能聊天/生成圖片 | 讀寫檔案、執行指令、呼叫 API |
| 記憶能力 | 每次對話獨立 | 長期記憶 + 日誌檔案 |
| 排程任務 | 不支援 | Cron job 自動排程 |
| 多平台整合 | 有限 | Telegram/Discord/Gmail/Sheets 等 |

---

## 四、實際應用案例（10 個場景）

### 案例 1：🌤️ 每日天氣預報推送

- **情境**：每天早上要知道會不會下雨
- **做法**：Cron job 每天 06:00 自動抓中央氣象署資料 → 整理三時段預報 + 穿衣建議 → 推送到 Telegram
- **效果**：起床就能看，不用開任何 app
<img width="364" height="451" alt="2026-06-04_113330" src="https://github.com/user-attachments/assets/380165a1-0f10-425b-ad74-15216f03a3e5" />



### 案例 2：🔌 水電帳單自動記錄

- **情境**：Gmail 收到台電帳單 email，手動抄金額很煩
- **做法**：偵測帳單 email → 自動提取金額/電號 → 寫入 Google Sheets
- **效果**：完全自動，還能計算信用卡回饋
[電費趨勢_echarts.html](https://github.com/user-attachments/files/28584413/_echarts.html)

### 案例 3：🎓 Excel 報表線上化

- **情境**：教育訓練成果報表化
- **做法**：Python 轉前端 JS + SheetJS → 網頁匯入 Excel → 自動比對
- **效果**：GitHub Pages 部署 (https://github.com/jackytslin8)
<img width="1334" height="601" alt="2026-06-04_133436" src="https://github.com/user-attachments/assets/64d22af3-257d-4dc0-b665-153e3799c6e3" />

### 案例 4：🏠 房屋修繕費用追蹤

- **情境**：整修工程廠商報價格式雜亂
- **做法**：ocr辨識、建立比較表
- **效果**：比較建議，一目了然
- <img width="506" height="232" alt="2026-06-04_134237" src="https://github.com/user-attachments/assets/d9e0e5e5-80b8-40d4-8320-96b0fa04c21d" />
<img width="497" height="228" alt="2026-06-04_134258" src="https://github.com/user-attachments/assets/f41beeed-1b64-41f6-8a7d-79d08f3bc2ce" />
<img width="1091" height="288" alt="2026-06-04_134426" src="https://github.com/user-attachments/assets/9ecb2234-7679-4721-bbdd-b1d068a5540a" />

### 案例 5：🎮 做遊戲互動

- **情境**：想快速做一個小遊戲
- **做法**：自然語言描述需求 → AI 寫出網頁遊戲（消消樂、暗棋）
- **效果**：幾分鐘內完成可玩的遊戲
[消消樂.html](https://github.com/user-attachments/files/28584778/default.html)
[暗棋_Longcat.html](https://github.com/user-attachments/files/28584871/_Longcat.html)

## 五、更多創意應用點子

- 📍 即時查詢附近的 YouBike 站點和可借數量
- 🚂 台鐵即時誤點資訊查詢
- 📸 每月電錶拍照 → OCR 辨識 → 自動寫入報表
- 📰 每日 AI 科技新聞摘要自動推送
- 💰 投資信號追蹤：監控 SEC 文件 + 社群情緒
- 🎬 YouTube/播客自動摘要，重點存入筆記
- 🏢 招募流程自動化：篩選履歷 → 排面試 → 追蹤
- 🏥 醫療報告解讀 + 健康趨勢追蹤
- ✈️ 自動規劃旅遊行程：比價、訂房、排景點
- 📦 電商訂單自動處理 + 庫存監控

---

## 六、技能市集（ClawHub https://clawhub.ai/skills / Twinkle Hub https://hub.twinkleai.tw/skills）

OpenClaw 的強大之處在於「技能」——可重用的工作流模組。社群已貢獻超過 **2,300 個技能**：

- 🌐 **agent-reach**：搜尋 Twitter、Reddit、YouTube、GitHub 等 16+ 平台
- 📊 **tw-opendata-tools**：查詢台灣 53,000 個政府開放資料集
- ⚖️ **tw-opendata-judicial**：查詢 600 萬筆判決書
- 🔍 **tw-opendata-patent**：TIPO 28 萬+ 專利檢索
- 🏠 **tw-opendata-realestate**：實價登錄房價查詢
- 🌤️ **weather**：即時天氣預報
- 📝 **notion**：Notion API 整合
- 📧 **gog**：Google Workspace（Gmail/Calendar/Drive/Sheets）
- 🎤 **sag / mimotts25**：文字轉語音
- 📄 **nano-pdf**：自然語言編輯 PDF

---

## 七、總結：AI Agent 的核心價值

> 把「每天都要做的瑣事」變成「自動發生的事」。

1. **自動化重複性工作**，釋放時間做更有價值的事
2. **24/7 全天候運作**，不會忘記、不會遲到
3. **跨平台整合**，把散落的資訊串在一起
4. **持續學習和記憶**，越用越懂你

---

📅 建立日期：2026-06-04
