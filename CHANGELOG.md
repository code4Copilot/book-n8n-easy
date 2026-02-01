# 📦 n8n-easy Release Notes

## v2.4.6 (對應n8n的版本)
- 提供 **Windows 本機免安裝版 n8n**，已內建 Node.js 和 5 個 n8n 社群節點。
- 使用 **7-ZIP 自解壓縮檔**，解壓縮後自動建立目錄：
  ```
  C:\n8nEasy
  ```
- 內建啟動程式 `startfChartMenu.exe`，在工作列建立圖示，提供以下功能表命令：
  1. **啟動 n8n**：執行 `1_n8n_start-n8n.bat`，啟動服務並設定環境變數。
  2. **開啟 Web 介面**：啟動瀏覽器連線至 `http://localhost:5678`。

---

## v2.2.6 (對應n8n的版本)
- 提供 **Windows 本機免安裝版 n8n**，已內建 Node.js 和 3 個 n8n 社群節點。
- 使用 **7-ZIP 自解壓縮檔**，解壓縮後自動建立目錄：
  ```
  C:\n8nEasy
  ```
- 內建啟動程式 `startfChartMenu.exe`，在工作列建立圖示，提供以下功能表命令：
  1. **啟動 n8n**：執行 `1_n8n_start-n8n.bat`，啟動服務並設定環境變數。
  2. **開啟 Web 介面**：啟動瀏覽器連線至 `http://localhost:5678`。

---

## 📝 注意事項
- **easy** 表示安裝簡單，並非功能簡化版。  
- 僅支援 **Windows 10/11**。  
- 若需進階設定（如資料庫、外部服務整合），請參考官方 [n8n 文件](https://docs.n8n.io)。  

---

## 📖 授權
本專案包含以下開源軟體：
- [n8n](https://n8n.io) （Apache 2.0 License）  
- [Node.js](https://nodejs.org) （MIT License）  

請依相關授權條款使用與再散佈。
```

---

### 建議操作流程
1. **建立 Repository**：放 `README.md` 與 `start-n8n.bat`。  
2. **建立 Release**：上傳自解壓縮檔（例如 `n8n-easy-win.exe`）。  
3. **套用範本**：在 Release 說明中貼上上述範本，並更新版本號與更新內容。  

