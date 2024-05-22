# docker compose

多容器管理

## Link

* [Dockerfile reference⁠](https://docs.docker.com/engine/reference/builder/)
* [Compose file reference](https://docs.docker.com/compose/compose-file/)

## shell

```shell

# 使用引導建立 dockerfile & compose.yaml
docker init

# 根據compose.yaml
# 建立並啟動容器s, -d:終端分離,不占用目前終端操作,不加則可以看到docker-compose的log資訊
docker compose up -d

# 建立並啟動容器s, -w:並啟用自動偵測更新
docker compose up -d -w

# 刷新容器(手動更新)
docker compose up -d --build

# 關閉並移除容器 (若未使用終端分離-d, 使用Ctrl+C可達同樣效果)
docker compose down

```

## docs