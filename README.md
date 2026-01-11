# 🎨 影像卡通化轉換器

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green.svg)
![Gradio](https://img.shields.io/badge/Gradio-Latest-orange.svg)

## 🚀 專題簡介
這是一個基於 **OpenCV** 與 **Gradio** 開發的工具。使用者可以透過直覺的滑桿調整，即時將影像轉換為具有藝術感的卡通風格，並支援本地下載。

### 核心技術點：
* **雙邊濾波 (Bilateral Filtering)**：實作保邊平滑演算法，產生卡通特有的「色塊感」。
* **自適應閾值 (Adaptive Thresholding)**：精確提取物體輪廓，模擬手繪線條筆觸。
* **極簡 UI 設計**：利用自定義 CSS 注入，隱藏冗餘元件，提供純淨的互動介面。
* **傳輸優化**：針對 Web 傳輸協議 (h11) 進行穩定化處理，確保高解析度影像處理不崩潰。

## 🛠 使用套件 (Dependencies)
在執行本程式碼前，請確保環境中已安裝以下套件：

```bash
pip install opencv-python numpy gradio
```

* **OpenCV (cv2)**：負責核心影像處理演算法。
* **NumPy**：高效處理影像矩陣數據。
* **Gradio**：建立基於 Web 的互動式 GUI 介面。

## 📖 使用說明
**啟動程式**：在 Jupyter Notebook 或 Python 環境中執行主程式碼。

**上傳影像**：點擊左側「原始影像」區塊，選擇電腦中的圖片上傳。

**調整風格：**
* **向左滑動 (Smooth)**：減少細節，增加色塊平滑度與模糊感。
* **向右滑動 (Detailed)**：增加細節，保留更多原圖特徵與細膩線條。
  
**預覽與下載：**
* 滑桿放開後，右側將自動生成卡通化影像。
* 點擊右側影像右上角的圖示即可開啟「全螢幕預覽」或「下載圖片」。
