# 幾點了，還在看手機？！

健康資訊管理課程期中報告：每日解鎖次數與學生讀書、運動時間的關係，作為自律 app 的設計依據。

- 報告網站：https://alan900206.github.io/social_media_unlock_study/
- 互動儀表板（Tableau Public）：https://public.tableau.com/app/profile/chih.yung.wang/viz/_17957643213190/sheet3

## 主要發現

- 每日解鎖次數與讀書時數呈明顯負相關（r = −0.85），高中、大學、研究所三組皆然。
- 解鎖 ≥240 次的學生平均每天只讀書 1.1 小時，<120 次的學生有 5.5 小時。
- 沒有學生「每天用 ≥7 小時又讀書 ≥4 小時」。
- 平台與使用目的差異很小，關鍵在打開手機的頻率。

## 檔案

| 路徑 | 說明 |
|---|---|
| `index.html` | 報告網頁（嵌入 Tableau 儀表板） |
| `data/student_social_media_clean.csv` | 整理後資料，5,000 筆 × 21 欄 |

## 資料

Kaggle「Student Social Media & Mental Health Impact」（CC BY-SA）。此資料集很可能為合成資料，結果僅供趨勢參考，不代表因果關係。

整理步驟：運動時數 10 筆負值修正為 0（`PA_Fixed_Flag` 標記）；新增使用時數、解鎖次數、讀書時數分組，以及「平均幾分鐘解鎖一次」等衍生欄位。

## 工具

生成式 AI（Claude）協助資料清理與分析；Tableau 製作儀表板。
