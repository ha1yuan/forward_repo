# forward_repo

A simple Go HTTP server scaffold.

## Quick Start

```bash
go run cmd/server/main.go
```

Server listens on `:8080` by default. Override with `ADDR` env var:

```bash
ADDR=:3000 go run cmd/server/main.go
```

## Endpoints

| Method | Path      | Description       |
|--------|-----------|-------------------|
| GET    | `/`       | Hello response    |
| GET    | `/health` | Health check (JSON)|

## Graceful Shutdown

The server handles `SIGINT` and `SIGTERM` for graceful shutdown with a 5s timeout.
