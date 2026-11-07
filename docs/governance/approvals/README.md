# Registro de aprobaciones

> **Estado:** EN DESARROLLO — procedimiento propuesto.

## Propósito

Mantener evidencia explícita de quién aprobó qué documento, en qué versión, cuándo y bajo qué autoridad.

## Reglas

1. No inferir aprobación por silencio, publicación, commit, merge o uso de un documento.
2. Registrar aprobaciones, rechazos y aprobaciones condicionadas.
3. Identificar la versión exacta aprobada mediante ruta y commit SHA o etiqueta de versión.
4. Si el documento cambia materialmente, evaluar si requiere nueva aprobación.
5. Conservar el registro anterior cuando una aprobación sea reemplazada o revocada.
6. La aprobación técnica de un Pull Request no equivale automáticamente a aprobación institucional.

## Ubicación

Crear un archivo por aprobación con identificador `ZIVA-APR-NNN`, numeración secuencial y sin reutilización. Nombre de archivo recomendado: `ZIVA-APR-NNN-titulo.md`. Usar la plantilla `APPROVAL-TEMPLATE.md`.

## Autoridades

La matriz de personas, cargos y facultades de aprobación se define en el documento de gobierno institucional correspondiente. La aprobación debe quedar vinculada a la autoridad y al alcance que correspondan.
