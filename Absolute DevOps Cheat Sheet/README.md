# 🚀 Absolute DevOps: Road to Architecture & Global Impact

Este directorio dentro de mi repositorio `DevOps-training` es una bitácora viva, una hoja de ruta técnica y un registro de estándares de ingeniería orientados a construir infraestructura de clase mundial.

## 🎯 Manifiesto de Calidad

  * **Si no está en código, no existe:** Prioridad absoluta a IaC (Terraform, Pulumi).
  * **Seguridad por defecto:** No existe el "lo arreglo después". Shift-left security en cada commit.
  * **Obsesión por la Observabilidad:** Si no se puede medir, no se puede mejorar.
  * **Diseño para el fallo:** La infraestructura debe ser resiliente y autosanable.

-----

## 🗺️ Roadmap: El Camino a la Cima (Senior & Architect)

### Fase 1: Excelencia en el Plano de Control (Actual)

  * [ ] **Dominio de Kubernetes (Nivel CKA/CKAD):** Networking profundo, Ingress Controllers, Resource Quotas y Affinity rules.
  * [ ] **GitOps Nativo:** Implementación de ArgoCD o Flux para eliminar la deriva de configuración.
  * [ ] **Secret Management:** Transición de variables de entorno a HashiCorp Vault o AWS Secrets Manager.

### Fase 2: Platform Engineering & Developer Experience (Próximo paso)

  * [ ] **Internal Developer Platforms (IDP):** Crear abstracciones para que los devs desplieguen sin tocar YAMLs complejos (Backstage.io).
  * [ ] **Service Mesh:** Gestión de tráfico complejo, mTLS y canary deployments con Istio o Linkerd.
  * [ ] **FinOps:** Análisis y optimización de costos en la nube (herramientas como Kubecost).

### Fase 3: Arquitectura y Liderazgo Global

  * [ ] **Multi-Cloud / Hybrid Strategy:** Diseñar sistemas que sobrevivan a la caída de una región entera o un proveedor.
  * [ ] **Gobernanza de Identidad (IAM):** Centralización de accesos escalables (IdP + Cloud Identity).
  * [ ] **SRE & Error Budgets:** Definir SLOs/SLIs reales que dicten el ritmo del negocio.

-----

## 🛠️ Checklist "Enterprise-Ready" (Definition of Done)

Cada vez que implemento una solución, debe pasar este filtro para ser considerada de alta calidad:

1.  **IaC:** ¿Está el estado de la infraestructura versionado y bloqueado?
2.  **Seguridad:** ¿Pasa el escaneo de vulnerabilidades (Trivy/Snyk)? ¿Usa el principio de mínimo privilegio?
3.  **Escalabilidad:** ¿Tiene definido HPA (Horizontal Pod Autoscaler) o reglas de escalado automático?
4.  **Recuperación:** ¿Existe un plan de Disaster Recovery documentado y probado?
5.  **Costo:** ¿Se han etiquetado (tags) los recursos para el seguimiento del presupuesto?

-----

## 📝 Registro de Decisiones Arquitectónicas (ADR)

*En esta sección guardo el "por qué" de mis elecciones técnicas para validar mi juicio.*

| Fecha | Decisión | Contexto | Resultado |
| :--- | :--- | :--- | :--- |
| 2024-XX | Uso de Helm vs Kustomize | Necesidad de plantillas reutilizables para múltiples entornos. | Helm adoptado por su manejo de ciclos de vida. |
| 2024-XX | Migración a GitHub Actions | Unificar el código y el CI en un solo lugar. | Reducción de latencia en pipelines en un 20%. |

-----

## 📚 Directorio de "Cheat Sheets" Rápidos

  * [Kubernetes: Comandos de debug avanzados](https://www.google.com/search?q=./k8s-debug.md)
  * [Terraform: Patrones de módulos escalables](https://www.google.com/search?q=./terraform-patterns.md)
  * [Cloud Networking: Troubleshooting de VPC Peering y DNS](https://www.google.com/search?q=./networking.md)
  * [Prometheus: Consultas QL para alertas críticas](https://www.google.com/search?q=./monitoring.md)

-----

## 🌍 Metas de Carrera

  * [ ] **Certificación Objetivo:** AWS Certified Solutions Architect - Professional.
  * [ ] **Contribución Open Source:** Realizar al menos 1 Pull Request mensual en proyectos de la CNCF.
  * [ ] **Networking:** Participar en comunidades internacionales (Meetups de Madrid, KubeCon, etc.).

-----

### ¿Cómo usar este repo para aprender?

Cuando aprendo una tecnología nueva, no solo guardo el código. Creo un archivo en la carpeta `/labs` con el siguiente formato:

1.  **Hipótesis:** ¿Qué problema intento resolver?
2.  **Implementación:** Código y configuración.
3.  **Lecciones aprendidas:** ¿Qué rompió? ¿Qué haría distinto? (Esto construye tu "juicio" profesional).