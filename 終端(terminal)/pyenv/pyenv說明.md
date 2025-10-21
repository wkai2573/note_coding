# 安裝

建議用 scoop 安裝，參考[Scoop](../scoop(win包管理)/新機初始安裝.md)

[Github](https://github.com/pyenv-win/pyenv-win#installation)

# 指令

```shell
# 查看指令
pyenv

# 檢查pyenv安裝成功 & 版本
pyenv --version

# 列出可安裝的python版本
pyenv install -l

# 安裝 python
pyenv install <version>

# 設定要使用的 python 版本
# pyenv local <version>
pyenv global <version>

# 列出已安裝和使用中的 python 版本
pyenv versions

# 檢查python是否運作
python -c "import sys; print(sys.executable)"
```