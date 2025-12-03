# 作業說明（README）

> 本作業以**預測病患適用藥物種類（Drug）**為主題。請從 `sample_code.ipynb` 起步，熟悉資料與評估流程，依規則完成 baseline 與模型改進，並撰寫報告。

---

## 1) 作業介紹

- **任務**：根據病患的生理資訊預測適用的藥物種類 **Drug**（分類問題）。
- **評估指標**：**Accuracy（準確率）**。所有分數均以評測平台的結果為準。
- **實作重點**
  1. 讀取並理解資料；完成必要的清理與轉換  
  2. 建立合適的分類模型並進行本地驗證  
  3. 產出正確格式的提交檔上傳評測  
  Kaggle網址：https://www.kaggle.com/t/f08cc09ab0c44e21a8aa265f4d75af1f
- **起始範例**：`sample_code.ipynb` 僅提供讀檔寫檔，你需要在此基礎上自行改進。

---

## 2) 資料集與特徵

- **檔案結構**
  ```
  data/
    ├─ train.csv      # 訓練資料（含 Drug 目標欄位）
    └─ test.csv       # 測試資料（不含 Drug）
  sample_code.ipynb
  ```

- **欄位概述**
  * `Age`: 病患年齡
  * `Sex`: 性別 (M: 男性, F: 女性)
  * `BP`: 血壓 (LOW: 低, NORMAL: 正常, HIGH: 高)
  * `Cholesterol`: 膽固醇 (NORMAL: 正常, HIGH: 高)
  * `Na_to_K`: 血液中鈉與鉀的比例
  * `Drug`: **(預測目標)** 適用的藥物種類 (DrugY, drugX, drugA, drugB, drugC)

---

## 3) 評分規則（總分 12 分）

1. **Simple Baseline（3 分）**  
   - 依作業說明完成**必要的輕量改動**與基本前處理，並**通過 public easy baseline**。

2. **Medium Baseline（3 分）**  
   - 在簡單基線之上做**更完整的調整／特徵設計／模型設定**，並**通過 public medium baseline**。

3. **報告（6 分）**  
  - 第一部分：準確度分數 (Accuracy Scores) (1分)  
  - 第二部分：我的實驗記錄 (My Experiment Log) (3分)  
  - 第三部分：總結與心得 (Conclusion & Reflection) (2分)  
  （請參考`sample_code.ipynb`的報告部分）
