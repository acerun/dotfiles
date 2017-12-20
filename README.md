## Install
git clone https://github.com/futureinsky/dotfiles.git ~/.dotfiles  
cd ~/.dotfiles  
ls -A | grep -v "README*\|.git$" | xargs -i ln -s -f ~/.dotfiles/{} ~/  

