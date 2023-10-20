# zsh-gcloud-prompt
Show current gcloud config in zsh prompt.

This script is inspired by [zsh-gcloud-prompt](https://github.com/ocadaruma/zsh-gcloud-prompt)

Extra feature avoid overwrite of RPROMPT config for other plugin and possibility to enable or disable display of gcloud config

![capture](capture.png)

## Installation

#### 1. Check out the repository.

```
$ git clone https://github.com/P00L/zsh-gcloud-prompt.git  ~/.oh-my-zsh/custom/plugins/zsh-gcloud-prompt
```

#### 2. Configure your zsh

Current gcloud config is stored in `ZSH_GCLOUD_PROMPT`. (in the form of `"${active-account}:${active-project}"`)

For example, add following lines to `~/.zshrc`

```
autoload -Uz colors; colors
source ~/.oh-my-zsh/custom/plugins/zsh-gcloud-prompt/gcloud.zsh
```

to enable plugin

```
gcp_prompt_info_on
```


to disable plugin

```
gcp_prompt_info_off
```