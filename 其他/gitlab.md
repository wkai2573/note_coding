## 【clone 使用帳號&令牌】

令牌生成: https://gitlab.com/-/user_settings/personal_access_tokens
目前令牌: [令牌]

clone方法，範例：

```shell
git clone https://帳號:令牌@git遠端位置(HTTPS) 本地存放位置

git clone https://kai.wei:[令牌]@gitlab.com/kaiwave/exmple-kai.git c:\Users\kai\Desktop\exmple-kai
git clone https://wkai2573:[令牌]@gitlab.com/wavein-iot/aiot/web/sdas.git c:\Users\admin\Desktop\sdas

```

一台電腦輸入過該帳號+token後，應該就不用再輸入了，可以直接用vscode的clone



## remote

```shell
# 添加remote 並fetch
git remote add gitlab https://wkai2573:[令牌]@gitlab.com/wavein-iot/aiot/web/sdas.git -f

```
