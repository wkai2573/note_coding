# 🧰 Windows 新機安裝應用整理

1. [參考1](https://www.cnblogs.com/fires/p/18727717)
2. [參考2](https://github.com/killsen/scoop-dev?tab=readme-ov-file)

---

## ⚙️ 命令列工具（必裝）

| 工具 | 來源 | 說明 |
|------|------|------|
| git | `scoop install main/git` | 版本控制工具 |
| nvm | `scoop install main/nvm` | Node.js 版本管理(未來專案改用bun) |
| pyenv | `scoop install main/pyenv` | Python 版本管理 |
| scoop-search | `scoop install main/scoop-search` | 搜尋 Scoop bucket 套件 |

---

## 🧑‍💻 命令列工具（推薦）

| 工具 | 來源 | 說明 |
|------|------|------|
| sudo | `scoop install main/sudo` | 以系統管理員權限執行命令（Windows 版 sudo）|
| go | `scoop install main/go` | Go 語言開發環境 |
| gcc | `scoop install main/gcc` | GNU 編譯器套裝 |
| ffmpeg | `scoop install main/ffmpeg` | 影音轉檔與處理工具 |
| imagemagick | `scoop install main/imagemagick` | 圖像處理工具 |
| fvm | `scoop install extras/fvm` | Flutter SDK 版本管理 |

---

## 🪟 圖形介面應用（推薦）

| 工具 | 來源 | 說明 |
|------|------|------|
| UniGetUI | `scoop install extras/unigetui` | 各包管理器的 GUI 介面（需 `main/scoop-search`）<br>支援 Scoop、WinGet、Chocolatey、MS Store、本機應用 |
| Windows Terminal | `scoop install extras/windows-terminal` | 現代終端機（建議同時安裝 `extras/vcredist2022`） |
| PowerToys | `scoop install extras/powertoys` | 微軟官方強化工具集（安裝後會提示右鍵整合指令） |
| Everything | `scoop install extras/everything` | 全域檔案搜尋工具（安裝後在 `%USERPROFILE%\scoop\apps\everything\current` 執行`.reg`檔：加入右鍵 |
| Snipaste | `scoop install extras/snipaste` | 螢幕截圖與貼圖工具 |
| Bandizip | `scoop install extras/bandizip` | 壓縮解壓縮工具（7.0 以上版本含廣告） |
| PotPlayer | `scoop install extras/potplayer` | 高效能影音播放軟體 |
| Discord | `scoop install extras/discord` | 聲音與文字通訊軟體 |
| Locale Emulator | `scoop install extras/locale-emulator` | 模擬不同地區語言環境（安裝後執行 *Locale Emulator Installer* 完成） |
| qBittorrent | `scoop install extras/qbittorrent` | BitTorrent 用戶端 |
| CrystalDiskInfo | `scoop install extras/crystaldiskinfo` | 硬碟健康監測工具 |
| PhotoDemon | `scoop install extras/photodemon` | 開源影像編輯工具 |
| draw.io | `scoop install extras/draw.io` | 圖表與流程圖繪製工具 |
| FileZilla | `scoop install extras/filezilla` | FTP/SFTP 客戶端 |
| Cheat Engine | `scoop install extras/cheat-engine` | 單機遊戲修改器 |

---

## 💡 其他常用 GUI 應用（推薦）

| 應用 | 來源 | 說明 |
|------|------|------|
| VSCode | WinGet | 開發編輯器，官網下載正常安裝，開始列右鍵才會列出最近開啟檔案 |
| Google Chrome (EXE) | WinGet 或 `scoop install extras/googlechrome` | 瀏覽器 |
| PowerShell | WinGet | 命令列介面與自動化工具(這個是跨平臺的，與 Windows PowerShell 不同) |
| Windhawk | WinGet | Windows 功能模組平台（自訂系統行為） |
| Tiefsee | Microsoft Store | 圖像瀏覽器（快速、乾淨） |
| Steam | WinGet | 遊戲平台 |
| JDownloader 2 | WinGet | 下載管理器 |
| LINE | 電腦本機 | 通訊軟體（建議直接安裝本機版） |
| WinRAR | 電腦本機 | 經典壓縮軟體（綁定右鍵需在 App 設定中啟用）|

---

## 🧩 其他工具（可選）

| 工具 | 來源 | 說明 |
|------|------|------|
| Navicat Premium Lite 17 | WinGet | 資料庫管理工具 |
| PostgreSQL | `scoop install main/postgresql` | 資料庫系統 |
| OBS Studio | `scoop install extras/obs-studio` | 串流錄影軟體 |
| PuTTY | `scoop install extras/putty` | SSH/Telnet 工具 |
| x64dbg | `scoop install extras/x64dbg` | Windows 除錯工具 |

---

## ✅ 安裝提示
- Scoop GUI 介面（如 unigetui）建議優先安裝。
- 某些 App 安裝後會提示可選的「右鍵整合」命令，建議執行。
- 若遇到缺少執行環境，可安裝：
  ```bash
  scoop install extras/vcredist2022
  ```
