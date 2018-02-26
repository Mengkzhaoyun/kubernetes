kubectl delete secret traefik-cert --namespace=devops

cd /data/traefik/ssl &&\
kubectl create secret generic traefik-cert \
--from-file=gitlab.ct.csii.com.cn.crt --from-file=gitlab.ct.csii.com.cn.key \
--from-file=harbor.ct.csii.com.cn.crt --from-file=harbor.ct.csii.com.cn.key \
--namespace=devops