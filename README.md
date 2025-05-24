# super_knight
# 一键命令大全
## nginx
```bash
apt install curl vim wget gnupg dpkg apt-transport-https lsb-release ca-certificates && curl -sSL https://n.wtf/public.key | gpg --dearmor > /usr/share/keyrings/n.wtf.gpg && echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/n.wtf.gpg] https://mirror-cdn.xtom.com/sb/nginx/ $(lsb_release -sc) main" > /etc/apt/sources.list.d/n.wtf.list && apt update && apt install nginx-extras -y
```


## 安装docker
```bash
apt-get update
wget -qO- get.docker.com | bash
systemctl start docker 
systemctl enable docker 
curl -L "https://github.com/docker/compose/releases/download/v2.35.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
docker-compose --version
```
