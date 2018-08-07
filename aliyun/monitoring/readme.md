# images
```bash
# quay.io/prometheus/alertmanager:v0.15.1
docker pull quay.io/prometheus/alertmanager:v0.15.1 && \
docker tag quay.io/prometheus/alertmanager:v0.15.1 hub.c.163.com/mengkzhaoyun/k8s:alertmanager-v0.15.1 && \
docker push hub.c.163.com/mengkzhaoyun/k8s:alertmanager-v0.15.1

# grafana/grafana:5.2.1
docker pull grafana/grafana:5.2.1 && \
docker tag grafana/grafana:5.2.1 hub.c.163.com/mengkzhaoyun/k8s:grafana-5.2.1 && \
docker push hub.c.163.com/mengkzhaoyun/k8s:grafana-5.2.1

docker pull quay.io/coreos/grafana-watcher:v0.0.8 && \
docker tag quay.io/coreos/grafana-watcher:v0.0.8 hub.c.163.com/mengkzhaoyun/k8s:grafana-watcher-v0.0.8 && \
docker push hub.c.163.com/mengkzhaoyun/k8s:grafana-watcher-v0.0.8

# quay.io/prometheus/prometheus:v2.2.1
docker pull quay.io/prometheus/prometheus:v2.2.1 && \
docker tag quay.io/prometheus/prometheus:v2.2.1 hub.c.163.com/mengkzhaoyun/k8s:prometheus-v2.2.1 && \
docker push hub.c.163.com/mengkzhaoyun/k8s:prometheus-v2.2.1

# quay.io/coreos/prometheus-operator:v0.20.0
docker pull quay.io/coreos/prometheus-operator:v0.20.0 && \
docker tag quay.io/coreos/prometheus-operator:v0.20.0 hub.c.163.com/mengkzhaoyun/k8s:prometheus-operator-v0.20.0  && \
docker push hub.c.163.com/mengkzhaoyun/k8s:prometheus-operator-v0.20.0 

docker pull quay.io/coreos/configmap-reload:v0.0.1 && \
docker tag quay.io/coreos/configmap-reload:v0.0.1 hub.c.163.com/mengkzhaoyun/k8s:configmap-reload-v0.0.1 && \
docker push hub.c.163.com/mengkzhaoyun/k8s:configmap-reload-v0.0.1

docker pull quay.io/coreos/prometheus-config-reloader:v0.20.0 && \
docker tag quay.io/coreos/prometheus-config-reloader:v0.20.0 ub.c.163.com/mengkzhaoyun/k8s:prometheus-config-reloader-v0.20.0 && \
docker push hub.c.163.com/mengkzhaoyun/k8s:prometheus-config-reloader-v0.20.0

docker pull quay.io/coreos/hyperkube:v1.7.6_coreos.0 && \
docker tag quay.io/coreos/hyperkube:v1.7.6_coreos.0 hub.c.163.com/mengkzhaoyun/k8s:hyperkube-v1.7.6_coreos.0 && \
docker push hub.c.163.com/mengkzhaoyun/k8s:hyperkube-v1.7.6_coreos.0

# quay.io/prometheus/node-exporter:v0.15.2
docker pull quay.io/prometheus/node-exporter:v0.15.2 && \
docker tag quay.io/prometheus/node-exporter:v0.15.2 hub.c.163.com/mengkzhaoyun/k8s:node-exporter-v0.15.2 && \
docker push hub.c.163.com/mengkzhaoyun/k8s:node-exporter-v0.15.2

# registry.cn-hangzhou.aliyuncs.com/google_containers/kube-state-metrics:v1.2.0
docker pull registry.cn-hangzhou.aliyuncs.com/google_containers/kube-state-metrics:v1.2.0 && \
docker tag registry.cn-hangzhou.aliyuncs.com/google_containers/kube-state-metrics:v1.2.0  hub.c.163.com/mengkzhaoyun/k8s:kube-state-metrics-v1.2.0 && \
docker push hub.c.163.com/mengkzhaoyun/k8s:kube-state-metrics-v1.2.0

docker pull registry.cn-hangzhou.aliyuncs.com/google_containers/addon-resizer:1.7 && \
docker tag registry.cn-hangzhou.aliyuncs.com/google_containers/addon-resizer:1.7 hub.c.163.com/mengkzhaoyun/k8s:addon-resizer-1.7 && \
docker push hub.c.163.com/mengkzhaoyun/k8s:addon-resizer-1.7
```