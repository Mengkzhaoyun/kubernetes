# images
```bash
docker login --username=mengkzhaoyun@gmail.com registry-vpc.cn-qingdao.aliyuncs.com

# quay.io/prometheus/alertmanager:v0.15.1
docker pull quay.io/prometheus/alertmanager:v0.15.1 && \
docker tag quay.io/prometheus/alertmanager:v0.15.1 registry-vpc.cn-qingdao.aliyuncs.com/wod/alertmanager:v0.15.1 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/alertmanager:v0.15.1

# grafana/grafana:5.2.1
docker pull grafana/grafana:5.2.1 && \
docker tag grafana/grafana:5.2.1 registry-vpc.cn-qingdao.aliyuncs.com/wod/grafana:5.2.1 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/grafana:5.2.1

docker pull quay.io/coreos/grafana-watcher:v0.0.8 && \
docker tag quay.io/coreos/grafana-watcher:v0.0.8 registry-vpc.cn-qingdao.aliyuncs.com/wod/grafana-watcher:v0.0.8 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/grafana-watcher:v0.0.8

# quay.io/prometheus/prometheus:v2.2.1
docker pull quay.io/prometheus/prometheus:v2.2.1 && \
docker tag quay.io/prometheus/prometheus:v2.2.1 registry-vpc.cn-qingdao.aliyuncs.com/wod/prometheus:v2.2.1 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/prometheus:v2.2.1

# quay.io/coreos/prometheus-operator:v0.20.0
docker pull quay.io/coreos/prometheus-operator:v0.20.0 && \
docker tag quay.io/coreos/prometheus-operator:v0.20.0 registry-vpc.cn-qingdao.aliyuncs.com/wod/prometheus-operator:v0.20.0  && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/prometheus-operator:v0.20.0 

docker pull quay.io/coreos/configmap-reload:v0.0.1 && \
docker tag quay.io/coreos/configmap-reload:v0.0.1 registry-vpc.cn-qingdao.aliyuncs.com/wod/configmap-reload:v0.0.1 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/configmap-reload:v0.0.1

docker pull quay.io/coreos/prometheus-config-reloader:v0.20.0 && \
docker tag quay.io/coreos/prometheus-config-reloader:v0.20.0 registry-vpc.cn-qingdao.aliyuncs.com/wod/prometheus-config-reloader:v0.20.0 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/prometheus-config-reloader:v0.20.0

docker pull quay.io/coreos/hyperkube:v1.7.6_coreos.0 && \
docker tag quay.io/coreos/hyperkube:v1.7.6_coreos.0 registry-vpc.cn-qingdao.aliyuncs.com/wod/hyperkube:v1.7.6_coreos.0 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/hyperkube:v1.7.6_coreos.0

# quay.io/prometheus/node-exporter:v0.15.2
docker pull quay.io/prometheus/node-exporter:v0.15.2 && \
docker tag quay.io/prometheus/node-exporter:v0.15.2 registry-vpc.cn-qingdao.aliyuncs.com/wod/node-exporter:v0.15.2 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/node-exporter:v0.15.2

# registry-vpc.cn-qingdao.aliyuncs.com/google_containers/kube-state-metrics:v1.2.0
docker pull registry.cn-hangzhou.aliyuncs.com/google_containers/kube-state-metrics:v1.2.0 && \
docker tag registry.cn-hangzhou.aliyuncs.com/google_containers/kube-state-metrics:v1.2.0  registry-vpc.cn-qingdao.aliyuncs.com/wod/kube-state-metrics:v1.2.0 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/kube-state-metrics:v1.2.0

docker pull registry.cn-hangzhou.aliyuncs.com/google_containers/addon-resizer:1.7 && \
docker tag registry.cn-hangzhou.aliyuncs.com/google_containers/addon-resizer:1.7 registry-vpc.cn-qingdao.aliyuncs.com/wod/addon-resizer:1.7 && \
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/addon-resizer:1.7
```