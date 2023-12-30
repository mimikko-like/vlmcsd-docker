# VLMCSD for Docker
fork 来自 wind4原库

Deploy vlmcsd service on Docker container

```bash
git clone https://github.com/Wind4/vlmcsd-docker.git vlmcsd
cd vlmcsd

# Use docker-compose service
docker-compose up -d

# or docker build image
docker build -t vlmcsd .
docker run -idt -p 1688:1688 vlmcsd
```


激活代码
新建文本文档，后缀该为bat，代码内容：

```bash
slmgr /skms ip:1688
slmgr /ato
slmgr.vbs -dlv
```
