# images
```bash
docker pull sameersbn/gitlab:11.1.4 && \
docker tag sameersbn/gitlab:11.1.4  registry-vpc.cn-qingdao.aliyuncs.com/wod/sameersbn-gitlab:11.1.4  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/sameersbn-gitlab:11.1.4 

docker pull sameersbn/postgresql:10 && \
docker tag sameersbn/postgresql:10 registry-vpc.cn-qingdao.aliyuncs.com/wod/sameersbn-postgresql:10 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/sameersbn-postgresql:10

docker pull sameersbn/redis:4.0.9-1 && \
docker tag sameersbn/redis:4.0.9-1 registry-vpc.cn-qingdao.aliyuncs.com/wod/sameersbn-redis:4.0.9-1 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/sameersbn-redis:4.0.9-1
```

# setup
```bash
# 1. enable storageapi
ClusterIP=$(kubectl get svc/storageos --namespace storageos -o custom-columns=IP:spec.clusterIP --no-headers=true) && \
ApiAddress=$(echo -n "tcp://$ClusterIP:5705" | base64) && \
kubectl patch secret/storageos-api --namespace devops --patch "{\"data\":{\"apiAddress\": \"$ApiAddress\"}}"

# 2. Install Gitlab
cd /etc/kubernetes/helm/gitlab && \
helm install . --name gitlab --namespace devops

# 3. Uninstall Gitlab
helm del --purge gitlab
```