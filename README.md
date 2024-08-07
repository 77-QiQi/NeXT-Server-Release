# NeXT-Server-Release

## 安装 Docker & Compose 便携版

```
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh && rm -f get-docker.sh
curl -SL https://github.com/docker/compose/releases/latest/download/docker-compose-linux-x86_64 -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
docker-compose -v
```

## 安装 NeXT-Server

```
git clone https://github.com/77-QiQi/NeXT-Server-Release.git
cd NeXT-Server-Release/
cp config/config.yml.example config/config.yml
```
编辑 config/config.yml 文件

### 启动 / 更新 NeXT-Server
```
docker-compose pull
docker-compose up -d
```
