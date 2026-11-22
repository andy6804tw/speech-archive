# 太陽能板瑕疵檢測與成因說明

讓 AI 看圖找瑕疵｜長榮大學資訊工程學系｜2026.12.05

用主辦方已訓練的 PRB-FPN 與已微調 Qwen，完成瑕疵偵測、整理文字線索與說明可能成因。
case01 跟著操作，case02～case10 從中選一組自行練習。

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andy6804tw/speech-archive/blob/main/2026/20261205-%E9%95%B7%E6%A6%AE%E5%A4%A7%E5%AD%B8%E8%B3%87%E5%B7%A5%E7%B3%BB-AI%E5%AF%A6%E4%BD%9C%E8%88%87%E5%AD%B8%E9%95%B7%E7%B6%93%E9%A9%97%E5%88%86%E4%BA%AB/notebooks/%E5%A4%AA%E9%99%BD%E8%83%BD%E6%9D%BF%E7%91%95%E7%96%B5%E6%AA%A2%E6%B8%AC/%E5%A4%AA%E9%99%BD%E8%83%BD%E6%9D%BF%E7%91%95%E7%96%B5%E6%AA%A2%E6%B8%AC%E8%88%87%E6%88%90%E5%9B%A0%E8%AA%AA%E6%98%8E.ipynb)

## 在 Google Colab 開始

1. 點選上方徽章，直接在 Colab 開啟教材。
2. 在「執行階段 → 變更執行階段類型」選擇 T4 或可用的 GPU。
3. 從第一格依序執行，程式會自動從 GitHub 下載並驗證素材，再準備套件與官方模型。
4. 跟著操作 case01，再從選單換一組案例練習。

第一次安裝與下載需要幾分鐘。模型解壓後約 **1.13 GB**，無需 API 金鑰。
套件在獨立環境執行，不需為了套件版本重新啟動 Notebook；沒有 GPU 也能使用 CPU，但速度較慢。

## 你會完成的步驟

觀察 EO／IR 原圖、執行 PRB-FPN、查看交給 Qwen 的文字、產生可能成因、換案例、對照人工標註，最後下載練習結果 JSON。

這份 baseline 的 Qwen 讀取的是文字線索，沒有直接看圖片。
成因說明是模型提出的推測，需要對照影像與標註檢查。
10 組案例來自競賽訓練集，適合練習操作，不能用來估算未見資料的準確率。
下載的 JSON 只包含所選案例，不是完整競賽提交檔。

## 檔案與來源

- [太陽能板瑕疵檢測與成因說明.ipynb](太陽能板瑕疵檢測與成因說明.ipynb)：學生操作教材。
- [太陽能板實作素材.zip](太陽能板實作素材.zip)：10 組案例、標註摘錄、官方程式與課堂輔助程式。
- 素材 SHA-256：`861608a4622565e174f3a319a8c587ca503d2b224da383b36ef90468b43cc0be`。

模型權重由程式另外從主辦方下載，不放入 GitHub 素材包。
素材 ZIP 內的 `來源與使用說明.md` 記錄資料來源，並保留原始授權。

本機操作使用 Python 3.12 或 3.13，以本資料夾為工作目錄。執行時建立的 `solar_classroom/` 存放環境、模型與練習輸出。

競賽資料：[AIdea 競賽頁面](https://www.aidea-web.tw/topic/3c8ec48b-0dff-4b14-9b5e-d91bbb98c699?lang=zh)・[主辦方資料](https://drive.google.com/drive/folders/1PO9jYBlQXbkAgbp-xTySJWQdnBXF2wGz)。
