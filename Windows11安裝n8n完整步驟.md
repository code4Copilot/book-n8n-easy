**Windows 11 安裝 n8n 完整步驟**

**前置準備**

**1\. 確認 Node.js 和 npm 已安裝**

node --version

npm --version

- n8n 需要 Node.js 18.10 或更高版本
- 如未安裝，請從 [nodejs.org](https://nodejs.org/) 下載安裝

**安裝步驟**

**2\. 清除 npm 快取**

npm cache clean --force

**3\. 驗證快取已清除**

npm cache verify

**4\. 建立並進入指定資料夾**

\# 例如在 D:\\n8n 資料夾

mkdir D:\\n8n

cd D:\\n8n

**5\. 初始化專案（可選，如果要在此資料夾管理）**

npm init -y

**6\. 安裝最新版 n8n**

npm install n8n@latest

或者全域安裝（推薦）：

npm install -g n8n@latest

**7\. 驗證安裝**

\# 如果是全域安裝

n8n --version

\# 如果是本地安裝

npx n8n --version

**8\. 啟動 n8n**

\# 全域安裝方式

n8n start

\# 本地安裝方式

npx n8n start

**進階設定**

**設定環境變數（可選）** 在 PowerShell 中設定 n8n 資料儲存位置：

\$env:N8N_USER_FOLDER="D:\\n8n\\data"

**設定自訂連接埠（預設 5678）**

\$env:N8N_PORT="5678"

**疑難排解**

如果安裝過程遇到問題：

- **檢查 npm 設定**

npm config list

- **重設 npm 設定**

npm config delete prefix

- **以管理員權限執行 PowerShell**（右鍵點選 PowerShell → 以系統管理員身分執行）
- **更新 npm 到最新版**

npm install -g npm@latest

**存取 n8n**

安裝並啟動成功後，在瀏覽器開啟：

<http://localhost:5678>

**診斷與解決方案**

**請先按 Ctrl + C 中斷目前的安裝程序**，然後依照以下步驟重新安裝：

**1\. 清除 npm 快取並重試**

\# 中斷目前程序（如果還在執行）

Ctrl + C

\# 清除 npm 快取

npm cache clean --force

\# 驗證快取

npm cache verify

\# 檢查 npm 連線速度（切換到淘寶鏡像，速度較快）

npm config set registry <https://registry.npmmirror.com>

\# 重新安裝

npm install n8n

**2\. 如果還是很慢，使用詳細模式查看進度**

npm install n8n --verbose

這樣可以看到安裝過程的詳細資訊，知道卡在哪裡。

**3\. 或者嘗試全域安裝（通常更快）**

npm install -g n8n

**4\. 檢查網路連線**

n8n 是一個較大的套件，安裝時間取決於：

- 網路速度
- npm 伺服器回應速度
- 相依套件數量（n8n 有很多相依套件）

正常安裝時間大約 **3-10 分鐘**，如果超過 10 分鐘沒反應，建議中斷重試。