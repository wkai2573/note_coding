# 安裝參考

[Github](https://github.com/coreybutler/nvm-windows)

建議用 scoop 安裝，參考[Scoop](../scoop(win包管理)/新機初始安裝.md)

# 指令
```shell
# 說明
nvm help

# nodejs版本清單
nvm list

# 切換nodejs版本
# 輸入開頭即可, 例如 nvm use 2
nvm use

# nodejs現在使用版本
nvm current
node -v

# 安裝最新穩定版
nvm install lts

# 安裝最新穩定版 & 裝上npm (建議)
# 安裝完記得 "nvm use 版本"
nvm install lts --latest-npm

# 安裝最新版(不建議)
nvm install latest

# 啟用pnpm (建議)
corepack enable
```