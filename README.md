## 👋 Welcome to mssql 🚀

Self-hosted mssql application

## 📋 Description

Self-hosted mssql application

## 🚀 Services

- **admin**: adminer:latest
- **db**: mcr.microsoft.com/mssql/server:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/mssql/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/mssql" ~/.local/srv/docker/mssql
cd ~/.local/srv/docker/mssql
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install mssql
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:59085

## 📂 Volumes

- `./volumes/data/db/mssql` - Data storage
- `./volumes/config/mssql/initdb` - Data storage

## 🔍 Logging

```shell
docker compose logs -f admin
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
