# docker_tutorial

## การติดตั้ง Docker บน Ubuntu 18

```git
   sudo apt-get update
```

```git
  sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common
```

```git
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```

```git
sudo apt-key fingerprint 0EBFCD88
```

```git
sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
```

```git
  sudo apt-get update
```

```git
sudo apt-get install docker-ce docker-ce-cli containerd.io
```

```git
apt-cache madison docker-ce
```

```git
sudo apt-get update
```

## ติดตั้ง git บน Ubuntu 18

```git
sudo apt-get install git
```

### ติดตั้ง Docker Compose บน Ubuntu 18

```
sudo apt-get update
```

```
sudo curl -L "https://github.com/docker/compose/releases/download/1.28.5/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

```
sudo chmod +x /usr/local/bin/docker-compose
```

```
sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
```

- เช็กเวอร์ชันของ Docker Compose

```
sudo docker-compose --version
```
