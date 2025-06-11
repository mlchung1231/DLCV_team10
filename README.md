# DLCV_team10

## 雲端檔案

- **Model**
    - best_model_class.h5
    - best_model_crack.pth
    - best_model_damage.pth
- **Dataset**
    - crack_classification
    - damage_classification_forTrain
    - damage_detection (檔案太大無法上傳)

## 檔案結構

下載完雲端檔案後，請確保資料夾結構如下：
```
DLCV_team10/
│
├── crack_classification/
│ ├── original/
│ ├── resized/
│
├── damage_classification_forTrain/
│ ├── beam_damage/
│ ├── column_damage/
│ ├── wall_damage/
│
├── damage_detection/
│ ├── 3class
│ ├── 4class(trial and wall only)
│
├── test_data/
|
├── best_model_class.h5
├── best_model_crack.pth
├── best_model_damage.pth
|
├── HW4_class.ipynb
├── HW4_crack.ipynb
├── HW4_damage.ipynb
├── HW4_predict.ipynb
|
├── team_10.yml
├── README.md
```

## 安裝環境

### 使用 Anaconda 建立虛擬環境

開啟 Anaconda Prompt，並使用以下指令建立一個新的虛擬環境：

```bash
conda env create -f your_path/team_10.yml
```

## 執行程式
### 訓練模型(可選)
選擇環境名稱為`team_10`，分別執行 `HW4_class.ipynb` 、 `HW4_crack.ipynb` 、 `HW4_damage.ipynb` 三個程式後，可得 `best_model_class.h5` 、 `best_model_crack.pth` 、 `best_model_damage.pth` 三個模型。(`damage`因資料太大無法上傳，請直接使用`best_model_damage.pth`)

### 預測結果上傳
同樣選擇環境名稱為`team_10`，執行 `HW4_predict.ipynb` 後，會在`./test_data/`中生成`beam.csv`、`column.csv`、`wall.csv`的預測結果。

