# My dotfiles
## Pre-Install
### oh-my-zsh
* via curl
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
* via wget
`sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"`

### VIM
* VIM8
```
git clone https://github.com/vim/vim.git
cd vim/src
make
```
* .vimrc
```
git clone git@github.com:futureinsky/.vim.git ~/.vim
ln -s ~/.vim/.vimrc ~/.vimrc
```

### Tmux
```
git clone https://github.com/tmux/tmux.git
./configure && make
sudo make install
```

## Install
```
git clone https://github.com/futureinsky/dotfiles.git ~/.dotfiles  
cd ~/.dotfiles  
ls -A | grep -v "README*\|.git$" | xargs -i ln -s -f ~/.dotfiles/{} ~/  
```

