# My dotfiles
## Pre-Install
### oh-my-zsh
* via curl
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
* via wget
`sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"`

### VIM
* Reference https://github.com/Valloric/YouCompleteMe/wiki/Building-Vim-from-source
* VIM8
```
git clone https://github.com/vim/vim.git
cd vim/src
make
```
* .vimrc
```
git clone https://github.com/futureinsky/.vim.git ~/.vim
ln -s ~/.vim/.vimrc ~/.vimrc
```

### Tmux
```
sudo apt install -y automake
sudo apt install -y build-essential
sudo apt install -y pkg-config
sudo apt install -y libevent-dev
sudo apt install -y libncurses5-dev

git clone https://github.com/tmux/tmux.git /tmp/tmux
cd /tmp/tmux
sh autogen.sh
./configure && make
sudo make install
```

## Install
```
git clone https://github.com/futureinsky/dotfiles.git ~/.dotfiles  
cd ~/.dotfiles  
ls -A | grep -v "README*\|.git$" | xargs -i ln -s -f ~/.dotfiles/{} ~/  
```

