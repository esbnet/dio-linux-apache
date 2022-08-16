# Provisionamento de servidor apache

Script para provisionar um servidor web no linux

## Atualizando o servidor

### 1. Sequência de comandos para atualizar o servidor apache2
```
apt-get update
apt-get upgrade -y
apt-get install apache2 -y
apt-get install unzip -y
```

### 2. Baixando, descompactando e copiando os arquivos da aplicação para o servidor web

```
cd /tmp
wget https://github.com/denilsonbonatti/linux-site-dio/archive/refs/heads/main.zip
unzip main.zip
cd linux-site-dio-main
cp -R * /var/www/html/
```

