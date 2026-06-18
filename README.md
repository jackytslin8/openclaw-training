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
- 影片節錄 (https://streamable.com/nvw8fj)

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

## 四、實際應用案例

### 案例 1：🌤️ 每日天氣預報推送

- **情境**：每天早上要知道會不會下雨
- **做法**：Cron job 每天 06:00 自動抓中央氣象署資料 → 整理三時段預報 + 穿衣建議 → 推送到 Telegram
- **效果**：起床就能看，不用開任何 app
<img width="364" height="451" alt="2026-06-04_113330" src="https://github.com/user-attachments/assets/380165a1-0f10-425b-ad74-15216f03a3e5" />



### 案例 2：🔌 水電帳單自動記錄

- **情境**：Gmail 收到台電帳單 email，想看長期用電狀況，手動整理很麻煩
- **做法**：偵測帳單 email → 自動提取金額/電號 → 寫入 Google Sheets
- **效果**：全自動，且提供完整報表
- [電費趨勢](https://jackytslin8.github.io/openclaw-training/case9/%E9%9B%BB%E8%B2%BB%E8%B6%A8%E5%8B%A2.html)


### 案例 3：🎓 Excel 報表線上化

- **情境**：教育訓練成果報表化
- **做法**：Python 轉前端 JS + SheetJS → 網頁匯入 Excel → 自動比對
- **效果**：GitHub Pages 部署 (https://github.com/jackytslin8)
<img width="1334" height="601" alt="2026-06-04_133436" src="https://github.com/user-attachments/assets/64d22af3-257d-4dc0-b665-153e3799c6e3" />

### 案例 4：🏠 房屋修繕費用追蹤

- **情境**：整修工程廠商報價格式雜亂
- **做法**：ocr辨識、建立比較表
- **效果**：比較建議，一目了然

<img width="506" height="232" alt="2026-06-04_134237" src="https://github.com/user-attachments/assets/4f2f5ad3-7377-4428-9316-463d36e53287" />
<img width="497" height="228" alt="2026-06-04_134258" src="https://github.com/user-attachments/assets/4f38c52e-7b2b-40f0-832e-7581d87b8b6a" />
<img width="1003" height="276" alt="2026-06-04_140540" src="https://github.com/user-attachments/assets/be0896cc-7c00-4387-909f-4c4464efe7ed" />


### 案例 5：🎮 做遊戲互動

- **情境**：想快速做一個小遊戲
- **做法**：自然語言描述需求 → AI 寫出網頁遊戲（消消樂、暗棋）
- **效果**：幾分鐘內完成可玩的遊戲
[消消樂](https://jackytslin8.github.io/openclaw-training/case9/消消樂.html)
[暗棋_Longcat](https://jackytslin8.github.io/openclaw-training/case9/暗棋_Longcat.html)

### 案例 6：🚲︎ 即時Ubike數量查詢

- **情境**：想查詢即時ubike站點資訊
- **做法**：自然語言描述，例：目前力行路23號上的ubike站點，可借的腳踏車資訊
- **效果**：透過API，提供即時資訊
 <img width="457" height="413" alt="image" src="https://github.com/user-attachments/assets/3659b06d-46c7-41f1-84d0-1b05390b8575" />
<img width="470" height="98" alt="image" src="https://github.com/user-attachments/assets/0bf2f476-3eea-4e56-94da-a467a6edf3fe" />

### 案例 7：🏘️ 實價登錄查詢

- **情境**：想查詢土地實價登錄資訊
- **做法**：prompt：幫我新增twinkle hub ("https://hub.twinkleai.tw/dashboard") 
api key：xxxxxxx
- **效果**：透過twinkle hub API查詢，例：新竹市力行路23號的實價登錄
<img width="472" height="276" alt="image" src="https://github.com/user-attachments/assets/86c6ad76-c449-4cd7-89b2-8e4188ba3b51" />
<img width="466" height="342" alt="image" src="https://github.com/user-attachments/assets/5b2c8d7a-7d5f-4f34-b6ee-a102062f4b32" />
<img width="464" height="412" alt="image" src="https://github.com/user-attachments/assets/0963ded0-9e9a-4b12-a05e-c3fe3d6fa637" />

### 案例 8：✍️ 寫腳本自動簽到
- **情境**：某網站每天自動簽到賺點數
- **做法**：openclaw插件 **Playwright + chromium**，無頭瀏覽器, chrome新增擴充功能：Get cookies.txt LOCALLY (下載cookies用)
- **效果**：寫腳本，自動搶LonCat內測名額 (演唱會門票！？ 嘘~~<img width="24" height="24" alt="1f92b" src="https://github.com/user-attachments/assets/624537c1-81d5-467f-bb67-b783853595ec" />
)
<img width="399" height="614" alt="2026-06-05_103102" src="https://github.com/user-attachments/assets/c3edc4cc-ccdd-4efc-b356-5d428a401e10" />
<img width="306" height="503" alt="image" src="https://github.com/user-attachments/assets/9f277e7c-5759-43ee-b13e-2147849b7a27" />
<img width="297" height="585" alt="image" src="https://github.com/user-attachments/assets/49d1adae-38b3-4a63-ad61-fdbd3a833b6f" />

### 案例 9：👩‍⚕ 中華民國30年來出生率vs死亡率變化
- **情境**：Chart.js 趨勢圖 — 30 年出生率vs死亡率變化一目瞭然
- **做法**：新增twinkle hub技能，詢問「30年來死亡率趨勢，合併出生率的圖表，html格式」
- **效果**：圖表上 2019 年有個明顯的 ✕ 標記，就是兩條線交叉的位置。滑鼠移上去可以看到每年的詳細數字。少子化 + 高齡化的「剪刀差」非常明顯 😬
- [📊 台灣出生 vs 死亡人數 — 30 年交叉趨勢](https://jackytslin8.github.io/openclaw-training/case9/taiwan_birth_death_30y_people.html)
- [📊 台灣出生 vs 死亡 — 2015~2026 最新趨勢](https://jackytslin8.github.io/openclaw-training/case9/taiwan_birth_death_2015_2026.html)

### 案例 10：🚂 臺鐵每日運輸量
- **情境**：2026/06/01（週日）日運輸量
- **做法**：prompt：查找昨天台鐵運輸量，openclaw自動透過台鐵api查找
- **效果**：查到後製作html
- [🛲 台鐵單日運輸量](https://jackytslin8.github.io/openclaw-training/case9/tra_20260601.html)

### 案例 11：🚂 比APP還要好用？
- **情境**：2026/7/1 火車時刻改點
- **做法**：prompt：7/1 火車時刻表即將改點，假設下班時間17:00，騎到竹中站停好車，大約17:15，如果要在19:00之前到苗栗，請列出最佳組合。TPASS不能坐自強號3000型，找html格式的火車時刻表 (OCR辨識PDF的火車時刻表，會失誤)
- **效果**：提供最佳搭車組合
<img width="273" height="607" alt="Screenshot_2026-06-12-17-25-17-634_tw gov tra twtraffic" src="https://github.com/user-attachments/assets/ab9447cd-946a-47bc-be90-7ae3ed4aa084" />
<img width="273" height="607" alt="Screenshot_2026-06-12-17-25-31-963_tw gov tra twtraffic" src="https://github.com/user-attachments/assets/99cab70b-1080-42f5-b3d2-e923437744d7" />
<img width="458" height="314" alt="2026-06-18_082052" src="https://github.com/user-attachments/assets/4be9375f-02d8-4e54-9de0-efb9fc6f03d8" />
<img width="465" height="245" alt="2026-06-18_081910" src="https://github.com/user-attachments/assets/a892ee2b-7192-4474-9ca9-2e016ac18fa1" />



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

---
