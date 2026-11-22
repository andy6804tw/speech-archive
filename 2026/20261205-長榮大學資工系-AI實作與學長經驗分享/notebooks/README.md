# Notebooks

長榮大學資訊工程學系｜2026.12.05

兩份實作各自包含 Notebook、資料與操作說明。點選 Colab 徽章即可從 GitHub 開啟教材，資料由程式自動讀取。

| 實作 | Notebook | Colab | 執行環境 |
|---|---|---|---|
| 01 外送時間預測 | [外送還要多久才會到](外送時間預測/外送還要多久才會到.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andy6804tw/speech-archive/blob/main/2026/20261205-%E9%95%B7%E6%A6%AE%E5%A4%A7%E5%AD%B8%E8%B3%87%E5%B7%A5%E7%B3%BB-AI%E5%AF%A6%E4%BD%9C%E8%88%87%E5%AD%B8%E9%95%B7%E7%B6%93%E9%A9%97%E5%88%86%E4%BA%AB/notebooks/%E5%A4%96%E9%80%81%E6%99%82%E9%96%93%E9%A0%90%E6%B8%AC/%E5%A4%96%E9%80%81%E9%82%84%E8%A6%81%E5%A4%9A%E4%B9%85%E6%89%8D%E6%9C%83%E5%88%B0.ipynb) | CPU 即可 |
| 02 太陽能板瑕疵檢測 | [太陽能板瑕疵檢測與成因說明](太陽能板瑕疵檢測/太陽能板瑕疵檢測與成因說明.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andy6804tw/speech-archive/blob/main/2026/20261205-%E9%95%B7%E6%A6%AE%E5%A4%A7%E5%AD%B8%E8%B3%87%E5%B7%A5%E7%B3%BB-AI%E5%AF%A6%E4%BD%9C%E8%88%87%E5%AD%B8%E9%95%B7%E7%B6%93%E9%A9%97%E5%88%86%E4%BA%AB/notebooks/%E5%A4%AA%E9%99%BD%E8%83%BD%E6%9D%BF%E7%91%95%E7%96%B5%E6%AA%A2%E6%B8%AC/%E5%A4%AA%E9%99%BD%E8%83%BD%E6%9D%BF%E7%91%95%E7%96%B5%E6%AA%A2%E6%B8%AC%E8%88%87%E6%88%90%E5%9B%A0%E8%AA%AA%E6%98%8E.ipynb) | 建議 T4 GPU |

- [外送時間預測：操作說明與資料](外送時間預測/README.md)
- [太陽能板瑕疵檢測：操作說明與素材](太陽能板瑕疵檢測/README.md)

## 資料夾結構

```text
notebooks/
├── README.md
├── 外送時間預測/
│   ├── README.md
│   ├── 外送還要多久才會到.ipynb
│   ├── 資料集/
│   └── 字型/
└── 太陽能板瑕疵檢測/
    ├── README.md
    ├── 太陽能板瑕疵檢測與成因說明.ipynb
    └── 太陽能板實作素材.zip
```

## 維護方式

各實作的資料與說明放在自己的資料夾內，保留資料來源及原始授權。
若調整目錄或 Notebook 檔名，請同步更新這個入口、各教材的 Colab 徽章與資料網址。
太陽能板素材 ZIP 更新後，也要同步更新 Notebook 第一格的 `素材版本` SHA-256。
