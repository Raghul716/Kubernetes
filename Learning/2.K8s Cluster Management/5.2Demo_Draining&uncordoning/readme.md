Create a directory in master node
pull the yaml files deployment.yaml and pod.yaml

#kubectl get nodes

#kubectl get pods -o wide                ---------to know all the running pods

#kubectl apply -f pod.yaml               ---------to start the pod

#kubectl apply -f deployment.yaml        

#kubectl get pods -o wide

#kubectl drain paradox2 --ignore-daemonsets --force      ---to drain the node

#kubectl get nodes                       

#kubectl uncordon paradox2                               ---to uncordon the node

#kubectl get pods -o wide





--



