# Registro de aprobaciones

> **Estado:** APROBADO — procedimiento de registro institucional. La plantilla asociada está aprobada para uso.

## Propósito

Mantener evidencia explícita de quién aprobó, rechazó o condicionó qué documento o decisión, en qué versión, cuándo, bajo qué autoridad y con qué alcance.

## Reglas

1. No inferir aprobación por silencio, publicación, commit, comentario, revisión técnica, merge o uso de un documento.
2. Registrar aprobación, rechazo, aprobación condicionada, suspensión o revocación.
3. Identificar la versión exacta aprobada mediante ruta y commit SHA o etiqueta inmutable.
4. Indicar alcance, exclusiones, condiciones y documentos relacionados.
5. Si el contenido cambia materialmente, evaluar y registrar si requiere una nueva aprobación.
6. Conservar el registro anterior cuando una aprobación sea reemplazada, suspendida o revocada; no sobrescribir el historial.
7. La aprobación técnica de un Pull Request no equivale automáticamente a aprobación institucional.
8. Una aprobación interna no sustituye permisos regulatorios, aceptación de terceros ni revisión profesional.
9. La persona que prepara y aprueba un documento debe declarar la acumulación de funciones; no presentarla como revisión independiente.

## Ubicación e identificadores

Crear un archivo por decisión de aprobación con ID `ZIVA-APR-NNN`, numeración secuencial y no reutilizable. Nombre recomendado: `ZIVA-APR-NNN-titulo-breve.md`. Usar `APPROVAL-TEMPLATE.md`.

Los identificadores de ejemplo no se consideran asignados. Mantener un índice que permita detectar duplicados y localizar registros anteriores.

## Autoridad y evidencia

La autoridad debe identificarse por persona u órgano, rol interno y alcance de facultades. Mientras exista un único titular responsable, su aprobación se limita al gobierno interno del proyecto y no acredita constitución societaria ni representación legal frente a terceros.

Adjuntar o enlazar evidencia de autorización explícita y registrar la versión exacta. No incluir contraseñas, códigos MFA, tokens, claves privadas ni firmas escaneadas innecesarias.

## Estados y mantenimiento

Distinguir BORRADOR, APROBADO, RECHAZADO, CONDICIONADO, SUSPENDIDO y REVOCADO. Una aprobación condicionada solo habilita aquello que esté expresamente dentro de su alcance y después de cumplir las condiciones indicadas. Revisar el índice cuando se incorpore, reemplace o revoque un registro.