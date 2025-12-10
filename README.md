# bwwpa_experiment

實作了二元水車植物演算法 (bWWPA)應用於特徵選擇的實驗。使用 KNN 分類器作為評估標準，並在 Zoo 與 Sonar 兩個公開資料集上進行效能測試。

## 1. 實驗環境 (Environment)

- **作業系統**: Windows 10
- **IDE**: Google Colab
- **程式語言**:Python 3.12.12
- **主要套件**:
  - `numpy`
  - `pandas`
  - `scikit-learn`

## 2. 資料集來源

程式碼會自動從 UCI Machine Learning Repository 下載資料，不需手動下載 CSV 檔。

1.  **Zoo Data Set**
    - **來源**: [UCI Zoo Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/zoo/zoo.data)
    - **描述**: 包含 101 種動物的特徵數據，用於動物分類任務。

2.  **Connectionist Bench (Sonar, Mines vs. Rocks) Data Set**
    - **來源**: [UCI Sonar Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/undocumented/connectionist-bench/sonar/sonar.all-data)
    - **描述**: 包含 208 筆聲納回波數據，用於區分岩石 (Rock) 與金屬 (Mine)。

## 3. 如何運行程式碼 

### 在 Google Colab 上執行 (推薦)

## 實驗參數設定 (Parameters)
程式碼預設參數如下，可於 `if __name__ == "__main__":`區塊中調整：
- **Zoo Dataset**: Runs=20, Population=20, Iterations=100
- **Sonar Dataset**: Runs=30, Population=20, Iterations=200
- **KNN k-neighbors**: 5 (Zoo), 9 (Sonar)
