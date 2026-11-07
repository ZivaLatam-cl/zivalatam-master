# Registros operativos de integridad y conservación

> **Estado:** EN DESARROLLO — plantillas propuestas, no registros de controles ya ejecutados.  
> **Uso:** crear un registro por evento o activo relevante. No incluir contraseñas, tokens, claves privadas ni datos personales innecesarios.

## 1. Inventario maestro documental

| Campo | Descripción |
|---|---|
| ID | Identificador único ZIVA-… |
| Título / tipo | Nombre y categoría del registro |
| Versión / estado | Versión y estado documental |
| Clasificación | Pública, interna, confidencial o restringida/sensible |
| Custodio | Responsable de conservación |
| Ubicación oficial | Ruta o referencia autorizada; no incluir secretos |
| Fecha de alta / revisión | Fechas de incorporación y última revisión |
| Retención | Regla, fundamento y fecha/evento de revisión |
| Relaciones | Fuentes, investigaciones, ADR, APR, REV y sucesores |
| Restricciones | Licencia, confidencialidad, privacidad o acceso |
| Verificación | Estado y evidencia asociada |

## 2. Registro de cadena de custodia

| Campo | Descripción |
|---|---|
| ID de evento | Identificador único del evento |
| ID del objeto | Documento o evidencia afectada |
| Fecha/hora | Incluye zona horaria cuando corresponda |
| Actor | Persona o sistema que ejecuta la acción |
| Acción | Recepción, copia, acceso, transferencia, transformación, verificación, archivo, eliminación |
| Motivo y autorización | Finalidad y referencia de aprobación |
| Origen / destino | Ubicaciones antes y después |
| Método / herramienta | Herramienta y versión si aplica |
| Hash | Algoritmo y valor antes/después, si está implementado |
| Resultado / incidencia | Resultado y referencia a incidente o excepción |

## 3. Registro de accesos

| Campo | Descripción |
|---|---|
| ID de solicitud | Identificador |
| Persona / entidad | Identidad y organización |
| Finalidad / función | Necesidad concreta |
| Sistema / recurso | Alcance solicitado |
| Permisos | Lectura, escritura, administración u otro |
| Autorizador | Responsable que aprueba |
| Vigencia | Inicio, expiración y revisión |
| Ejecutor | Quién concedió, modificó o revocó |
| Evidencia | Referencia al log o confirmación |
| Estado | Solicitado, concedido, modificado, revocado, vencido |

## 4. Registro de respaldos y restauraciones

| Campo | Descripción |
|---|---|
| ID de operación | Identificador único |
| Tipo | Respaldo o restauración |
| Fecha/hora | Inicio y fin |
| Alcance | Sistemas, repositorios y datos incluidos |
| Origen / destino | Ubicaciones autorizadas |
| Responsable | Operador |
| Resultado | Correcto, parcial, fallido |
| Integridad | Hash u otra validación |
| RPO / RTO | Objetivos y resultado medido, cuando estén definidos |
| Incidencias | Errores y acciones correctivas |
| Evidencia | Reporte, log o acta |

## 5. Registro de conservación extraordinaria

| Campo | Descripción |
|---|---|
| ID | Identificador |
| Motivo / autoridad | Causa y fuente de instrucción |
| Alcance | Personas, sistemas, fechas y categorías |
| Fecha de inicio | Inicio de suspensión de eliminación |
| Custodios notificados | Personas y confirmaciones |
| Excepciones | Imposibilidad o incidencia documentada |
| Revisiones | Fechas y asesoría recibida |
| Levantamiento | Autoridad, fecha y fundamento |
| Evidencia | Ubicación del expediente |

## 6. Registro de incidentes

| Campo | Descripción |
|---|---|
| ID | Identificador |
| Detección | Fecha/hora y reportante |
| Tipo / clasificación | Integridad, confidencialidad, disponibilidad, acceso |
| Alcance | Sistemas y registros afectados |
| Contención | Medidas y responsables |
| Evidencia | Elementos preservados y ubicación |
| Escalamiento | Responsable y profesionales consultados |
| Notificación | Evaluación y decisión autorizada |
| Recuperación | Acciones y pruebas |
| Cierre | Conclusión, acciones correctivas y aprobador |

## 7. Registro de excepciones

| Campo | Descripción |
|---|---|
| ID | Identificador |
| Requisito | Regla afectada |
| Motivo | Razón de la desviación |
| Riesgo | Impacto y probabilidad evaluados |
| Control compensatorio | Medida alternativa |
| Autorizador / revisión | Aprobación y opinión profesional cuando aplique |
| Vigencia | Inicio y vencimiento |
| Condición de cierre | Evidencia requerida |
| Estado | Propuesta, autorizada, vencida, cerrada, rechazada |

## 8. Reglas de uso

- Las tablas anteriores son esquemas de campos; no deben interpretarse como registros ya completados.
- Los registros deben tener identificadores únicos y conservar historial de rectificaciones.
- Restringir el acceso conforme a la clasificación.
- No almacenar secretos ni credenciales en estos registros.
- Vincular cada registro con evidencia objetiva y ubicación autorizada.
- La ausencia de un registro no debe suplirse con una afirmación retrospectiva no verificable.
