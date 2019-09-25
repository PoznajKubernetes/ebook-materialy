
## Instalacja minikube

```
curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 \ && chmod +x minikube 

sudo install minikube /usr/local/bin 
```

## Ręczna instalacja kubectl

```
curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl

chmod +x ./kubectl 

sudo install kubectl /usr/local/bin
```

## Instalacja kubectl z APT

```
curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add 

echo "deb http://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee /etc/apt/sources.list.d/kubernetes.list 

sudo apt update 

sudo apt install kubectl
```
