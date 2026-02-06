# n8n-easy

這是一個在 **Windows 平台** 使用 **npm 安裝的本機 n8n 套件**，已內建 **Node.js**，並打包成 **7-ZIP 自解壓縮檔**。  
使用者只需解壓縮至預設目錄 `n8nEasy`，即可快速建立並啟動 n8n。

---

## 📦 套件特色
- **免安裝**：包含 Node.js,  n8n 與 n8n 社群節點，解壓縮即可使用。  
- **啟動程式**：內建 `startfChartMenu.exe`，在工作列建立圖示，點選即可呼叫功能表。  
- **教學友善**：適合課堂分發、快速測試與本機開發。  

---

## 🆕 2.7.2 版更新
- 升級內建 n8n 至 2.7.2 版本。
- 新增社群節點：n8n-nodes-filemanager，支援檔案管理功能。

1. 執行自解壓縮檔，預設會展開至：
   ```
   C:\n8nEasy
   ```

2. 在 `n8nEasy` 目錄中，找到 **啟動程式 `startfChartmenu.exe`**。  
   執行後會在 **工作列建立圖示**，點選圖示即可開啟功能表，提供以下兩個命令：

   - **啟動 n8n**  
     執行 `1_n8n_server.bat` 檔案以啟動本機 n8n 服務。  
     使用 `.bat` 的目的在於方便設定環境變數。  
     
   - **開啟 Web 介面**  
     使用 `2_n8n_editor.url` 檔案啟動瀏覽器並連線至：
     ```
     http://localhost:5678
     ```

---

## 📝 注意事項
- 本套件僅支援 **Windows 10/11**。  
- 若需進行進階設定（如資料庫、外部服務整合），請參考官方 [n8n 文件](https://docs.n8n.io)。  

## 📖 授權
本專案包含以下開源軟體：
- [n8n](https://n8n.io) （Apache 2.0 License）  
- [Node.js](https://nodejs.org) （MIT License）  

請依相關授權條款使用與再散佈。