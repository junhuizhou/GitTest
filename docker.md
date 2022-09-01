<!--
 * @Author: ZhouJunhui
 * @Date: 2022-09-01 15:26:57
 * @LastEditor: ZhouJunhui
 * @LastEditTime: 2022-09-01 15:32:19
 * @FilePath: \GitTest\docker.md
 * @Description: file content
-->

docker pull debian

docker images

docker run --name test -itd debian sleep infinity

docker ps

docker exec -it test /bin/bash

docker cp SRC DEST

docker stop test && docker rm test

cat > sources.list << EOF


```sh

# 默认注释了源码镜像以提高 apt update 速度，如有需要可自行取消注释
deb http://mirrors.bit.edu.cn/debian/ bullseye main contrib non-free
# deb-src http://mirrors.bit.edu.cn/debian/ bullseye main contrib non-free
deb http://mirrors.bit.edu.cn/debian/ bullseye-updates main contrib non-free
# deb-src http://mirrors.bit.edu.cn/debian/ bullseye-updates main contrib non-free

deb http://mirrors.bit.edu.cn/debian/ bullseye-backports main contrib non-free
# deb-src http://mirrors.bit.edu.cn/debian/ bullseye-backports main contrib non-free

deb http://mirrors.bit.edu.cn/debian-security bullseye-security main contrib non-free
# deb-src http://mirrors.bit.edu.cn/debian-security bullseye-security main contrib non-free

```
