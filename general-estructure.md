# Arbol documentación

```
design-software-docs/
│
├── README.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── LICENSE
│
├── .github/
│   └── workflows/
│
├── docs/
│
│   ├── 00-governance/
│   │   ├── standards.md
│   │   ├── versioning.md
│   │   └── review-process.md
│   │
│   ├── 01-product/
│   │   ├── vision.md
│   │   ├── business-objectives.md
│   │   ├── scope.md
│   │   ├── constraints.md
│   │   ├── assumptions.md
│   │   ├── roadmap.md
│   │   ├── mvp.md
│   │   ├── personas.md
│   │   └── user-journeys.md
│   │
│   ├── 02-domain/
│   │   ├── glossary.md
│   │   ├── actors.md
│   │   ├── entities.md
│   │   ├── business-rules.md
│   │   └── bounded-contexts.md
│   │
│   ├── 03-architecture/
│   │   ├── overview.md
│   │   ├── principles.md
│   │   ├── quality-attributes.md
│   │   ├── integration-strategy.md
│   │   ├── deployment-strategy.md
│   │   │
│   │   ├── c4/
│   │   ├── diagrams/
│   │   └── decisions/
│   │
│   ├── 04-data/
│   │   ├── conceptual-model.md
│   │   ├── logical-model.md
│   │   ├── relational-model.md
│   │   ├── data-dictionary.md
│   │   └── migration-strategy.md
│   │
│   ├── 05-api/
│   │   ├── standards.md
│   │   ├── authentication.md
│   │   ├── error-handling.md
│   │   ├── pagination.md
│   │   ├── versioning.md
│   │   └── contracts/
│   │
│   ├── 06-security/
│   │   ├── iam.md
│   │   ├── threat-model.md
│   │   ├── data-protection.md
│   │   ├── auditability.md
│   │   └── security-checklist.md
│   │
│   ├── 07-devops/
│   │   ├── ci-cd.md
│   │   ├── environments.md
│   │   ├── docker.md
│   │   └── deployment-checklist.md
│   │
│   ├── 08-observability/
│   │   ├── monitoring.md
│   │   ├── alerting.md
│   │   ├── tracing.md
│   │   ├── logging.md
│   │   └── dashboards.md
│   │
│   ├── 09-quality/
│   │   ├── testing-strategy.md
│   │   ├── unit-testing.md
│   │   ├── integration-testing.md
│   │   ├── e2e-testing.md
│   │   └── quality-gates.md
│   │
│   ├── 10-ux/
│   │   ├── design-system.md
│   │   ├── component-catalog.md
│   │   ├── responsive-strategy.md
│   │   ├── accessibility.md
│   │   └── wireframes.md
│   │
│   ├── 11-services/
│   │   ├── auth-service/
│   │   ├── user-service/
│   │   └── schedule-service/
│   │
│   ├── 12-operations/
│   │   ├── runbooks.md
│   │   ├── incidents.md
│   │   ├── backup-restore.md
│   │   └── support-model.md
│   │
│   ├── 13-compliance/
│   │   ├── audit-policies.md
│   │   ├── data-retention.md
│   │   └── legal-requirements.md
│   │
│   ├── 14-training/
│   │   ├── onboarding.md
│   │   ├── user-guide.md
│   │   ├── admin-guide.md
│   │   └── faq.md
│   │
│   ├── 15-references/
│   │   ├── external-links.md
│   │   ├── standards.md
│   │   └── bibliography.md
│   │
│   └── 99-archive/
│
├── templates/
├── assets/
└── tools/
```

# El por qué de la decisión 

Se recomienda fusionar `project-context` y `product-definition` porque ambos describen el producto y así se evita duplicidad. Renombrar `sena-domain` a `domain` hace la arquitectura más reutilizable e independiente de una institución. Reducir documentos de governance y tantos `README.md` ayuda a disminuir burocracia y mantenimiento innecesario. El backlog es mejor manejarlo fuera de `docs` porque cambia constantemente. Reemplazar `microservices` por `services` mejora la modularidad y organización de cada servicio. Separar `observability` de `devops` permite manejar mejor monitoreo, logs y métricas. Agregar `compliance` ayuda con auditorías y normativas, mientras que `references` centraliza estándares y documentación externa. También es importante fortalecer UX con responsive strategy y catálogo de componentes para definir mejor la experiencia del usuario. En general, simplificar la estructura hace el proyecto más mantenible, claro y escalable.
