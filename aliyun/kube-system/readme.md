# images
```bash
# containous/traefik:1.6.5
docker pull traefik:1.6.5-alpine && \
docker tag traefik:1.6.5-alpine hub.c.163.com/mengkzhaoyun/public:traefik-1.6.5-alpine && \
docker push hub.c.163.com/mengkzhaoyun/public:traefik-1.6.5-alpine

docker pull traefik:v1.7.0-rc3-alpine && \
docker tag traefik:v1.7.0-rc3-alpine registry-vpc.cn-qingdao.aliyuncs.com/wod/traefik:v1.7.0-rc3-alpine && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/traefik:v1.7.0-rc3-alpine
```
