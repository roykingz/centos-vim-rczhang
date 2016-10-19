这些vim配置文件可以安装一些好用的vim插件，并改变vim外观
切换到普通用户（以下命令均在普通用户下执行）

cd ~

mv .vim .vim_bak

mv .vimrc .vimrc_bak

mv .bashrc .bashrc_bak

git clone https://github.com/roykingz/centos-vim-rczhang.git

cd centos-vim-rczhang

mv .bashrc .vim/ .vimrc ~

git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle

cd ~

rm -rf centos-vim-rczhang/

sudo pip install powerline-status


下面的命令只是为使shell提示符有个酷炫的效果，可以不执行

. /usr/lib/python2.7/site-packages/powerline/bindings/bash/powerline.sh


然后切换为root用户，再执行一遍上述命令，使得root的vim和shell提示符也有上述效果。
