# Inventory Service API

Сервис обмена остатками товаров между магазинами.

## Запуск локально

```bash
uvicorn app.main:app --reload
```

## Docker

```bash
docker build -t inventory-service .
docker run -d -p 8000:8000 inventory-service
```

## Эндпоинты

- `POST /update_stock/` — обновить остаток
- `GET /stock/{product_id}` — получить остатки по товару
