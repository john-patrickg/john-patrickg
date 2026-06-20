<h1 align="center">Hi, I'm John Patrick G 👋</h1>

<p align="center">
  <em>Backend engineer building distributed systems in Java &amp; Python.</em><br/>
  <em>Currently an SDE-II @ COWRKS · Bengaluru, India.</em>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/john-patrick-g/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?logo=linkedin&logoColor=white&style=flat-square" alt="LinkedIn">
  </a>
  <a href="mailto:johnpatrick118j@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?logo=gmail&logoColor=white&style=flat-square" alt="Email">
  </a>
</p>

---

## About me

- 6+ years designing and scaling distributed backend systems.
- Spend most of my day in **Java (Spring Boot)** and **Python (Flask / FastAPI / Django / Falcon)**.
- Currently shipping the F&amp;B, payments, and tenant platform backends at COWRKS — serving **1,500+ orders/day for 2,000+ active users**.
- Strongest when the problem involves **performance, concurrency, caching, or messy distributed state**.
- Things I've shipped that I'm proud of:
  - Cut a high-traffic API from **2–5s → ~100ms (~95%)** via query + caching rework.
  - Killed a **concurrent duplicate-order race** with composite DB unique constraints + idempotent APIs → **0** duplicates in prod.
  - Hardened payment workflows to **0% transaction failure** across meeting-room and credit-order flows.
  - Rolled out distributed tracing (OpenTelemetry + SigNoz) → **MTTR down 40%**.

---

## 🛠 Tech I work with

**Languages** &nbsp;
![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white&style=flat-square)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white&style=flat-square)

**Backend** &nbsp;
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?logo=springboot&logoColor=white&style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white&style=flat-square)
![Flask](https://img.shields.io/badge/Flask-000000?logo=flask&logoColor=white&style=flat-square)
![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white&style=flat-square)

**Data / Cache** &nbsp;
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white&style=flat-square)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?logo=elasticsearch&logoColor=white&style=flat-square)
![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white&style=flat-square)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white&style=flat-square)

**Cloud / DevOps** &nbsp;
![AWS](https://img.shields.io/badge/AWS-232F3E?logo=amazonaws&logoColor=white&style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white&style=flat-square)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?logo=jenkins&logoColor=white&style=flat-square)
![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white&style=flat-square)

**Observability** &nbsp;
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?logo=opentelemetry&logoColor=white&style=flat-square)
![SigNoz](https://img.shields.io/badge/SigNoz-E75A24?style=flat-square)
![Graylog](https://img.shields.io/badge/Graylog-FF3633?style=flat-square)

---

## 🚧 Currently building

Two production-style projects I'm using to sharpen distributed-systems fundamentals. Each is being built step-by-step, with a learning log committed alongside the code.

### 🔒 [rcb-ticket-booking-backend](https://github.com/john-patrickg/rcb-ticket-booking-backend)

> No-duplicate order creation under concurrent requests, network retries, and double-clicks.

`Java 17` · `Spring Boot 3` · `PostgreSQL` · `Redis` · `Testcontainers`

Three-layer defense: Redis `SET NX` lock → cached idempotent response → Postgres composite unique constraint. Includes a concurrency integration test that fires 100 parallel requests with the same idempotency key and asserts exactly **1** order.

### 🚦 [distributed-rate-limiter](https://github.com/john-patrickg/distributed-rate-limiter)

> Pluggable rate limiter as FastAPI middleware — Token Bucket + Sliding Window, backed by Redis.

`Python 3.11` · `FastAPI` · `Redis` (Lua scripts, Sorted Sets) · `pytest-asyncio`

Atomic check-and-decrement via a Redis Lua script (no read-modify-write races across pods). Strategy pattern for pluggable algorithms. Load-tested with k6.

---

## 📚 Currently learning

- Kubernetes (CKAD path) — moving our services from EC2 → EKS.
- Kafka — eventual-consistency patterns, transactional outbox.
- System design: re-reading *Designing Data-Intensive Applications* + *Database Internals*.
- LeetCode — solidifying DSA patterns for interview season.

---

## 📫 How to reach me

- **LinkedIn:** [linkedin.com/in/john-patrick-g](https://www.linkedin.com/in/john-patrick-g/)
- **Email:** johnpatrick118j@gmail.com
- **Location:** Bengaluru, India
