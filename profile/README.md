
# TraceForge

**TraceForge** is a modern, self-hosted ERP-like platform designed for electronics and hardware companies to manage their component inventories, production workflows, and procurement processes — all in one place.

---

## 🚀 Features

### 📦 Component & Stock Management
- Track electronic parts with technical specs, datasheets, and compatibility.
- Define categories, manufacturers, minimum stock levels.

### 🧾 BOM (Bill of Materials) Management
- Import from design tools (KiCad, Altium - upcoming).
- Versioned, project-linked BOMs with stock usage and cost breakdown.

### 🏗️ Production & Project Tracking
- Project-based workflow tracking: Design → Prototype → Production → Testing → Delivery.
- Step-wise material usage, cost per unit, and failure tracking.

### 🔐 User Roles & Access Control
- Admin, Engineer, Purchaser, Operator.
- JWT-based authentication with refresh tokens and RBAC.

### 🧰 Tech Stack
- **Go** (Fiber) for backend
- **PostgreSQL** as the primary database
- **Redis** for caching & token/session management
- **Docker**-based deployment (self-hosted by default)
- **React + Tailwind + Shadcn UI** for frontend (coming soon)

---

## ⚙️ Architecture

```text
Frontend (React)
        ↓
    REST API (Fiber, Go)
        ↓
 Postgres DB + Redis
        ↓
   Docker / Self-hosted
```

---

## 📦 Installation

**Requirements**: Docker, Docker Compose

```bash
git clone https://github.com/your-org/traceforge.git
cd traceforge
docker-compose up --build
```

Once running, the backend will be available at `http://localhost:8080`.

---

## 📄 Roadmap

- [x] Auth module with JWT & RBAC
- [x] Component (Part) management
- [ ] BOM CRUD and CSV import
- [ ] Production flow UI
- [ ] Altium/KiCad integration
- [ ] Cloud deployment option
- [ ] Mobile-friendly frontend

---

## 📖 License

TraceForge is released under the [MIT License](LICENSE).

---

## ✨ Contribute

We welcome contributors from hardware, manufacturing, and OSS communities.
Feel free to open issues, submit pull requests, or suggest improvements.

---

## 🔗 About

TraceForge is built by hardware developers, for hardware developers.
