```markdown
# 💾 Backend: Microservices

## 🔄 Repo: landlord-backend

### ⚙️ Services
- Tenant Service
- Due Service
- Payment Service
- Expense Service

### 📊 Stack
- Node.js (Express)
- PostgreSQL / MongoDB
- Docker / Docker Compose

### 🎨 Architecture
Use Docker for service containers and a gateway (optional).
```bash
docker-compose up --build

---

# docs/api-specs.md

```markdown

# 🔢 API Specifications

### 🔹 Tenant Service
- `GET /api/tenants`
- `POST /api/tenants`

### 🔹 Due Service
- `GET /api/dues`
- `POST /api/dues`

### 🔹 Payment Service
- `POST /api/payment`
- `PATCH /api/payment/:id`

### Response Format
```json
{
  "status": "success",
  "data": {}
}

---
