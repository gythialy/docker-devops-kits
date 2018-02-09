## 介绍

包含 gitea+kanboard+jenkins，通过 nginx 反向代理实现域名访问。域名只需修改环境变量 `VIRTUAL_HOST`。mysql root 密码保存在 `mysql/my_secret.txt`。

```yml
environment:
    - VIRTUAL_HOST=task.vking.io
    - VIRTUAL_PORT=80
```

## 准备
- docker
- docker-compose (1.9+)

## 使用

- 创建镜像并执行 `docker-compose up -d `
- 删除容器 `docker-compose down -v`


## TODO
- [ ] 增加 dnsmasq 配置
- [ ] nginx 增加 https 支持

