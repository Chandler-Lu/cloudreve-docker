# cloudreve-docker

## 说明

1. 本项目使用 PostgreSQL 替换 Cloudreve 内置的数据库。

## 测试环境

本 docker-compose 在 Ubuntu 24.04, 4C4G 下测试通过。

## 资源占用

### 待机状态

```
NAME                                  CPU %     MEM USAGE / LIMIT     MEM %     NET I/O           BLOCK I/O
cloudreve                             0.00%     40.04MiB / 3.824GiB   1.02%     51.2MB / 30.9MB   2.12MB / 8.89MB
cloudreve-cache-1                     0.63%     3.707MiB / 3.824GiB   0.09%     5.77MB / 34MB     618kB / 147kB
cloudreve-database-1                  0.00%     25.52MiB / 3.824GiB   0.65%     424kB / 7.65MB    1.81MB / 2.56MB
```
