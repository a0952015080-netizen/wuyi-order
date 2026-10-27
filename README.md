# WUYI Cake 當週公版蛋糕訂購

線上公版蛋糕訂購系統，提供三步驟流暢訂購體驗，填寫完成後自動產生純文字明細並跳轉至 LINE 官方帳號進行客服報價確認。

## ✨ 特色功能

1. **三步驟訂購流程**：
   - 步驟 1：公版照片卡片直接勾選與點擊放大檢視。
   - 步驟 2：完全隨機口味安排（附忌口與過敏備註欄）、緞帶顏色更換。
   - 步驟 3：加購品項、取貨日期與自取時段、訂購人聯絡資料、注意事項打勾確認。

2. **跨專案多網站總控台（4 大專案一鍵管理）**：
   - **支援的專案網站**：
     1. 🎂 客製蛋糕預訂單：`https://a0952015080-netizen.github.io/wuyi-order/`
     2. 🔥 當週公版蛋糕：`https://a0952015080-netizen.github.io/wuyi-cakethisweek/`
     3. 🍔 漢堡盒蛋糕：`https://a0952015080-netizen.github.io/wuyi-burger/`
     4. 🌸 鮮花蛋糕：`https://a0952015080-netizen.github.io/wuyi-flower2/`
   - **自動識別**：開啟任一網站時，後台自動切換至該網站所屬的 GitHub 儲存庫。
   - **單獨管理**：可在下拉選單選擇特定網站，只修改該網站的日期。
   - **⚡ 一鍵同步全部 4 個網站**：全店統一休假時，只要勾選「同步推送到全部 4 個網站」，點擊一次儲存，系統透過 GitHub API 一口氣同步 4 個儲存庫的 `schedule.json`！

3. **如何設定 GitHub API Token（只需設定一次，全專案通用）**：
   1. 登入 GitHub，點擊右上角頭像 ➔「**Settings**」。
   2. 頁面左側滑到底部 ➔ 點「**Developer settings**」。
   3. 點選「**Personal access tokens**」➔「**Tokens (classic)**」➔「**Generate new token (classic)**」。
   4. Note 填寫 `wuyi-cake`，Expiration 選 `No expiration`（無期限），勾選 `repo`（完整儲存庫寫入權限）。
   5. 點擊綠色「**Generate token**」，將產生的 `ghp_...` 貼在任一網站後台的 Token 欄位。
   6. 該 Token 在您名下所有儲存庫（wuyi-order / wuyi-burger / wuyi-cakethisweek / wuyi-flower2）完全通用！

4. **LINE 訂單純文字格式（無 Emoji）**：
   - 跳轉至 LINE 或點擊複製訂單明細時，自動過濾並移除所有 Emoji 表情符號，呈現乾淨俐落的純文字排版，方便客服複製與建檔。
