```mermaid
graph TD
    1[研擬計畫 (4天)] --> 2[任務分配 (1天)]
    1 --> 3[取得硬體 (17天)]
    2 --> 4[程式開發 (70天)]
    3 --> 5[安裝硬體 (3天)]
    4 --> 6[程式測試 (30天)]
    5 --> 7[撰寫使用手冊 (25天)]
    6 --> 8[轉換檔案 (20天)]
    5 --> 9[系統測試 (25天)]
    7 --> 10[使用者訓練 (20天)]
    8 --> 10
    9 --> 11[使用者測試 (25天)]
    10 --> 11


---

### (2) 甘特圖
```markdown
```mermaid
gantt
    title 甘特圖 - 作業2
    dateFormat  YYYY-MM-DD
    axisFormat  %m/%d

    section 任務
    研擬計畫         :a1, 2025-10-01, 4d
    任務分配         :a2, after a1, 1d
    取得硬體         :a3, after a1, 17d
    程式開發         :a4, after a2, 70d
    安裝硬體         :a5, after a3, 3d
    程式測試         :a6, after a4, 30d
    撰寫使用手冊      :a7, after a5, 25d
    轉換檔案         :a8, after a6, 20d
    系統測試         :a9, after a5, 25d
    使用者訓練       :a10, after a7, 20d
    使用者測試       :a11, after a9, 25d
