# Kubectl:

kubectl is a command-line tool used to interact with Kubernetes clusters. It provides a way to manage and control various Kubernetes resources, such as deployments, pods, services, and more

# Key functions of kubectl:

Create, update, and delete Kubernetes resources: Use kubectl to create new resources, modify existing ones, and delete resources when they are no longer needed.

List and view resources: Get information about the status and configuration of different Kubernetes resources.

Run commands in containers: Execute commands within running containers within a pod.

Manage namespaces: Create, delete, and switch between different namespaces within a Kubernetes cluster.

Interact with the Kubernetes API server: kubectl communicates directly with the Kubernetes API server to perform various operations.

# Example commands

# ➤ Kubectl get

Kubectl get is used to get the objects, present in K8s Cluster
$ kubectl get <object_type> <object_name> -o <output> —sort-by <JSONpath> —selector <selector>

#kubectl get pod draining-node-test-pod -o json 


➤ Kubectl describe

kubectl describe <object_type> <object_name>
#kubectl describe pod draining-node-test-pod

➤ Kubectl create

kubectl create -f pod.yaml

➤ Kubectl apply

kubectl apply -f pod.yaml
If user use kubectl apply on already existing object. It will modify the existing object, if possible.

➤ Kubectl delete

kubectl delete <object_type> <object_name>

➤ Kubectl exec

kubectl exec draining-node-test-pod -c nginx -- cat /etc/nginx/nginx.conf

kubectl api-resources

