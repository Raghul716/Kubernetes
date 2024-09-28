# Text Direction : Install Kubernetes using MiniKube

# ********** Install Docker CE Edition **********

sudo apt-get remove docker docker-engine docker.io containerd runc

sudo apt-get update

https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository

# ********** Install KubeCtl **********

https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/#install-kubectl-binary-with-curl-on-linux

1.Download the latest release with the command:
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"

2.Validate the binary (optional)
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl.sha256"
echo "$(cat kubectl.sha256)  kubectl" | sha256sum --check

3.Install kubectl
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl

4.Test to ensure the version you installed is up-to-date:
kubectl version --client

# ********** Install MiniKube **********

https://minikube.sigs.k8s.io/docs/start/?arch=%2Flinux%2Fx86-64%2Fstable%2Fbinary+download

1.Installation
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube && rm minikube-linux-amd64

3.Verify Installation
minikube version 









