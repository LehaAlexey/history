# History Service

Сервис читает `PriceMeasured` из Kafka, пишет в History DB и обновляет Redis (последние измерения).

## Запуск

- Docker: `docker compose up -d --build`
- Локально (Windows PowerShell): `$env:configPath = ".\\config.yaml"` и `go run .\\cmd\\app`

gRPC: `:50062`
Health: `http://localhost:8072/health`

