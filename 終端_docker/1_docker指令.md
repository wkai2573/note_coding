# docker image

```shell
docker image ls

# 複製並重命名新image, 可用於複製別人的image
docker tag imageName newImageName

# 使用dockerfile 建立 image, -t:命名為myImage, 使用.(=目前目錄)下的dockerfile
docker build -t myImage .

```

# docker container

```shell
docker container ls

# 使用image運行容器
# --rm: 結束後刪除容器
# -it: 這兩個選項是分別指定的，-i 讓容器的 STDIN 保持打開，-t 分配一個虛擬終端（TTY）。這兩個選項一起使用，可以讓你與容器的命令行進行交互操作，就像在本地的終端中一樣。
# -v: 指定Volume映射
docker run --rm -it -v $(pwd)/AndroidTacticalAssaultKit-CIV:/AndroidTacticalAssaultKit-CIV atak-build-env

# 重新命名
docker rename oldContainerName newContainerName

# 進入容器命令列
docker exec containerID /bin/bash

```