<div align="center">
<img src="./AWS%20banner.png" alt="Sridhar - AWS Solutions Architect" width="100%">
  
</div>

---

## 🧭 About Me

I'm **Sridhar**, an AWS-focused Cloud Engineer interested in designing and building reliable, secure, scalable, and cost-aware cloud systems.

My engineering focus is on understanding systems from the architecture level to implementation — including cloud infrastructure, backend services, containerization, infrastructure as code, observability, security, and deployment automation.

---

## ☁️ Engineering Focus

| Area | Focus |
|---|---|
| ☁️ Cloud Architecture | AWS infrastructure and cloud-native system design |
| 🏗️ Infrastructure | AWS resources, networking and infrastructure automation |
| ⚙️ DevOps | CI/CD, Docker and deployment automation |
| 🔐 Security | IAM, least privilege and secure cloud practices |
| 📊 Observability | Monitoring, health checks and operational visibility |
| 💰 Cost Optimization | Cloud cost awareness and resource efficiency |
| 🧱 Architecture | Clean Architecture and maintainable system design |

---

# 🚀 Flagship Project

## ☁️ Cloud Control Center

**AWS Infrastructure Control, Monitoring & Cloud Operations Platform**

A centralized cloud management dashboard designed to help cloud engineers and administrators monitor, analyze and interact with AWS infrastructure through a unified interface.

### Core Capabilities

- 🖥️ **Elastic Compute Control**
  - AWS EC2 resource aggregation
  - Instance monitoring and operational controls

- 💰 **Billing & Cost Guard**
  - AWS Cost Explorer integration
  - Cost visibility and analysis
  - Resource cost awareness

- 🔐 **IAM Least-Privilege Security**
  - AWS IAM integration
  - Permission-aware cloud operations
  - Secure credential and role handling

- 📊 **Service Telemetry**
  - System health indicators
  - API connectivity checks
  - AWS service connectivity monitoring

---

## 🏗️ System Architecture

```text
                    ┌─────────────────────┐
                    │   React Dashboard   │
                    │   Vite + Tailwind   │
                    └──────────┬──────────┘
                               │
                            HTTPS/REST
                               │
                    ┌──────────▼──────────┐
                    │      FastAPI        │
                    │      Backend        │
                    └──────────┬──────────┘
                               │
                    ┌──────────▼──────────┐
                    │  Clean Architecture │
                    │                     │
                    │ Handlers / Routes   │
                    │ Use Cases           │
                    │ Domain / Models     │
                    │ Repositories        │
                    └──────────┬──────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
       ┌──────▼─────┐   ┌──────▼─────┐   ┌────▼─────┐
       │   Boto3    │   │ PostgreSQL │   │ SQLAlchemy│
       │ AWS SDK    │   │ Database   │   │    ORM    │
       └──────┬─────┘   └────────────┘   └───────────┘
              │
       ┌──────▼──────────────────────────┐
       │          AWS Services            │
       │ EC2 • IAM • Cost Explorer • etc │
       └─────────────────────────────────┘
