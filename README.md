# cloudreve-docker

## 说明

1. 本项目使用 MySQL 替换 Cloudreve 内置的数据库；
2. 轻量使用环境下，本不需要使用 MySQL 作为数据库，但 PostgreSQL [无法正常读取配置](https://github.com/cloudreve/Cloudreve/issues/960)。

### 测试环境

本 docker-compose 在以下服务器上测试通过：

1. 腾讯云轻量应用服务器（Ubuntu 20.04），Hong Kong，1C1G，30Mbps

## 资源占用

### 待机状态

```
NAME                           CPU %     MEM USAGE / LIMIT     MEM %     NET I/O          BLOCK I/O

cloudreve-docker_cloudreve_1   0.00%     35.24MiB / 980.8MiB   3.59%     15MB / 22.3MB    38.7MB / 0B

cloudreve-docker_redis_1       0.12%     3.258MiB / 980.8MiB   0.33%     2MB / 2.61MB     9.63MB / 381kB

cloudreve-docker_mysql_1       0.04%     462.7MiB / 980.8MiB   47.17%    2.66MB / 8.1MB   50.6MB / 33.5MB
```

## 参考

本 docker-compose 参考下方仓库的相关代码，在此向作者表示感谢！
1. [xavier-niu/cloudreve-docker](https://github.com/xavier-niu/cloudreve-docker)
2. [helingfeng/Docker-LNMP](https://github.com/helingfeng/Docker-LNMP)