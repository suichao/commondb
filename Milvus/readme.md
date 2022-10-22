安装教程：

[用户指南快速入门安装 Milvus - 安装 CPU 版 Milvus - 《Milvus 0.8 开源向量搜索引擎使用教程》 - 书栈网 · BookStack](https://www.bookstack.cn/read/milvus-0.8/guides-get_started-install_milvus-cpu_milvus_docker.md)



docker run -d --name milvus_cpu -p 19530:19530 -p 19121:19121 -p 9091:9091 -v /home/denis/milvus_sample/db:/var/lib/milvus/db -v /home/denis/milvus_sample/conf:/var/lib/milvus/conf -v /home/denis/milvus_sample/logs:/var/lib/milvus/logs -v /home/denis/milvus_sample/wal:/var/lib/milvus/wal milvusdb/milvus:0.8.0-cpu-d041520-464400



可视化

```text
docker run -d -p 8000:3000 -e HOST_URL=http://127.0.0.1:8000 -e MILVUS_URL=127.0.0.1:19530 milvusdb/milvus-insight:latest
```

