<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=220&section=header&text=MANUEL%20SOLIVEY&fontSize=50&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=BACKEND+ARCHITECT+%7C+DATA+ENGINEER&descAlignY=60&descSize=20&descColor=1D9E75" width="100%"/>

<br>

![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&pause=1500&color=1D9E75&center=true&vCenter=true&width=700&lines=Computer+Systems+Engineer;Specializing+in+High-Concurrency+APIs;Designing+Resilient+Data+Pipelines;Focus:+Scalability+|+Observability;Santo+Domingo,+Dominican+Republic+🇩🇴)

<br>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-1A1A1A?style=for-the-badge&logo=linkedin&logoColor=1D9E75)](https://www.linkedin.com/in/manuel-yeison-solivey-medrano-data/)
[![Email](https://img.shields.io/badge/Email-1A1A1A?style=for-the-badge&logo=gmail&logoColor=1D9E75)](mailto:manuelsolivey36@gmail.com)
[![GitHub followers](https://img.shields.io/github/followers/Manueldev24?style=for-the-badge&logo=github&logoColor=1D9E75&color=1A1A1A)](https://github.com/Manueldev24)

</div>

---

## 👨‍💻 Professional Profile | Executive Summary

I am a **Computer Systems Engineer** specializing in the design, implementation, and maintenance of robust backend architectures and scalable data infrastructures. My expertise bridges the gap between high-performance API development and complex large-scale data processing (ETL/ELT).

> **Engineering Philosophy:** Building asynchronous, stateless, and highly observable systems, prioritizing clean code, long-term maintainability, and data integrity under high-demand environments.

---

## 🛠️ Tech Stack | Core Competencies

<div align="center">

| Category | Technologies & Tools | Primary Focus |
| :--- | :--- | :--- |
| **Languages** | ![Python](https://img.shields.io/badge/Python_3.11+-1A1A1A?style=flat-square&logo=python&logoColor=1D9E75) ![SQL](https://img.shields.io/badge/SQL-1A1A1A?style=flat-square&logo=postgresql&logoColor=1D9E75) ![TypeScript](https://img.shields.io/badge/TypeScript-1A1A1A?style=flat-square&logo=typescript&logoColor=1D9E75) | Strong Typing, Async, Efficiency. |
| **Frameworks & ORMs** | ![FastAPI](https://img.shields.io/badge/FastAPI-1A1A1A?style=flat-square&logo=fastapi&logoColor=1D9E75) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy_2.0-1A1A1A?style=flat-square&logo=sqlalchemy&logoColor=1D9E75) ![Alembic](https://img.shields.io/badge/Alembic-1A1A1A?style=flat-square) | RESTful Design, Data Modeling, Migrations. |
| **Data & Cache** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-1A1A1A?style=flat-square&logo=postgresql&logoColor=1D9E75) ![Redis](https://img.shields.io/badge/Redis-1A1A1A?style=flat-square&logo=redis&logoColor=1D9E75) | Relational Persistence, Distributed Caching. |
| **DevOps & Infra** | ![Docker](https://img.shields.io/badge/Docker-1A1A1A?style=flat-square&logo=docker&logoColor=1D9E75) ![GitHub Actions](https://img.shields.io/badge/CI/CD-1A1A1A?style=flat-square&logo=githubactions&logoColor=1D9E75) ![Linux](https://img.shields.io/badge/Linux-1A1A1A?style=flat-square&logo=linux&logoColor=1D9E75) | Containerization, Automated Pipelines. |
| **Data Engineering** | ![Pandas](https://img.shields.io/badge/Pandas-1A1A1A?style=flat-square&logo=pandas&logoColor=1D9E75) ![PySpark](https://img.shields.io/badge/PySpark-1A1A1A?style=flat-square&logo=apachespark&logoColor=1D9E75) | Data Wrangling, Distributed Processing. |

</div>

---

## 🏗️ Architectural Principles

I apply modern design patterns to ensure system resilience, elasticity, and decoupling:

- **Domain-Driven Design (DDD):** Software modeling centered on core business logic.
- **Hexagonal Architecture (Ports & Adapters):** Strict isolation of business logic from frameworks and external infrastructure.
- **Concurrent Programming:** Intensive use of `asyncio` and event-driven architectures to optimize I/O.
- **12-Factor Apps:** Rigorous standards for developing cloud-native SaaS applications.

---

## 📐 System Design Showcase: Auth & Data Pipeline

High-level visualization of the reference architecture implemented in my microservices deployments, prioritizing separation of concerns, Zero-Trust security, and high availability.

```mermaid
flowchart LR
    Client([Client / Frontend]) -->|HTTPS/REST| API[FastAPI Gateway]
    API -->|Validate/RateLimit| Cache[(Redis Cluster)]
    API -->|Read/Write Async| DB[(PostgreSQL Core DB)]
    
    subgraph "Data & Analytics Pipeline"
        direction TB
        DB -.->|CDC / Extraction| Worker[Python Celery Worker]
        Worker -->|Transform & Batch| Warehouse[(Data Warehouse / BI)]
    end
    
    %% Node Styles
    linkStyle default stroke:#888,stroke-width:1px;
    
    style API fill:#1A1A1A,stroke:#1D9E75,stroke-width:2px,color:#fff
    style Cache fill:#1A1A1A,stroke:#1D9E75,stroke-width:2px,color:#fff
    style DB fill:#1A1A1A,stroke:#1D9E75,stroke-width:2px,color:#fff
    style Worker fill:#333,stroke:#888,stroke-width:1px,color:#fff
    style Warehouse fill:#333,stroke:#888,stroke-width:1px,color:#fff
    style Client fill:#333,stroke:#888,stroke-width:1px,color:#fff
