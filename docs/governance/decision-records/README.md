# Registro de decisiones

> **Estado:** EN DESARROLLO — procedimiento propuesto.

## Qué registrar

Usar un ADR (*Architecture Decision Record*) para decisiones relevantes, duraderas o difíciles de revertir, incluidas arquitectura, estándares, modelos de datos, seguridad, interoperabilidad, proveedores, criterios institucionales y compromisos de producto.

No todo comentario o tarea requiere un ADR. Las decisiones operativas menores pueden quedar documentadas en el Issue o Pull Request correspondiente, siempre que sean trazables y no alteren una decisión vigente.

## Convención e índice

Identificador: `ZIVA-ADR-NNN`, secuencial y no reutilizable. Nombre recomendado: `ZIVA-ADR-NNN-titulo-breve.md`.

Estados: PROPUESTO, EN REVISIÓN, APROBADO, RECHAZADO, SUPERADO y ARCHIVADO. El índice debe mostrar ID, título, estado, fecha, responsable y decisión sucesora cuando exista.

Una decisión solo pasa a APROBADO cuando la autoridad competente la confirma explícitamente y el registro de aprobación `APR` queda vinculado. El merge de un ADR no lo aprueba por sí mismo.

## Contenido mínimo

Usar la plantilla `ADR-TEMPLATE.md`. Registrar contexto, problema, alcance, alternativas reales consideradas, criterios de evaluación, evidencia, decisión, consecuencias, riesgos, costos, dependencias, reversibilidad y condiciones de revisión.

No inventar alternativas, fuentes, aprobadores ni fechas. Si no se evaluó una opción, marcarla como no evaluada.

## Revisión y cambios

Las decisiones reemplazadas no se eliminan: se marcan SUPERADAS y enlazan al ADR sucesor. Si una decisión aprobada cambia materialmente, crear una nueva versión o ADR según el impacto, conservar el historial y evaluar la necesidad de una nueva aprobación.

## Índice inicial

No existen ADR institucionales aprobados en este expediente inicial. El primer ADR se creará cuando exista una decisión concreta que registrar.