
# 安裝

```shell

# 安裝scoop (請在powerShell中執行)
# 官網: https://scoop.sh/
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression

# 安裝git
scoop install git

# bucket 加入 extras來源 (許多包放在extras 要先加入才能安裝各種包)
scoop bucket add extras
scoop bucket list #查看bucket

# 安裝nvm (NodeJs版本管理)
# scoop search nvm
scoop install nvm
nvm install lts   # 安裝最新穩定版NodeJs
nvm list          # 查看已安裝版本
nvm use <version> # 使用版本
corepack enable   # 啟用pnpm

# 安裝pyenv (Python版本管理)
# scoop search pyenv
scoop install pyenv
pyenv install -l        # 查看可安裝版本
pyenv install <version> # 安裝Python
pyenv global <version>  # 使用版本(全域)

# 如果安裝失敗, 參考: https://github.com/pyenv-win/pyenv-win/issues/449#issuecomment-2143194236
# scoop uninstall pyenv
# scoop install pyenv (需系統管理員)
# pyenv update
# pyenv install <version>
```

# Windows新機安裝Apps

[Windows新機安裝Apps](./windows-setup-apps.md)


# Scoop目錄

```shell
%USERPROFILE%\scoop       # Scoop根目錄
%USERPROFILE%\scoop\shims # 各App的shims (命令列開啟App)
```


# 其他指令

```shell
# 更新相關
scoop status # 查看可更新的Apps
scoop update # 更新全部安裝的Apps

# APP相關
scoop list         # 列出已安裝的pps
scoop prefix <app> # 查看安裝的App目錄
scoop shim <subcommand> [<shim_name>...] [options] [other_args] # 建立命令快捷(有些App會自動建立)

# 查詢有無可用的套件
scoop search <AppName>

# 切換使用的版本
scoop reset [package] [version]


# 搬移新電腦方式
# 舊電腦
scoop export > scoopfile.json
# 新電腦
iwr -useb get.scoop.sh | iex
scoop import scoopfile.json
```
