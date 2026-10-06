# 社團檔案整理報告 (Club Files Organization Report)

## 一、整理概述
- **輸入檔案總數**：12 個文字檔
- **整理後副本總數**：12 個檔案（完整保留原檔與所有副本，無刪除、無覆蓋）
- **建議分類**：
  1. nnouncements/：活動公告、文宣及副本
  2. proposals/：活動企畫草案（不同版本）及雨天備案
  3. planning_and_notes/：會議紀錄、後續待辦事項及回饋問卷
  4. 
esources_and_budget/：預算草案與器材清單副本

---

## 二、檔案整理清單與分類

| 原始檔案 (source) | 分類目的路徑 (destination) | 分類理由 (reason) |
|---|---|---|
| nnouncement.txt | nnouncements/announcement.txt | 活動宣傳與通知資訊 |
| nnouncement_copy.txt | nnouncements/announcement_copy.txt | 活動宣傳與通知資訊（與 announcement.txt 內容完全相同之副本，予以保留） |
| poster_text.txt | nnouncements/poster_text.txt | 活動文宣與宣傳短語 |
| proposal_final.txt | proposals/proposal_final.txt | 活動企畫第一版（戶外活動30分鐘，內容註明尚未定案） |
| proposal_final2.txt | proposals/proposal_final2.txt | 活動企畫第二版（室內活動20分鐘，內容註明仍待討論） |
| 
ain_plan.txt | proposals/rain_plan.txt | 雨天備案規劃 |
| meeting_notes.txt | planning_and_notes/meeting_notes.txt | 社團幹部會議討論紀錄 |
| 
ext_steps.txt | planning_and_notes/next_steps.txt | 後續執行與比對兩版企畫之指引 |
| eedback_questions.txt | planning_and_notes/feedback_questions.txt | 活動回饋問卷題目設計 |
| udget_draft.txt | 
esources_and_budget/budget_draft.txt | 活動預算模擬草案 |
| quipment_list.txt | 
esources_and_budget/equipment_list.txt | 活動所需器材清單 |
| quipment_backup.txt | 
esources_and_budget/equipment_backup.txt | 活動器材備份清單（與 equipment_list.txt 內容完全相同之副本，予以保留） |

---

## 三、重複與版本分析

### 1. 內容完全相同之重複檔案（經 SHA-256 雜湊驗證）
- nnouncement.txt 與 nnouncement_copy.txt：
  - SHA-256：c19164b1f6dbbb97390979e27c1f8a8bb231f8f121d51a66e4a2d88efbcf9dfd
  - 狀態：兩者文字內容一致。已全部保留在 nnouncements/ 分類中。
- quipment_list.txt 與 quipment_backup.txt：
  - SHA-256：c21d53ba5fa8d7a1262d1421f158aa5d045d6a4548aa2185c7c1dae2a77a9446
  - 狀態：兩者文字內容一致。已全部保留在 
esources_and_budget/ 分類中。

### 2. 名稱相近但內容不同之不同版本
- proposal_final.txt vs proposal_final2.txt：
  - proposal_final.txt：內容為「企畫第一版：戶外活動，30分鐘。尚未定案。」
  - proposal_final2.txt：內容為「企畫第二版：室內活動，20分鐘。仍待討論。」
  - **重要提醒**：依規則不以檔名中的 inal 或修改時間認定定稿。兩份企畫主題（室外 vs 室內）與時間長度不同，且皆標明尚未定案，因此兩者皆完整保留在 proposals/。

---

## 四、待確認問題（需人工作出判斷事項）
1. **企畫定案選擇**：需由社團會議比對 proposal_final.txt 與 proposal_final2.txt，決定採用戶外方案或室內方案。
2. **公告時間地點**：nnouncement.txt 中註記「時間與地點未定」，需待企畫定案後補齊資訊再正式發布。
3. **重複副本處置**：重複檔案（nnouncement_copy.txt、quipment_backup.txt）確認不影響存檔後，是否移入歷史封存區。

---

## 五、實際檢查與未確認事項

### 實際做過的檢查
- [x] 原 input/ 資料夾中 12 個檔案原封不動，大小與內容未受任何變更。
- [x] output/ 各分類資料夾中 12 個副本完整產生，SHA-256 雜湊與原檔逐一比對 100% 吻合。
- [x] 成功產生 output/manifest.json，且包含 12 筆物件，每筆具備 source、destination、
eason。
- [x] 未安裝任何外部套件、未進行網路請求、未碰觸題目範圍外的檔案。

### 還沒確認的部分
- [ ] 兩版企畫的最終採納方案（需由幹部開會決定）。
- [ ] 預算草案與器材數量是否已獲學校／指導老師核可。
