# 🚀 Docker Compose Images Collection

A curated collection of ready-to-use Docker Compose setups for popular databases and message brokers. Instantly spin up local development environments for Redis, PostgreSQL, MySQL, MongoDB, and Kafka with a single command.

---

## 📋 Table of Contents

- [Features](#features)
- [Quick Start](#quick-start)
- [Services](#services)
  - [Redis & RedisInsight](#redis--redisinsight)
  - [PostgreSQL & pgAdmin](#postgresql--pgadmin)
  - [MySQL & phpMyAdmin](#mysql--phpmyadmin)
  - [MongoDB](#mongodb)
  - [Kafka & Zookeeper](#kafka--zookeeper)
- [Contributing](#contributing)
- [License](#license)

---

## ✨ Features

- **Plug & Play**: Launch any service with a single `docker compose up` command.
- **UI Tools Included**: Each database comes with a web-based management UI.
- **Isolated Setups**: Each service is self-contained in its own directory.
- **Pre-configured Connection Strings**: Copy-paste connection strings for instant integration.

---

## ⚡ Quick Start

1. **Clone this repository:**
   ```bash
   git clone https://github.com/shakibkhandev/docker-compose-images.git
   cd docker-compose-images
   ```
2. **Choose a service and start it:**
   ```bash
   cd <service>
   docker compose up -d
   ```
   Replace `<service>` with one of: `redis`, `postgres`, `mysql`, `mongodb`, `kafka`
3. **Access the service and its management UI** (see below for details).

---

## 🛠️ Services

### Redis & RedisInsight

- **Connection String:**
  ```
  redis://localhost:6379
  ```
- **Management UI:** [RedisInsight](http://localhost:8001)

### PostgreSQL & pgAdmin

- **Connection String:**
  ```
  postgresql://postgres:postgres@localhost:6432/postgres
  ```
- **Management UI:** [pgAdmin](http://localhost:8080)
  - _Login:_ `admin@localhost.com` / `admin123`

### MySQL & phpMyAdmin

- **Connection String:**
  ```
  mysql://myuser:mypassword@localhost:3306/mydb
  ```
- **Management UI:** [phpMyAdmin](http://localhost:8082)
  - _Login:_ `myuser` / `mypassword`

### MongoDB

- **Connection String:**
  ```
  mongodb://localhost:27017
  ```
- _No web UI included by default. Use your favorite MongoDB client._

### Kafka & Zookeeper

- **Kafka Broker:** `localhost:9092`
- **Zookeeper:** `localhost:2181`
- _No web UI included by default. Use your favorite Kafka client._

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open an issue or submit a pull request.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
