# images
```bash
docker pull registry.ispacesys.cn/cig/drone-server:1.0.3-alpha && \
docker tag registry.ispacesys.cn/cig/drone-server:1.0.3-alpha registry-vpc.cn-qingdao.aliyuncs.com/wod/drone-server:0.8.4-3 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/drone-server:0.8.4-3

docker pull registry.ispacesys.cn/cig/drone-agent:1.0.3-alpha && \
docker tag registry.ispacesys.cn/cig/drone-agent:1.0.3-alpha registry-vpc.cn-qingdao.aliyuncs.com/wod/drone-agent:0.8.4-3 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/drone-agent:0.8.4-3
```

# setup
```bash
# 1. Install
cd /etc/kubernetes/helm/drone && \
helm install . --name drone --namespace devops

# 2. Uninstall
helm del --purge drone

# 3. template
cd /etc/kubernetes/helm/drone && mkdir -p /etc/kubernetes/helm/drone/dist && \
helm template . --name drone --namespace devops > ./dist/drone.yml
```