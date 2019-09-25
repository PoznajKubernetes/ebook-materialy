
## Instalacja WSL

```
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux 
```

## Instalacja kubectl

```
curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add 

echo "deb http://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee /etc/apt/sources.list.d/kubernetes.list 

sudo apt update 

sudo apt install kubectl 
echo 'source <(kubectl completion bash)' >>~/.bashrc
```

## Instalacja kubens i kubectx

```
git clone https://github.com/ahmetb/kubectx.git ~/.kubectx 

sudo ln -sf ~/.kubectx/completion/kubens.bash /etc/bash_completion.d/kubens 

sudo ln -sf ~/.kubectx/completion/kubectx.bash /etc/bash_completion.d/kubectx 

cat << FOE >> ~/.bashrc 

#kubectx and kubens 

export PATH=~/.kubectx:\$PATH 

FOE
```

## Instalacja kube-ps1

```
git clone https://github.com/jonmosco/kube-ps1  ~/.kube-ps1 
```

## Zawartość do dodania w profilu bash dla kube-ps1

```
source  ~/.kube-ps1/kube-ps1.sh 

PS1='[\u@\h \W $(kube_ps1)]\$ '
```
