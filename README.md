# Setup Server

Đây là bước đầu tiên để setup môi trường, các ứng dụng để lưu trữ dữ liệu.
Các ứng dụng sẽ được cài đặt: Redis, MariaDB, Nginx Proxy

- [ ] MariaDB
- [ ] Mysql Backup ( cho việc backup dữ liệu thường xuyên)
- [ ] Nginx proxy manager
- [ ] Redis

## Prerequisites

Trước tiên cần cài đặt Docker & Docker Compose

- [ ] [Docker Engine for Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
- [ ] [Docker Desktop for Windows](https://docs.docker.com/desktop/install/windows-install/)
- [ ] [Docker Desktop for Macos](https://docs.docker.com/desktop/install/mac-install/)

## Installation

Trước khi cài đặt, chúng ta có thể thay đổi các thông tin cơ bản như user, password cho mariadb tại file .env

Sử dụng terminal chạy command sau ở thư mục gốc

```bash
docker compose up -d --build
```

## Setup

Note khi setup

## Project Service Names

Services trong stack nay dung ten rieng de tranh trung voi container dang chay san:

- `maternity-proxy`: host ports `80`, `81`, `443`
- `maternity-redis`: Redis 7.2, host port `6379`, Docker network port `6379`
- `maternity-mariadb`: host port `3306`, Docker network port `3306`
- `maternity-mysql-backup`

Backend Docker container ket noi noi bo qua network:

- `DB_HOST=maternity-mariadb`, `DB_PORT=3306`
- `REDIS_HOST=maternity-redis`, `REDIS_PORT=6379`

## Hoàn thành
