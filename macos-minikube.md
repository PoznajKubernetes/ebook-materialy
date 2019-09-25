
## Instalacja minikube

```
brew update # aktualizuje formuły możliwe do zainstalowania 

brew tap caskroom/cask # dodaje repozytorium formuł 

brew cask install virtualbox 

brew cask install minikube 
```

## Ręczna instalacja kubectl

```
curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/darwin/amd64/kubectl 

chmod +x ./kubectl 

sudo mv ./kubectl /usr/local/bin/kubectl
```

## Ręczna instalacja minikube

```
curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-amd64 \ && chmod +x minikube 

sudo mv minikube /usr/local/bin 
```
