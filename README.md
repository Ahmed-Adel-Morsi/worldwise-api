# WorldWise API (Backend)

Lightweight JSON Server backend used by the WorldWise frontend.

## Live Links

- Frontend repo: https://github.com/Ahmed-Adel-Morsi/Worldwise
- Backend repo: https://github.com/Ahmed-Adel-Morsi/worldwise-api
- Live API base URL: https://worldwise-api-9gg8.onrender.com/

## What This API Does

- Serves city travel records from `db.json`.
- Supports basic REST operations for the `cities` resource.
- Runs with `json-server` in a small Node entrypoint (`index.js`).

## Tech Stack

- Node.js
- json-server

## Scripts

- `npm start` — run API server

## Run Locally

```bash
npm install
npm start
```

Default local URL:

- `http://localhost:8080`

## Available Endpoints

`json-server` exposes standard REST routes for `cities`:

- `GET /cities`
- `GET /cities/:id`
- `POST /cities`
- `PATCH /cities/:id`
- `PUT /cities/:id`
- `DELETE /cities/:id`

## Data Shape (cities)

Each city object in `db.json` includes fields like:

- `id`
- `cityName`
- `country`
- `emoji`
- `date`
- `notes`
- `position` (`lat`, `lng`)

## Deployment

This API is deployed on Render and consumed by the frontend:

- https://worldwise-api-9gg8.onrender.com/
