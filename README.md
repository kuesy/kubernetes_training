# k8s_training
## docker setup
1. install docker
```
$ sudo apt update && sudo apt install -y docker.io
```
2. give ubuntu user permission to execute docker command
```
$ sudo usermod -aG docker ubuntu
$ sudo systemctl restart docker

$ exit
$ ssh -i ...
```
## kubernetes setup
1. install kubernetes install(use minikube)
```
$ wget https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
$ sudo chmod +x minikube-linux-amd64
$ sudo mv minikube-linux-amd64 /usr/local/bin/minikube

$ minikube start
```
2. kubectl install
```
$ curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
$ sudo chmod +x kubectl
$ sudo mv kubectl /usr/local/bin/kubectl
```
