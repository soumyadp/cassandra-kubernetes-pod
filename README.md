# Apache Cassandra pod for Kubernetes cluster
A Kubernetes pod for Apache Cassandra containers. By default, pod will contain 3 containers. You can easily scale up and down by editing the cassandra.yml file in the repository. The containers use a glusterFS persistent volume to store data. In case of container/service crash, the data is still persisted and mapped to the new containers which come up.

# Run
kubectl create -f cassandra.yml
