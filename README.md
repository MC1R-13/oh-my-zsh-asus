# Installation of Oh My Zsh on Asus Routers

## Before 

- Know how to use [ssh](https://www.unix.com/man-page/redhat/1/ssh/), [git](https://git-scm.com/), and [Entware](https://github.com/Entware/Entware)
- [Entware](https://github.com/Entware/Entware) is installed on your Asus router

## Installation
### 1. Install these commands with Entware
```
opkg install zsh
opkg install git-http
````
You should already have the `curl` command

### 2. Download and install

```
curl -Lo install.sh https://raw.githubusercontent.com/usercase/oh-my-zsh/master/tools/install.sh
sh install.sh --unattended
```

### 3. Type zsh to start the shell :thumbsup:

##  About the author's modifications of the installation script
The script has slightly changed, I replaced the `command` command (yes !) with the `which`command.
Unfortunately the above command doesn't exist on Asus router, and you can not install it via Entware.

## License 

[MIT License](https://github.com/robbyrussell/oh-my-zsh/blob/master/LICENSE.txt)

The script is based on the work of Robby Russel and other developers, have a look there : 

https://github.com/robbyrussell/oh-my-zsh
