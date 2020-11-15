# 一些Linux软件的安装




<!--more-->

## 0. 注意

- 以下只用于`Ubuntu`系统

## 1. docker

```bash
# 安装官方docker
curl -fsSL get.docker.com -o get-docker.sh
# 使用镜像源
sudo sh get-docker.sh --mirror Aliyun
sudo sh get-docker.sh --mirror AzureChinaCloud
```

> 参考网址：[https://yeasy.gitbook.io/docker_practice/install/ubuntu](https://yeasy.gitbook.io/docker_practice/install/ubuntu)

##  2.nodejs

- 安装最新长期服务版

```bash
# root 用户执行
curl -sL https://deb.nodesource.com/setup_lts.x | bash -
apt-get install -y nodejs
```

> 参考网址：[https://github.com/nodesource/distributions#installation-instructions](https://github.com/nodesource/distributions#installation-instructions)
