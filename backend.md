# 💾 Backend: Microservices

## 🔄 Repo: `landlord-backend`

This is the backend powering the Landlord App. It follows a microservices architecture for better scalability and separation of concerns. Each service is independently deployable and Dockerized.

---

## ⚙️ Core Services

| Service         | Responsibility                               |
|------------------|-----------------------------------------------|
| Tenant Service   | Manage tenant creation, updates, and retrieval |
| Due Service      | Automatically generate monthly rent dues       |
| Payment Service  | Track full or partial payments from tenants    |
| Expense Service  | Record landlord or tenant-related expenses     |

---

## 🛠 Tech Stack

- **Language**: Node.js (TypeScript)
- **Framework**: Express.js
- **Database**: PostgreSQL (preferred) or MongoDB (optional)
- **Validation**: Zod or Joi
- **Containerization**: Docker & Docker Compose
- **API Gateway**: Optional (using Express Gateway or NGINX)

---

## 📦 Folder Structure

/landlord-backend
├── services/
│ ├── tenant/
│ ├── due/
│ ├── payment/
│ └── expense/
├── gateway/ # Optional API Gateway
├── shared/ # Common code (utils, db)
├── docker-compose.yml
└── README.md


---

## 🚀 Local Development

### Clone & Start Project
```bash
git clone https://github.com/yourname/landlord-backend.git
cd landlord-backend
docker-compose up --build

Default Ports
Tenant Service → http://localhost:3001
Due Service → http://localhost:3002
Payment Service → http://localhost:3003
Expense Service → http://localhost:3004


