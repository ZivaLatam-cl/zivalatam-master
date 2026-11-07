# ZivaLatam — Repositorio institucional maestro

Este repositorio es el punto central de documentación y trazabilidad institucional de **ZivaLatam**. Su finalidad es organizar, conservar y controlar la documentación que sustenta la visión, el gobierno, las decisiones, las políticas, los estándares y la coordinación del ecosistema.

> **Estado del repositorio:** base documental institucional inicial. La existencia de documentos aprobados no significa que los sistemas, servicios, controles o capacidades descritos estén implementados ni operativos.

## 1. Propósito

El repositorio `zivalatam-master` sirve para:

- Mantener una fuente institucional controlada de documentación.
- Registrar políticas, procedimientos, decisiones y aprobaciones.
- Organizar investigaciones, fuentes, evidencias y resultados.
- Documentar la arquitectura organizativa y tecnológica a medida que se definan y aprueben.
- Mantener trazabilidad de cambios, responsables, revisiones y versiones.
- Coordinar el desarrollo futuro del ecosistema ZivaLatam sin confundir propuestas con capacidades existentes.

## 2. Alcance actual

La estructura incorporada actualmente establece la base de gobierno documental, revisión y aprobación, trazabilidad, integridad, conservación, custodia y recuperación de información.

El repositorio podrá ampliarse mediante Pull Requests para incorporar áreas institucionales, investigaciones, arquitectura, productos, tecnología, operaciones, cumplimiento y otras materias que se aprueben formalmente. La inclusión de una carpeta, nombre o documento futuro no debe interpretarse como evidencia de que exista una unidad operativa o un servicio productivo.

## 3. Estructura del repositorio

```text
zivalatam-master/
├── .github/
│   └── pull_request_template.md
├── docs/
│   └── governance/
│       ├── README.md
│       ├── commit-conventions.md
│       ├── review-and-approval.md
│       ├── traceability-model.md
│       ├── integrity-retention.md
│       ├── custody-access-recovery.md
│       ├── integrity-registers.md
│       ├── decision-records/
│       │   ├── README.md
│       │   └── ADR-TEMPLATE.md
│       └── approvals/
│           ├── README.md
│           ├── APPROVAL-TEMPLATE.md
│           ├── ZIVA-APR-001-governance-framework.md
│           └── ZIVA-APR-002-integrity-retention.md
└── README.md
```

Esta representación describe la estructura documental incorporada en esta etapa. No anticipa directorios o componentes que todavía no hayan sido creados y aprobados.

## 4. Áreas documentales

| Área | Función |
|---|---|
| Gobierno documental | Reglas para crear, revisar, aprobar, publicar y mantener documentos |
| Trazabilidad | Relación entre necesidades, investigaciones, fuentes, evidencias, decisiones, aprobaciones y versiones |
| Integridad y conservación | Requisitos y procedimientos para custodia, acceso, respaldo, recuperación y conservación |
| Registro de decisiones | Documentación de decisiones institucionales y técnico-arquitectónicas mediante ADR |
| Registro de aprobaciones | Evidencia de aprobaciones, rechazos, condiciones, suspensiones y revocaciones mediante APR |
| Áreas futuras | Investigación, arquitectura, productos, tecnología, operaciones y cumplimiento, cuando su alcance y estructura sean definidos |

## 5. Relación entre ZivaLatam y sus iniciativas

ZivaLatam es el proyecto institucional y el marco del ecosistema. Los productos, plataformas, módulos e iniciativas asociados se documentarán bajo ese marco cuando corresponda. Su mención en documentos de planificación no implica constitución jurídica, licencia, disponibilidad comercial, implementación técnica ni operación productiva.

Cada iniciativa deberá tener alcance, responsable, estado, evidencia y decisiones identificables. Las relaciones entre iniciativas se documentarán sin crear estructuras organizativas ficticias ni presentar planes futuros como unidades existentes.

## 6. Gobierno del repositorio

- `main` es la rama de referencia para la documentación institucional incorporada.
- Las ramas de trabajo contienen cambios en preparación.
- Los Pull Requests documentan el propósito, alcance, evidencias, revisiones y aprobación de cada cambio.
- Los commits conservan el historial de modificaciones.
- Los registros APR vinculan una decisión de aprobación con una versión y un commit concretos.
- La integración técnica (*merge*) no sustituye una aprobación institucional ni una revisión profesional requerida.

Consulta el [marco de gobierno documental](docs/governance/README.md) para conocer las reglas completas.

## 7. Estados: aprobación e implementación

Los estados deben interpretarse por separado:

- **BORRADOR / EN REVISIÓN:** contenido en preparación o revisión.
- **APROBADO:** contenido autorizado institucionalmente dentro del alcance registrado.
- **IMPLEMENTADO:** actividad o control efectivamente puesto en funcionamiento, con evidencia.
- **VERIFICADO:** resultado comprobado mediante evidencia objetiva, fechada y atribuible.
- **SUPERADO / ARCHIVADO:** contenido reemplazado o conservado sin vigencia operativa.

La aprobación de una política o procedimiento no acredita que sus controles estén implementados. Las plantillas aprobadas son formatos de registro, no evidencia de que las actividades se hayan ejecutado.

## 8. Documentación de referencia

- [Gobierno documental](docs/governance/README.md)
- [Convenciones de commits](docs/governance/commit-conventions.md)
- [Revisión y aprobación](docs/governance/review-and-approval.md)
- [Modelo de trazabilidad](docs/governance/traceability-model.md)
- [Política de integridad, conservación y respaldo](docs/governance/integrity-retention.md)
- [Procedimiento de custodia, acceso, respaldo y recuperación](docs/governance/custody-access-recovery.md)
- [Registros operativos de integridad y conservación](docs/governance/integrity-registers.md)
- [Registro de decisiones](docs/governance/decision-records/README.md)
- [Registro de aprobaciones](docs/governance/approvals/README.md)

## 9. Límites institucionales

Este repositorio es un instrumento documental. Por sí mismo no constituye una sociedad, licencia, certificación, autorización regulatoria, sistema productivo, infraestructura desplegada, auditoría independiente ni prueba de cumplimiento. Las materias legales, regulatorias, financieras, de privacidad, ciberseguridad y otras especialidades deberán someterse a revisión profesional competente cuando corresponda.

---

**Mantenimiento:** toda modificación de este README debe presentarse mediante Pull Request y mantener consistencia con la estructura y los documentos efectivamente existentes.
