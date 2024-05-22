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

# 重新命名
docker rename oldContainerName newContainerName

# 進入容器命令列
docker exec containerID /bin/bash

```