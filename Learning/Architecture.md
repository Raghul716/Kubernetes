![image](https://github.com/user-attachments/assets/2d28d41b-dbbe-4435-8e24-fd5b14503de2)

Kubernetes follow the Master - Slave(Worker) Node Architecture.
Master Node : Responsible for the management of Kubernetes cluster. Entry point for all administrative tasks.
Kubernetes can have Multi-Master Architecture.

![image](https://github.com/user-attachments/assets/90657685-2b41-43de-a679-763909769464)


# API Server : 
(Kube-api-server) API server is the entry point for all the REST commands used to control the cluster. It is the interaction Point with Kubernetes cluster.

# Etcd : 
Distributed keyvalue store whichstores the cluster state. Used as Back-End for K8s. Provides high availability of Data related to Cluster State.

# Scheduler : 
Regulates the tasks on slave nodes. Stores the resource usage information for each slave node.

# Controller : 
Runs multiple Controller utility in single process. Carry on Automated tasks in K8s Cluster.

# Worker Node : 
It’s a physical server or you can say a VM where the container managed by the Cluster Run. Worker nodes contain all the necessary services to manage the networking between the containers, communicate with the master node, and assign resources to the scheduled containers.

# Kubelet : 
K8s Agent executed on the worker nodes Kubelet gets the configuration of a Pod from the API server and ensures that the described containers are up and running.

# Pods : 
Is a group of one or more containers with shared storage/network, and a specification for how to run the containers. Share the Same Shared content and same IP but reach other Pods via LocalHost. Single Pod can Run on Multiple Machines and Single Machine can Run Multiple Pods.

# Kube-Proxy : 
Kube-proxy runs on each node to deal with individual host sub-netting and ensure that the services are available to external parties. Kube-proxy acts as a network proxy and a load balancer for a service on a single worker node.

 









