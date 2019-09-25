
## Zawartość do dodania w profilu bash dla kube-ps1 oraz autodopełniania (bash-completion)

```
export BASH_COMPLETION_COMPAT_DIR="/usr/local/etc/bash_completion.d" 

[[ -r "/usr/local/etc/profile.d/bash_completion.sh" ]] && . "/usr/local/etc/profile.d/bash_completion.sh" 

 

source "/usr/local/opt/kube-ps1/share/kube-ps1.sh" 

PS1='$(kube_ps1)'$PS1
```
