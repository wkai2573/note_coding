# Dockerfile

使用dockerfile 建立 image

## Link

* [Dockerfile reference⁠](https://docs.docker.com/engine/reference/builder/)
* [Compose file reference](https://docs.docker.com/compose/compose-file/)

## docs

```Dockerfile

# 定義變數
ARG NODE_VERSION=19.5.0

# 設定環境變數
ENV NODE_ENV=production

# 從指定image開始建置階段
FROM node:${NODE_VERSION}-alpine

# 更改docker接下來執行的工作目錄
WORKDIR /path/to/workdir

# 執行指令 (建置image時執行)
RUN npm install -g nodemon
# 將檔案掛在到image上 (https://docs.docker.com/reference/dockerfile/#run---mount)
RUN --mount=type=bind,source=package.json,target=package.json


# 將本地目錄複製到image目前工作目錄
COPY . .

# 公開port
EXPOSE 3000

# 執行指令 (建立容器時, 預設執行的命令, 僅能一個CMD)
CMD npm run dev



```