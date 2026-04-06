# DevOps-training
Repositorio utilizado para ejercitar practicas y herramientas utilizadas como DevOps.

## Proposito

El proposito de este repositorio es tener un lugar donde poder practicar y experimentar con diferentes herramientas y practicas relacionadas con DevOps. 

## Herramientas 

* ☁️ **Cloud (AWS/Azure/GCP)**
* 🐳 **Docker + Kubernetes**
* ⚙️ **CI/CD**
* 🧱 **IaC (Terraform / Ansible / CloudFormation)**

---

## Roadmap DevOps

## Fase 1 — Base operativa (Linux + Git + DevOps)

Duración recomendada: **1–2 semanas**

Labs de KodeKloud:

* [Linux labs](https://kodekloud.com/free-labs/linux)
* [Git labs](https://kodekloud.com/free-labs/git)
* [DevOps basics](https://kodekloud.com/free-labs/devops)

Objetivo técnico:

✔ debugging real
✔ CLI avanzada
✔ networking básico

Cosas que se debe dominar al terminar:

* permisos
* procesos
* logs
* systemctl
* networking
* bash scripting

Mini práctica real:

```bash
script deploy.sh
```

que haga:

1. build docker image
2. push registry
3. deploy a kubernetes

Esto simula lo que luego hará el pipeline.

---

## Fase 2 — Docker profundo

Duración: **1 semana**

Labs de KodeKloud:

* [Docker](https://kodekloud.com/free-labs/docker)

Labs a completar:

* Docker images
* Docker containers
* Docker networking
* Docker volumes

Objetivo del puesto:

> "Manejo avanzado de contenedores"

Por lo tanto no alcanza con correr contenedores.

Se debe dominar:

* multi-stage builds
* optimización de imágenes
* networking
* logs
* debugging

Mini proyecto:

Crear:

```
app-demo/
 ├ Dockerfile
 ├ docker-compose.yml
 └ app
```

Con:

* backend
* database
* frontend

---

## Fase 3 — Kubernetes (la parte más importante)

Duración: **3 semanas**

Labs KodeKloud:

* Pods
* Deployments
* Services
* ConfigMaps
* Secrets
* Networking

Objetivo para la posición:

> manejo avanzado de Kubernetes

Entonces después de los labs se debe practicar:

### Nivel 1

deploy simple:

```
Deployment
Service
ConfigMap
```

### Nivel 2

agregar:

* HPA
* resource limits
* probes

### Nivel 3

simular entorno real:

```
namespace dev
namespace staging
namespace prod
```

con deploy por entorno.

---

## Fase 4 — Cloud (AWS orientado)

Duración: **2 semanas**

👉 enfoque en **AWS**.

Arquitectura típica que se debe dominar:

```
Route53
   ↓
Load Balancer
   ↓
EKS / EC2
   ↓
Containers
```

Servicios clave que se debe practicar:

* EC2
* VPC
* Security Groups
* IAM
* ECR
* EKS
* S3
* CloudWatch

Mini proyecto:

Deploy de app en:

```
ECR
↓
EKS
↓
ALB
```

---

## Fase 5 — Infrastructure as Code

Duración: **2 semanas**

Labs KodeKloud:

* [Terraform labs](https://kodekloud.com/free-labs/terraform)

Objetivo:

> Infraestructura reproducible.

Arquitectura Terraform sugerida:

```
terraform/
 ├ modules/
 │   ├ vpc
 │   ├ eks
 │   └ security
 ├ dev
 ├ staging
 └ prod
```

Cosas importantes:

* remote state
* modules
* variables
* outputs
* workspaces

Bonus:

agregar **Ansible** para configuración.

---

## Fase 6 — CI/CD

Duración: **1–2 semanas**

Labs:

* [Jenkins labs](https://kodekloud.com/free-labs/jenkins)
* [Git labs](https://kodekloud.com/free-labs/git)

👉 GitHub Actions (lo usamos mucho hoy).

Pipeline ejemplo:

```
Push code
   ↓
Run tests
   ↓
Build Docker image
   ↓
Push ECR
   ↓
Deploy Kubernetes
```

Ejemplo workflow:

```
.github/workflows/deploy.yml
```

---

## Proyecto final

Repositorio:

```
DevOps-training
```

Arquitectura:

```
Terraform → AWS infra
Docker → containers
Kubernetes → orchestration
GitHub Actions → CI/CD
```

Flujo completo:

```
git push
   ↓
pipeline
   ↓
build docker
   ↓
push ECR
   ↓
deploy EKS
```

Esto es **exactamente lo que hace falta hoy**.

---

## Roadmap total

| Semana | Tema                |
| ------ | ------------------- |
| 1      | Linux + Git         |
| 2      | DevOps basics       |
| 3      | Docker              |
| 4      | Kubernetes core     |
| 5      | Kubernetes avanzado |
| 6      | Cloud AWS           |
| 7      | Terraform           |
| 8      | CI/CD               |
| 9      | Proyecto final      |
