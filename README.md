### dockefiles
some usefull dockerfile

-  Mongo.Dockerfile

    阿里云部署时, 将/data/db外挂到NAS时,报权限错误(linux不允许修改mount存储的chown),去掉官方dockerfile的中`chown`命令
    >chown -R mongodb:mongodb /data/db /data/configdb
- java_node.Dockerfile

    包含Java和node的基础镜像, 用于build一些既有java+node的应用.
    - openjdk8
    - node 8.11.3
    - yarn 1.9.2
    - gradle 4.6
