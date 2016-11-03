## Install [Mint](https://www.linuxmint.com)

I prefer the Xfce desktop

## Install Chromium, Git vim etc.

sudo apt-get install chromium-browser git terminator vim geany tree htop

## Customize your development enviorment

```
mkdir -p ~/workspace/github
cd ~/workspace/github
git clone --recursive git@github.com:liangyulai/ubuntu-configuration.git
ln -s ~/workspace/github/ubuntu-configuration/zshrc ~/.zshrc
sudo chsh -s /bin/zsh
```

### Chose your editor
#### ![](https://www.meteor.com/assets/icon-atom.svg) [ATOM: A hackable text editor](https://atom.io/)
```
```

#### ![](https://www.meteor.com/assets/icon-subline.svg) [Sublime Text 3](https://www.sublimetext.com/3)
```
```

#### ![](https://www.meteor.com/assets/icon-visual.svg) [Visual Studio Code](https://code.visualstudio.com/download)
```
```

#### ![](https://www.meteor.com/assets/icon-webstr.svg) [WebStrom](https://www.jetbrains.com/webstorm/)
```
```

## [Install Docker](https://docs.docker.com/engine/installation/linux/ubuntulinux/)

```
sudo apt-get update
sudo apt-get install apt-transport-https ca-certificates
sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D

echo "deb https://apt.dockerproject.org/repo ubuntu-xenial main" | sudo tee /etc/apt/sources.list.d/docker.list
sudo apt-get update
sudo apt-get install linux-image-extra-$(uname -r) linux-image-extra-virtual


sudo apt-get install linux-image-generic
sudo apt-get install linux-headers-generic
sudo apt-get install linux-image-extra-virtual
```

```
sudo apt-get install docker-engine

sudo groupadd docker
sudo usermod -aG docker $USER
```



## [Install Node.js](https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions)
```
curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
sudo apt-get install -y nodejs
sudo apt-get install -y build-essential
```

## [Meteor](https://www.meteor.com/install)

```
curl https://install.meteor.com/ | sh
sudo cp ~/.meteor/packages/meteor-tool/1.4.1_3/mt-os.linux.x86_64/scripts/admin/launch-meteor /usr/local/bin/meteor
```
