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

docker pull goharbor/registry-photon:dev && \
docker tag goharbor/registry-photon:dev  registry-vpc.cn-qingdao.aliyuncs.com/wod/registry-photon:dev  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/registry-photon:dev 

docker pull goharbor/chartmuseum-photon:dev && \
docker tag goharbor/chartmuseum-photon:dev  registry-vpc.cn-qingdao.aliyuncs.com/wod/chartmuseum-photon:dev  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/chartmuseum-photon:dev 

docker pull goharbor/clair-photon:dev && \
docker tag goharbor/clair-photon:dev  registry-vpc.cn-qingdao.aliyuncs.com/wod/clair-photon:dev  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/clair-photon:dev 

docker pull goharbor/notary-server-photon:dev && \
docker tag goharbor/notary-server-photon:dev  registry-vpc.cn-qingdao.aliyuncs.com/wod/notary-server-photon:dev  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/notary-server-photon:dev 

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
