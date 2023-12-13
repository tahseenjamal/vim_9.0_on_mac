# VIM 9.0 on Mac OS Sonoma 14.1.12

How to setup vim 9.0 with homebrew

This is about how to install vim 9.0 version on **Mac OS Sonoma 14.1.12**

On terminal enter the following commands

Install vim using brew command

    brew install vim
Go inside the folder using cd command

    cd /usr/local/Cellar/vim/9.0.2150/share/vim/vim90/
Then create symbolic link of bin folder inside it

    ln -s ../../../bin
Then go to the below folder

    cd /usr/local
And create another symbolic link

    sudo ln -s /usr/local/Cellar/vim/9.0.2150/share/vim/vim90 vim

Next add below in your .profile or .zprofile file

    export VIM="/usr/local/vim"
    export PATH=$VIM:$VIM/bin:$PATH
