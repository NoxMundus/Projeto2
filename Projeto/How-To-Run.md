## Como rodar o projeto

IMPORTANTE: Garanta que a estrutura de arquivos é preservada conforme o GitHub. Os paths estão considerando essa estrutura. 
O Makefile não é nescessario, só ficou para caso queria facilitar alguns comandos

### 1. Install docker, caso tenham falhas em usar comandos com o docker só

sudo yum install -y yum-utils

sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo

sudo yum install docker

sudo groupadd docker

#### Coloque seu usuario
sudo usermod -aG docker ec2-user

newgrp docker

docker version

sudo systemctl start docker

### 2. Install docker-compose, caso tenham falhas em usar comandos com o docker só, usar sudo 

sudo curl -SL https://github.com/docker/compose/releases/download/v2.24.6/docker-compose-linux-x86_64 -o /usr/local/bin/docker-compose

sudo chmod +x /usr/local/bin/docker-compose

docker-compose version

#### 2.1 Uma vez feito a instalação do docker compose. Faça um up, na pasta de Projeto em que estiver o arquivo do compose passado. 

docker-compose up