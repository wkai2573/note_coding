# docker compose
多容器管理

```shell

# 根據compose.yaml
# 建立並啟動容器s, -d:終端分離,不占用目前終端操作,不加則可以看到docker-compose的log資訊
docker compose up -d

# 建立並啟動容器s, -w:並啟用自動偵測更新
docker compose up -d -w

# 刷新容器(手動更新)
docker compose up -d --build

```