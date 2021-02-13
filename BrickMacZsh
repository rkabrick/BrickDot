# Zsh History #
HISTFILE="$HOME/.zshstory"
HISTSIZE=10000000
SAVEHIST=10000000

autoload -Uz compinit && compinit
# Brick Env #
export EDITOR="/usr/bin/nvim"

# NVIDIA OptiX
# export OptiX_INSTALL_DIR="/home/brick/BrickLib/NVIDIA-OptiX-SDK-6.5.0-linux64"
export OptiX_INSTALL_DIR="/home/brick/BrickLib/nvidia/NVIDIA-OptiX-SDK-7.2.0-linux64-x86_64"

### Brick Path
path+=home/brick/.local/bin
path+=/usr/local/bin
path+=/snap/bin
path+=/opt/intel
path+=/home/brick/BrickApps
path+=/home/brick/.local/bin
path+=/home/brick/.cargo/bin
path+=/home/brick/.nix-profile/bin
path+=/home/brick/BrickConfig/BrickScripts 
path+=/home/brick/nsight-systems-2020.5.1/bin
export PATH

# export PATH="#/usr/local/java/jre1.8.0_281/bin:$PATH"

# Custom Brick Functions
source ~/BrickConfig/BrickFunctions.sh
source ~/.BrickZsh/VimEmacs.sh

# Alias vim -> nvim
if type nvim > /dev/null 2>&1; then
  alias vim='nvim'
fi
alias vi="nvim"

antibody bundle < ~/.BrickZsh.txt > ~/.BrickZsh.sh 
source ~/.BrickZsh.sh


# Autocomplete settings 
ZSH_AUTOSUGGEST_STRATEGY=(history completion)
ZSH_AUTOSUGGEST_USE_ASYNC=1
# zstyle ':completion:*:complete:*:' group-order \
  # options arguments values history-words local-directories files builtins 
### ALIASES ###
alias mkbld='mkdir build && cd build'
alias szrc='source ~/.zshrc'
alias cb=clipboard
export ANTIBODY_HOME=~/.antibody/

# 0 -- vanilla completion (abc => abc)
# 1 -- smart case completion (abc => Abc)
# 2 -- word flex completion (abc => A-big-Car)
# 3 -- full flex completion (abc => ABraCadabra)
zstyle ':completion:*' matcher-list '' \
  'm:{a-z\-}={A-Z\_}' \
  'r:[^[:alpha:]]||[[:alpha:]]=** r:|=* m:{a-z\-}={A-Z\_}' \
  'r:|?=** m:{a-z\-}={A-Z\_}'

alias ydl=youtube-dl
alias copy='xclip -sel clip'
export TERM=xterm-256color
export VIMINIT='source $MYVIMRC'
export MYVIMRC='/home/brick/.config/nvim/init.vim'
#compdef _gh gh

# zsh completion for gh                                   -*- shell-script -*-

# FZF Bindings 
# source /usr/share/fzf/completion.zsh
# source /usr/share/fzf/key-bindings.zsh
alias fd=fdfind

export NVDIR=/home/brick/.config/nvim
export NVPLUGS=$NVDIR/vim-plug/plugins.vim
alias cat=bat
if [ -e /home/brick/.nix-profile/etc/profile.d/nix.sh ]; then . /home/brick/.nix-profile/etc/profile.d/nix.sh; fi # added by Nix installer
alias kt='curl -L https://sw.kovidgoyal.net/kitty/installer.sh | sh /dev/stdin'

export SPICETIFY_INSTALL="/home/brick/spicetify-cli"
export PATH="$SPICETIFY_INSTALL:$PATH"

#  Autosuggestion Complete on <tab> 
# bindkey '^E' end-of-line

