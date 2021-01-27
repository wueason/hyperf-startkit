[English](./README.md) | 中文

# 介绍

提供基于`Docker`镜像的[`Hyperf`](https://github.com/hyperf/hyperf)服务的快速开发环境。

# 依赖

 - `docker`环境
 - `docker-compose`命令

# 使用

- 生成镜像 `docker-compose build`
- 安装`composer.json`依赖 `docker-compose run --rm hyperf-web "composer install --no-dev"`
- 启动服务 `docker-compose up -d`
- 访问地址：`Windows`中为`Docker`虚拟机IP（一般为`http://192.168.99.100:9501`），`Linux`/`Mac`中为宿主机IP（`http://127.0.0.1:9501`）

# 注意点

- 在`Windows`系统中使用时，需要将代码放在`C:\Users\{USERANME}`中，否则会挂载到`Docker`会失效
- 当`Dockerfile`有变动时，需要重新编译`Docker`镜像，执行`docker-compose build`