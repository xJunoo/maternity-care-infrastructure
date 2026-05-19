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

## Hoàn thành
