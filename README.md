# Redis
## 1、创建网络
``` SHELL
docker network create hoppscotch
```


## 2、启动
启动容器
``` SHELL
docker-compose up -d
```

执行数据迁移
``` SHELL
docker compose run --entrypoint sh hoppscotch-aio
pnpx prisma migrate deploy
```

## 3、测试
http://localhost:3000# docker-compose-hoppscotch
