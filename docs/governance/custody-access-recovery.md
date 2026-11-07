# Procedimiento de custodia, acceso, respaldo y recuperación

> **Estado:** APROBADO — procedimiento institucional.  
> **Documento relacionado:** Política de integridad, conservación y respaldo documental.  
> **Versión:** 0.2.0.

## 1. Propósito y reglas de uso

Convertir la política en pasos repetibles y evidenciables. Este procedimiento no declara controles técnicos activos. Cada actividad permanece PENDIENTE hasta su implementación y prueba.

Antes de incorporar información, determinar si su obtención, conservación y tratamiento son lícitos, necesarios y compatibles con derechos, licencias, contratos y restricciones. Ante duda material, detener la incorporación y solicitar evaluación competente.

## 2. Recepción e incorporación

1. Asignar ID único o vincular con uno existente.
2. Registrar procedencia, autor/remitente, entidad emisora, fechas conocidas, zona horaria, responsable y método de obtención.
3. Clasificar la información; ante duda, aplicar provisionalmente la categoría más protectora.
4. Conservar el original sin alteraciones cuando sea legal y posible; crear copia de trabajo.
5. Registrar ubicación oficial, custodio, relaciones y limitaciones.
6. Calcular SHA-256 solo cuando el control esté implementado y sea aplicable; registrar herramienta, versión, fecha y resultado.
7. Incorporar metadatos al inventario sin copiar secretos ni datos sensibles innecesarios.
8. Si no se puede conservar el original, registrar motivo y referencia verificable.

## 3. Cadena de custodia

Crear un evento por recepción, transferencia, duplicación, conversión, extracción, redacción, anotación, análisis, verificación, cambio de ubicación, restauración, archivo o eliminación relevante.

Cada evento debe incluir ID de evento y objeto, fecha/hora y zona horaria, actor, acción, motivo, origen/destino, autorización, herramienta/método, hash antes/después cuando aplique, resultado y vínculo a incidencia o expediente.

No borrar ni editar silenciosamente eventos previos. Rectificar mediante un nuevo evento que identifique el registro afectado y explique el motivo. El registro interno no debe presentarse como certificación o cadena judicial sin evaluación jurídica aplicable.

## 4. Gestión de accesos

### Alta
- Documentar identidad/entidad, función, finalidad, sistemas y documentos requeridos.
- Definir permisos mínimos, duración y fecha de revisión.
- Obtener autorización del responsable competente.
- Usar cuentas individuales y autenticación reforzada cuando esté disponible.
- Registrar concesión y evidencia.

### Modificación
- Revisar permisos ante cambios de función, proyecto, contrato o necesidad.
- Retirar permisos que dejaron de ser necesarios.
- Registrar solicitante, autorizador, ejecutor y fecha.

### Baja
- Revocar accesos oportunamente según riesgo y obligaciones.
- Recuperar activos y transferir custodia.
- Rotar secretos compartidos potencialmente expuestos.
- Confirmar devolución/eliminación de copias de terceros cuando corresponda.
- Preservar registros sujetos a retención o legal hold.
- Registrar alcance, ejecutor, fecha y verificación de cierre.

### Cuentas bajo un mismo titular
La cuenta institucional principal declarada es `ZivaLatam-Oficial`; la cuenta secundaria declarada bajo control del mismo titular es `lusdrey523`. Esta declaración no es una verificación independiente de GitHub. La cuenta secundaria podrá ejecutar operaciones previamente autorizadas si los permisos y reglas lo permiten, pero no representa una persona revisora independiente ni podrá utilizarse para simular aprobación ajena o eludir la autoaprobación. La aprobación institucional debe registrarse separadamente mediante `APR`. No compartir contraseñas, MFA, tokens ni claves.

## 5. Respaldo y restauración

Antes de seleccionar solución, documentar sistemas y datos incluidos, criticidad, frecuencia, retención, cifrado, separación, responsables, costes, dependencias, RPO/RTO propuestos y riesgos residuales. No contratar ni activar servicios sin aprobación presupuestaria.

Cada respaldo debe registrar fecha/hora, alcance, origen, destino, resultado, errores, responsable y reporte/manifiesto. Proteger copias contra modificación y borrado no autorizado.

Una prueba de restauración debe:
1. Identificar respaldo y alcance.
2. Usar entorno controlado que no sobrescriba producción.
3. Registrar inicio, fin, operador y versión de herramientas.
4. Comprobar integridad con hashes u otros controles adecuados.
5. Validar legibilidad, estructura, permisos y dependencias.
6. Comparar con RPO/RTO definidos, si existen.
7. Documentar fallos, correcciones y autorización de cierre.

La existencia de un archivo no demuestra que sea restaurable. No declarar recuperación exitosa sin prueba documentada.

## 6. Conservación extraordinaria (legal hold)

Ante requerimiento de autoridad competente, instrucción jurídica o decisión autorizada de preservar información por investigación, controversia o litigio:
- Abrir registro de conservación extraordinaria.
- Delimitar personas, sistemas, fechas, categorías y documentos.
- Identificar quién instruye y la base/alcance de la instrucción.
- Notificar a custodios y solicitar confirmación.
- Suspender los procesos de eliminación comprendidos.
- Registrar excepciones o imposibilidades y escalar de inmediato.
- Revisar alcance con asesoría competente.
- Levantar la suspensión solo mediante autorización documentada y evaluación de obligaciones vigentes.

No interpretar una solicitud informal o ambigua como instrucción legal concluyente; escalar para determinar alcance y competencia.

## 7. Incidentes

Registrar ID, detección, reportante, fecha/hora, sistemas y registros afectados, clasificación, impacto conocido, contención, evidencia preservada, escalamiento, evaluaciones profesionales, comunicaciones autorizadas, recuperación, causa confirmada (si se determina), acciones correctivas y cierre.

La comunicación externa debe estar autorizada y basarse en hechos confirmados. No publicar datos personales, credenciales ni detalles técnicos sensibles. Evaluar con profesionales las obligaciones y plazos de notificación.

## 8. Excepciones

Registrar requisito, motivo, riesgo, control compensatorio, responsable, autorizador, revisión profesional cuando corresponda, vencimiento y cierre. Si implica incumplir una obligación legal, regulatoria o contractual o un impedimento profesional, no se concede: detener la actividad y solicitar asesoría competente.

## 9. Evidencia de ejecución

La evidencia puede incluir logs exportados, reportes de respaldo, pruebas de restauración, registros de permisos, manifiestos hash, actas de revisión y registros de incidentes. Conservar fecha, responsable, alcance, resultado y ubicación autorizada. Evitar datos personales y secretos innecesarios.

## 10. Estados de implementación

Cada control o actividad se etiqueta PENDIENTE, IMPLEMENTADO, EN PRUEBA o VERIFICADO. VERIFICADO exige evidencia objetiva, fecha, alcance, responsable, resultado y revisión. Este procedimiento no demuestra por sí mismo que las actividades estén implementadas.

## 11. Revisión

Revisar ante cambios de sistemas, responsables, jurisdicciones, proveedores, riesgos o después de incidentes. Registrar versión, fecha, responsable y cambios.