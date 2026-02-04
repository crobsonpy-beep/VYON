# VYON
```markdown
# VYON Discovery Marketplace - Local dev

Prereqs:
- Docker & Docker Compose
- Node 18+, Python 3.11 (for local edits)

1) Generate .env
   powershell infra\env.ps1

2) Build & up
   powershell infra\docker.ps1
   (ou) docker-compose up --build

3) Services:
   - API Gateway: http://localhost:3000/api/health
   - Frontend: http://localhost:8080
   - Auth: http://localhost:4000
   - Marketplace: http://localhost:5000
   - Payments: http://localhost:6000
   - Analytics: http://localhost:7000
   - Recommender: http://localhost:8000
   - Avatar Seller: http://localhost:8100

Notes:
- This prototype uses placeholders and simple rule-based logic.
- For production: configure secrets via AWS Secrets Manager / GCP Secret Manager / Azure Key Vault.
- Add HTTPS, rate limiting, logging & monitoring, error handling, and real connectors (SDK/API) to marketplaces.
```
