docker pull mazdermind/hostpath-provisioner:latest &&\
docker tag mazdermind/hostpath-provisioner:latest registry-vpc.cn-qingdao.aliyuncs.com/wod/hostpath-provisioner:latest &&\
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/hostpath-provisioner:latest


docker pull busybox:1.24 &&\
docker tag busybox:1.24 registry-vpc.cn-qingdao.aliyuncs.com/wod/busybox:1.24 &&\
docker push registry-vpc.cn-qingdao.aliyuncs.com/wod/busybox:1.24