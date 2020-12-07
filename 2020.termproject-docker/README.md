---
title : smart factory dockerize
---



# docker installation 

ref : https://docs.docker.com/engine/install/ubuntu/

```zsh
sudo apt-get remove docker docker-engine docker.io containerd runc
sudo apt-get update
sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common
    
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo apt-key fingerprint 0EBFCD88

sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
   
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io
```



# docker-compose installation

```zsh
sudo curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```



# docker image build

```zsh
docker-compose build
```



# Application Running

- move to application root directory

```zsh
docker-compose up # Run with prompt
docker-compose up -d # Run as daemon
```



# Application Termination

```
docker-compose down
```

