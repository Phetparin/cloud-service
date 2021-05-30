# Cloud-Service

### Docker Image/Set up the repository:
```sh
$ sudo apt-get update
$ sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
$ echo \
  "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

### Docker Image Install:
```sh
$ sudo apt-get update
$ sudo apt-get install docker-ce docker-ce-cli containerd.io
```

### Install Docker-Compose on Linux systems:
```sh
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

### Upgrade Docker-Compose on Linux systems:
```sh
$ docker-compose migrate-to-labels
```

### Docker-Compose Build:
```sh
$ cd /hw-me #into location file
$ docker-compose build
```

### Start service:
```sh
$ docker-compose up
```

### Stop service:
```sh
$ docker-compose down
```
