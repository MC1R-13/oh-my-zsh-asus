# Install Oh My Zsh on Asus Router

## Before the install 

- Know how to use [ssh](https://www.unix.com/man-page/redhat/1/ssh/), [git](https://git-scm.com/), and [Entware](https://github.com/Entware/Entware)
- [Entware](https://github.com/Entware/Entware) is installed on your Asus router

## Install 
- Install these commands with Entware
```
opkg install zsh
opkg install git-http
````
You should already have the `curl` command

- Download and install

```
curl -Lo install.sh https://raw.githubusercontent.com/usercase/oh-my-zsh/master/tools/install.sh
sh install.sh --unattended
```

- Type zsh to start the shell 

## Author modifications of the install script
The script has slightly changed, I replaced the `command` command (yes !) with the `which`command.
Unfortunately the above command doesn't exist on Asus router, and you can not install it via Entware.

The script is based on the work of Robby Russel and other developers, have a look there : 
https://github.com/robbyrussell/oh-my-zsh
