## Install [Mint](https://www.linuxmint.com)

Prefer the Xfce desktop

## Install Chromium, Git

sudo apt-get install chromium-browser git terminator vim geany tree htop

## Customize your development enviorment

* mkdir -p ~/workspace/github
* git clone --recursive git@github.com:liangyulai/ubuntu-configuration.git
* ln -s ~/workspace/github/ubuntu-configuration/zshrc ~/.zshrc
* sudo chsh -s /bin/zsh


## [Install Docker](https://docs.docker.com/engine/installation/linux/ubuntulinux/)

```
$ sudo apt-get update
$ sudo apt-get install apt-transport-https ca-certificates
$ sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D

$ echo "deb https://apt.dockerproject.org/repo ubuntu-xenial main" | sudo tee /etc/apt/sources.list.d/docker.list
$ sudo apt-get update
$ sudo apt-get install linux-image-extra-$(uname -r) linux-image-extra-virtual

$ sudo apt-get install linux-image-generic
$ sudo apt-get install linux-headers-generic
$ sudo apt-get install linux-image-extra-virtual
```

```
$ sudo apt-get install docker-engine

$ sudo groupadd docker
$ sudo usermod -aG docker $USER
```
