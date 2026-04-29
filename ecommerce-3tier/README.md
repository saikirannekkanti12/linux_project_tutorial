# Online Ecommerce 3-Tier Architecture (Docker)

This sample project demonstrates a classic 3-tier architecture:

1. **Frontend tier**: Nginx serving static HTML/JS (`frontend`)
2. **Application tier**: Node.js + Express REST API (`backend`)
3. **Data tier**: PostgreSQL database (`db`)

## Run

```bash
cd ecommerce-3tier
docker compose up --build
```

## Access

- Frontend: http://localhost:8080
- Backend health: http://localhost:5000/health
- Backend API: http://localhost:5000/api/products

## Stop

```bash
docker compose down
```

To remove DB data volume as well:

```bash
docker compose down -v
```
