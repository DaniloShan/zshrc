```shell
# Path to your oh-my-zsh configuration.
ZSH=$HOME/.oh-my-zsh

# Set name of the theme to load.
# Look in ~/.oh-my-zsh/themes/
# Optionally, if you set this to "random", it'll load a random theme each
# time that oh-my-zsh is loaded.
ZSH_THEME="robbyrussell"

# Example aliases
# alias zshconfig="mate ~/.zshrc"
# alias ohmyzsh="mate ~/.oh-my-zsh"

# Set to this to use case-sensitive completion
# CASE_SENSITIVE="true"

# Uncomment this to disable bi-weekly auto-update checks
# DISABLE_AUTO_UPDATE="true"

# Uncomment to change how often before auto-updates occur? (in days)
# export UPDATE_ZSH_DAYS=13

# Uncomment following line if you want to disable colors in ls
# DISABLE_LS_COLORS="true"

# Uncomment following line if you want to disable autosetting terminal title.
# DISABLE_AUTO_TITLE="true"

# Uncomment following line if you want to disable command autocorrection
# DISABLE_CORRECTION="true"

# Uncomment following line if you want red dots to be displayed while waiting for completion
# COMPLETION_WAITING_DOTS="true"

# Uncomment following line if you want to disable marking untracked files under
# VCS as dirty. This makes repository status check for large repositories much,
# much faster.
# DISABLE_UNTRACKED_FILES_DIRTY="true"

# Uncomment following line if you want to  shown in the command execution time stamp 
# in the history command output. The optional three formats: "mm/dd/yyyy"|"dd.mm.yyyy"|
# yyyy-mm-dd
# HIST_STAMPS="mm/dd/yyyy"

# Which plugins would you like to load? (plugins can be found in ~/.oh-my-zsh/plugins/*)
# Custom plugins may be added to ~/.oh-my-zsh/custom/plugins/
# Example format: plugins=(rails git textmate ruby lighthouse)
plugins=(git)

source $ZSH/oh-my-zsh.sh

# User configuration

#export PATH="/Library/ImageMagick/bin:/usr/local/bin/emacs-24.3:/usr/bin:/bin:/usr/sbin:/sbin:/usr/local/bin:/Users/danilo/bin:/usr/local/oracle/instantclient_10_2"
# export MANPATH="/usr/local/man:$MANPATH"

# # Preferred editor for local and remote sessions
# if [[ -n $SSH_CONNECTION ]]; then
#   export EDITOR='vim'
# else
#   export EDITOR='mvim'
# fi

# Compilation flags
# export ARCHFLAGS="-arch x86_64"

# ssh
# export SSH_KEY_PATH="~/.ssh/dsa_id"

[[ -s "$HOME/.rvm/scripts/rvm" ]] && source "$HOME/.rvm/scripts/rvm" # Load RVM into a shell session *as a function*

#alias cp='cp -i'
alias ll='ls -lG'
# alias php-fpm='/usr/local/sbin/php-fpm'

# export PATH="$(brew --prefix php55)/bin:$PATH"
#export PATH="/usr/local/Cellar/nginx/1.4.4/bin:$PATH"
export PATH="/usr/local/Cellar/nginx/1.6.1_1/bin:$PATH"

export MAGICK_HOME=/Library/ImageMagick
export PATH=$MAGICK_HOME/bin:$PATH
export PATH=${PATH}:~/bin
export PATH="/usr/local/Cellar/node/0.10.35/bin:$PATH"
export PATH="$HOME/.node/bin:$PATH"
export PATH="/Users/danilo/.node/bin:$PATH"

# Âø´Êç∑Ë∑ØÂæÑ
alias f2e='cd /Users/danilo/Sites/mobile-fe'
alias nodejs='cd ~/Sites/node/'
#alias back='cd ~/Sites/netease/backend/finance/trunk/php/'
alias site='cd ~/Sites/'
alias 360='cd ~/Sites/360/'
alias private='cd ~/Sites/private'
alias algo='cd ~/Sites/algorithm'
alias algorithm='cd ~/Sites/algorithm'
alias hosts='sudo emacs /etc/hosts'
alias nginx.conf="emacs /usr/local/etc/nginx/nginx.conf"
alias nebula='cd ~/Sites/nebula'
alias nebulajs='cd /Users/danilo/Sites/nebula/nebulajs'
alias test='cd ~/Sites/test'
alias mock='node-dev /Users/danilo/Sites/node/mock/app.js'
alias python='python3'
alias py='python3'
alias py2='/usr/bin/python'
alias tree='tree -L 2'
alias traceur='/Users/danilo/Sites/libs/traceur-compiler/traceur'

alias gorestart='launchctl unload -w ~/Library/LaunchAgents/com.google.goagent.plist;launchctl load -w ~/Library/LaunchAgents/com.google.goagent.plist'

alias up='svn up'

alias doc="cd ~/Documents"
alias down="cd ~/Downloads"
alias desk="cd ~/Desktop"

alias -s html=emacs
alias -s rb=emacs  
alias -s py=emacs
alias -s js=emacs
alias -s css=emacs
alias -s less=emacs
alias -s c=emacs
alias -s java=emacs
alias -s txt=emasc

export PATH=/usr/local/bin:$PATH
ZSH_THEME="ys"
export PATH="$(brew --prefix homebrew/php/php55)/sbin:$PATH"

# Setup zsh-autosuggestions
source ~/.zsh-autosuggestions/autosuggestions.zsh

# Enable autosuggestions automatically
zle-line-init() {
    zle autosuggest-start
}

zle -N zle-line-init

# use ctrl+t to toggle autosuggestions(hopefully this wont be needed as
# zsh-autosuggestions is designed to be unobtrusive)
bindkey '^T' autosuggest-toggle
[[ -s $(brew --prefix)/etc/autojump.sh ]] && . $(brew --prefix)/etc/autojump.sh

```
