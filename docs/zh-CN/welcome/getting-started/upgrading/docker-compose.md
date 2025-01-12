# Docker 安装的升级

## 0. 升级前的准备

:::warning
升级前一定要先备份数据库！！！
:::

## 1. 切换到 `docker-compose.yml` 所在的目录

例如

```bash
# MacOS, Linux...
cd /your/path/my-project/
# Windows
cd C:\your\path\my-project
```

## 2. 更新 image 版本号

- `latest` 截止目前最稳定的版本，推荐安装此版本；
- `next` 内测版，包含一些未发布的新特性，这个版本可能还不完全稳定，适用于开发者或测试人员，用于提前体验新功能或进行兼容性测试；
- `1.2.4-alpha` 指定版本号升级，最新版本情况，查看[已发布版本列表](https://hub.docker.com/r/nocobase/nocobase/tags)

:::warning
镜像只能升级不能降级，不能将 next 降级为 latest
:::

```yml
# ...
services:
  app:
    # 阿里云 main 版本（只支持 AMD64 架构）
    image: registry.cn-shanghai.aliyuncs.com/nocobase/nocobase:main
    # 阿里云 latest 版本
    image: registry.cn-shanghai.aliyuncs.com/nocobase/nocobase:latest
    # 阿里云指定版本
    image: registry.cn-shanghai.aliyuncs.com/nocobase/nocobase:1.2.4-alpha
    # Docker Hub 镜像，可能会下载不了
    image: nocobase/nocobase:main
    image: nocobase/nocobase:latest
    image: nocobase/nocobase:1.2.4-alpha
# ...
```

## 3. 重启容器

```bash
# 拉取最新镜像
docker-compose pull
# 启动
docker-compose up -d app
# 查看 app 进程的情况
docker-compose logs app
```

## 4. 独立插件的升级

NocoBase 升级之后，通过界面安装的独立插件可能也需要升级，参考文档 [独立插件的安装与升级](/welcome/getting-started/plugin)
