# ZSHRC

```bash
export ZSH="$HOME/.oh-my-zsh"

ZSH_THEME="robbyrussell"

plugins=(git brew rails python)

source $ZSH/oh-my-zsh.sh

# User configuration

export LANG="en_US.UTF-8"
export LC_ALL="en_US.UTF-8"
export LC_CTYPE="en_US.UTF-8"

alias cleanup='brew cleanup --prune=1 && yarn cache clean && composer clearcache'

export PATH="/usr/local/opt/python@3.11/libexec/bin:$PATH"

alias python='python3'
alias dev='cd /Volumes/Code'

export EDITOR='nano'
export VISUAL='nano'

export PATH="/usr/local/sbin:$PATH"
export PATH="/usr/local/opt/ruby/bin:$PATH"
export PATH="/usr/local/lib/ruby/gems/3.1.0/bin:$PATH"

export HOMEBREW_NO_ENV_HINTS=true
```