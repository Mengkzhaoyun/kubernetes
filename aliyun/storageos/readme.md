# images
```bash
docker pull storageos/node:1.0.0-rc2 && \
docker tag storageos/node:1.0.0-rc2 registry-vpc.cn-qingdao.aliyuncs.com/wod/storageos-node:1.0.0-rc2 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/storageos-node:1.0.0-rc2

docker pull storageos/init:0.1 && \
docker tag storageos/init:0.1 registry-vpc.cn-qingdao.aliyuncs.com/wod/storageos-init:0.1 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/storageos-init:0.1

docker pull quay.io/k8scsi/driver-registrar:v0.2.0 && \
docker tag quay.io/k8scsi/driver-registrar:v0.2.0 registry-vpc.cn-qingdao.aliyuncs.com/wod/k8scsi-driver-registrar:v0.2.0 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/k8scsi-driver-registrar:v0.2.0

docker pull quay.io/k8scsi/csi-provisioner:canary && \
docker tag quay.io/k8scsi/csi-provisioner:canary registry-vpc.cn-qingdao.aliyuncs.com/wod/k8scsi-csi-provisioner:canary && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/k8scsi-csi-provisioner:canary

docker pull quay.io/k8scsi/csi-attacher:canary && \
docker tag quay.io/k8scsi/driver-registrar:v0.2.0 registry-vpc.cn-qingdao.aliyuncs.com/wod/k8scsi-csi-attacher:canary && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/k8scsi-csi-attacher:canary

ClusterIP=$(kubectl get svc/storageos --namespace storageos -o custom-columns=IP:spec.clusterIP --no-headers=true) && \
ApiAddress=$(echo -n "tcp://$ClusterIP:5705" | base64) && \
kubectl patch secret/storageos-api --namespace default --patch "{\"data\":{\"apiAddress\": \"$ApiAddress\"}}"

helm install . --name storageos --namespace storageos
```