# saathi-mock-app

Minimal Express app used to validate the Jenkins + Ansible CI/CD pipeline
deploying to the "saathi" GCP VM via pm2, before the real application is ready.

## Routes

- `GET /` — JSON message + timestamp
- `GET /health` — `{ "status": "ok" }`

## Run locally

```bash
npm install
npm start
```

Listens on `process.env.PORT || 4000`, bound to `0.0.0.0`.
