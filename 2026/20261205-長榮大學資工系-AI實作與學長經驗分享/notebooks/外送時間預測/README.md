# 外送時間預測

從生活認識 AI｜長榮大學資訊工程學系｜2026.12.05

用 1,000 筆模擬外送訂單的「距離」與「實際耗時」，訓練線性迴歸模型，預測新訂單的送達時間。

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andy6804tw/speech-archive/blob/main/2026/20261205-%E9%95%B7%E6%A6%AE%E5%A4%A7%E5%AD%B8%E8%B3%87%E5%B7%A5%E7%B3%BB-AI%E5%AF%A6%E4%BD%9C%E8%88%87%E5%AD%B8%E9%95%B7%E7%B6%93%E9%A9%97%E5%88%86%E4%BA%AB/notebooks/%E5%A4%96%E9%80%81%E6%99%82%E9%96%93%E9%A0%90%E6%B8%AC/%E5%A4%96%E9%80%81%E9%82%84%E8%A6%81%E5%A4%9A%E4%B9%85%E6%89%8D%E6%9C%83%E5%88%B0.ipynb)

## 開始練習

1. 點選上方徽章，在 Google Colab 開啟教材。
2. 從第 1 步開始，依序按下各程式區塊左側的 **▶**。
3. 最後改變外送距離，觀察預估時間如何變化。

本實作使用 CPU 即可，不需要 API 金鑰。CSV 直接從 GitHub 讀取；繪圖設定會自動準備繁體中文字型。
重新啟動執行階段後，請從第一格依序執行。

## 這次會完成什麼？

看資料、畫圖、訓練模型、檢查誤差，再預測自己的新訂單。
訓練後取出 `y = ax + b` 的斜率與截距，將距離代入公式，並與 `model.predict()` 的結果比較。

## 檔案內容

- [外送還要多久才會到.ipynb](外送還要多久才會到.ipynb)：學生操作教材。
- [資料集/delivery_distance_time.csv](資料集/delivery_distance_time.csv)：課堂使用的距離與時間兩欄資料。
- [資料集/food_delivery_original.csv](資料集/food_delivery_original.csv)：原始模擬訂單。
- [資料集/food_delivery_clean.csv](資料集/food_delivery_clean.csv)：整理缺失值後的完整資料。
- [資料集/資料說明.md](資料集/資料說明.md)：來源、欄位與整理紀錄。
- [字型/](字型/README.md)：中文字型來源與授權。

本機操作時，以本資料夾作為工作目錄；目前 Notebook 會透過網路讀取 GitHub CSV。
資料是教學用的模擬訂單，不代表特定外送平台的實際資料。
