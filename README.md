# PostgreSQL and pgAdmin with Docker Compose

**Author:** Robson Niemeyer  
**Repository:** [https://github.com/nierobs/postgres-pgadmin](https://github.com/nierobs/postgres-pgadmin)

## Directory structure

```bash
.
├── .dockerignore
├── .env
├── .gitignore
├── README.md
├── compose.yaml
└── init.sql
```
## Beginner's guide

### 1. Before building the containers

```bash
$ mkdir -p data/{pgadmin,postgres}
$ sudo chown -R 5050:5050 ./data/pgadmin
```

### 2. Build and start containers

```bash
$ docker compose up -d
```

### 3. Login credentials

#### pgAdmin

**Base URL:** http://localhost:5050  
**Email:** admin@admin.com  
**Password:** 123456

#### Postgres

**Host name:** localhost  
**Port:** 5432  
**Username:**  admin  
**Password:** 123456

### 4. Stop and remove containers and images

```bash
$ docker compose down --rmi all
```

