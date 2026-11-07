# Registros operativos de integridad y conservación

> **Estado:** EN DESARROLLO — plantillas propuestas; no son registros de controles ya ejecutados.  
> **Uso:** crear un registro por evento o activo relevante. No incluir contraseñas, tokens, claves privadas ni datos personales innecesarios.

## Reglas generales

- Asignar ID único, secuencial y no reutilizable dentro de cada serie de registros.
- Registrar fechas con zona horaria cuando sea relevante.
- Identificar responsable, fuente, alcance, estado y ubicación autorizada.
- Conservar historial de rectificaciones; no sobrescribir eventos anteriores.
- Restringir acceso según clasificación.
- Vincular los registros con evidencia objetiva; no sustituir la falta de evidencia con afirmaciones retrospectivas.
- Estas plantillas no demuestran que el control exista o haya sido ejecutado.

## 1. Inventario maestro documental

| Campo | Descripción |
|---|---|
| ID | Identificador único ZIVA-… |
| Título / tipo | Nombre y categoría |
| Versión / estado | Versión y estado documental |
| Clasificación | Pública, interna, confidencial o restringida/sensible |
| Custodio | Responsable de conservación |
| Ubicación oficial | Ruta o referencia autorizada; nunca secretos |
| Alta / revisión | Fechas |
| Retención | Regla, fundamento, evento inicial y revisión |
| Relaciones | Fuentes, investigaciones, ADR, APR, REV y sucesores |
| Restricciones | Licencia, confidencialidad, privacidad o acceso |
| Verificación | Estado y evidencia asociada |

## 2. Cadena de custodia

| Campo | Descripción |
|---|---|
| ID de evento / objeto | Identificador único del evento y objeto |
| Fecha/hora | Incluye zona horaria |
| Actor | Persona o sistema |
| Acción | Recepción, copia, acceso, transferencia, transformación, verificación, archivo o eliminación |
| Motivo / autorización | Finalidad y referencia |
| Origen / destino | Ubicaciones antes y después |
| Método / herramienta | Herramienta, versión y parámetros si aplica |
| Hash | Algoritmo y valor antes/después, si está implementado |
| Resultado / incidencia | Resultado y referencia |

## 3. Accesos

| Campo | Descripción |
|---|---|
| ID de solicitud | Identificador |
| Persona / entidad | Identidad y organización |
| Finalidad / función | Necesidad concreta |
| Sistema / recurso | Alcance |
| Permisos | Lectura, escritura, administración u otro |
| Autorizador | Responsable que aprueba |
| Vigencia | Inicio, expiración y revisión |
| Ejecutor | Quién concede, modifica o revoca |
| Evidencia | Log o confirmación |
| Estado | Solicitado, concedido, modificado, revocado o vencido |

## 4. Respaldos y restauraciones

| Campo | Descripción |
|---|---|
| ID de operación | Identificador |
| Tipo | Respaldo o restauración |
| Fecha/hora | Inicio y fin, zona horaria |
| Alcance | Sistemas, repositorios y datos |
| Origen / destino | Ubicaciones |
| Responsable | Operador |
| Resultado | Correcto, parcial o fallido |
| Integridad | Hash u otra validación |
| RPO / RTO | Objetivos y resultado medido, cuando existan |
| Incidencias | Errores y correcciones |
| Evidencia | Reporte, log o acta |

## 5. Conservación extraordinaria

| Campo | Descripción |
|---|---|
| ID | Identificador |
| Motivo / autoridad | Causa e instrucción |
| Fundamento / alcance | Base, sistemas, personas, fechas y categorías |
| Inicio | Fecha/hora de suspensión |
| Custodios notificados | Personas y confirmaciones |
| Excepciones | Imposibilidades e incidencias |
| Revisiones | Fechas y asesoría recibida |
| Levantamiento | Autoridad, fecha y fundamento |
| Evidencia | Ubicación del expediente |

## 6. Incidentes

| Campo | Descripción |
|---|---|
| ID | Identificador |
| Detección | Fecha/hora y reportante |
| Tipo / clasificación | Integridad, confidencialidad, disponibilidad o acceso |
| Alcance | Sistemas y registros afectados |
| Contención | Medidas y responsables |
| Evidencia | Elementos preservados y ubicación |
| Escalamiento | Responsable y profesionales consultados |
| Notificación | Evaluación y decisión autorizada |
| Recuperación | Acciones y pruebas |
| Cierre | Conclusión, acciones correctivas y aprobador |

## 7. Excepciones

| Campo | Descripción |
|---|---|
| ID | Identificador |
| Requisito | Regla afectada |
| Motivo | Razón |
| Riesgo | Impacto y probabilidad evaluados |
| Control compensatorio | Medida alternativa |
| Autorizador / revisión | Aprobación y opinión profesional cuando aplique |
| Vigencia | Inicio y vencimiento |
| Condición de cierre | Evidencia requerida |
| Estado | Propuesta, autorizada, vencida, cerrada o rechazada |

## 8. Revisión periódica del inventario

| Campo | Descripción |
|---|---|
| Fecha / responsable | Quién y cuándo revisa |
| Alcance | Categorías y ubicaciones revisadas |
| Registros sin custodio | ID y acción correctiva |
| Enlaces / ubicaciones rotas | ID y corrección |
| Retención pendiente | ID, motivo y responsable |
| Clasificación dudosa | ID y evaluación requerida |
| Resultado | Hallazgos y acciones |
| Evidencia | Acta, log o referencia |

## 9. Uso y conservación

Las tablas son esquemas de campos, no registros completados. Mantener historial de rectificaciones, acceso restringido y vínculos a evidencia objetiva. La ausencia de un registro no debe suplirse con una afirmación retrospectiva no verificable.