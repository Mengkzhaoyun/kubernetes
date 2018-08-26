# images
```bash
docker pull goharbor/harbor-ui:dev && \
docker tag goharbor/harbor-ui:dev  registry-vpc.cn-qingdao.aliyuncs.com/wod/harbor-ui:dev  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/harbor-ui:dev 

docker pull goharbor/harbor-adminserver:dev && \
docker tag goharbor/harbor-adminserver:dev  registry-vpc.cn-qingdao.aliyuncs.com/wod/harbor-adminserver:dev  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/harbor-adminserver:dev 

docker pull goharbor/harbor-jobservice:dev && \
docker tag goharbor/harbor-jobservice:dev  registry-vpc.cn-qingdao.aliyuncs.com/wod/harbor-jobservice:dev  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/harbor-jobservice:dev 

docker pull goharbor/harbor-db:dev && \
docker tag goharbor/harbor-db:dev  registry-vpc.cn-qingdao.aliyuncs.com/wod/harbor-db:dev  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/harbor-db:dev 

docker pull registry:2.6.2 && \
docker tag registry:2.6.2  registry-vpc.cn-qingdao.aliyuncs.com/wod/registry:2.6.2  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/registry:2.6.2 

docker pull nginx:1.15.2-alpine && \
docker tag nginx:1.15.2-alpine  registry-vpc.cn-qingdao.aliyuncs.com/wod/nginx:1.15.2-alpine  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/nginx:1.15.2-alpine 
```

# setup
```powershell
# 1.template
cd C:\Go\src\github.com\mengkzhaoyun\kubernetes\aliyun\devops\harbor ;`
helm template . --name harbor --namespace devops > ./dist/harbor.yaml
```
