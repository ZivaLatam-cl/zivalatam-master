# Procedimiento de custodia, acceso, respaldo y recuperación

> **Estado:** EN DESARROLLO — documento complementario propuesto.  
> **Documento relacionado:** Política de integridad, conservación y respaldo documental.  
> **Versión:** 0.1.0.

## 1. Propósito

Convertir los principios de la política en pasos repetibles y evidenciables. Este procedimiento no declara controles técnicos activos: cada actividad debe marcarse como PENDIENTE hasta su implementación y prueba.

## 2. Recepción e incorporación de una fuente o evidencia

1. Confirmar que la obtención y conservación son lícitas y compatibles con derechos, licencias y restricciones.
2. Asignar identificador documental único o vincularlo con uno existente.
3. Registrar procedencia, remitente/autor, fecha de publicación conocida, fecha y hora de recepción/consulta, responsable de incorporación y método.
4. Clasificar la información; ante duda, aplicar provisionalmente la categoría más protectora.
5. Conservar el original sin alteraciones cuando sea posible y crear una copia de trabajo.
6. Registrar ubicación oficial, custodio, relaciones con investigaciones o decisiones y limitaciones conocidas.
7. Calcular hash SHA-256 cuando el control técnico esté implementado y sea aplicable. Registrar resultado y herramienta.
8. Incorporar el registro al inventario maestro sin copiar secretos ni datos sensibles innecesarios.

## 3. Registro de cadena de custodia

Crear un evento por cada recepción, transferencia, duplicación, conversión, anotación, análisis, verificación, cambio de ubicación, restauración o eliminación relevante. Cada evento incluirá: ID de evento, ID del objeto, fecha/hora y zona horaria, actor, acción, motivo, origen, destino, autorización, herramienta/método, hash antes/después cuando aplique, resultado y enlace a incidencia o expediente.

No borrar ni editar silenciosamente eventos ya registrados. Rectificar mediante un evento adicional que identifique el registro rectificado y explique el motivo.

## 4. Gestión de accesos

### Alta
- Documentar identidad/entidad, función, finalidad, sistemas y documentos requeridos.
- Definir permisos mínimos, duración y fecha de revisión.
- Obtener autorización del responsable competente.
- Usar cuentas individuales y autenticación reforzada cuando esté disponible.
- Registrar fecha efectiva y evidencia de concesión.

### Modificación
- Revisar permisos al cambiar funciones, proyectos, contrato o necesidad.
- Retirar permisos que dejaron de ser necesarios.
- Registrar quién solicitó, autorizó y ejecutó el cambio.

### Baja
- Revocar accesos oportunamente según riesgo y obligaciones contractuales.
- Recuperar activos y transferir custodia de documentos.
- Rotar secretos compartidos que pudieran haber sido conocidos.
- Confirmar devolución o eliminación de copias bajo control del tercero cuando corresponda.
- Preservar registros sujetos a retención o conservación extraordinaria.
- Registrar fecha, alcance, ejecutor y verificación de cierre.

## 5. Respaldo y restauración

Antes de seleccionar una solución, documentar: sistemas y datos incluidos, criticidad, frecuencia, retención, cifrado, ubicación separada, responsables, costes, dependencias, RPO/RTO propuestos y riesgos residuales.

Cada ejecución de respaldo debe registrar fecha/hora, alcance, sistema origen, destino, resultado, errores, responsable y referencia al manifiesto o reporte. Las copias deben protegerse contra modificación y borrado no autorizado.

Una prueba de restauración debe:
1. Identificar el respaldo y alcance a restaurar.
2. Usar un entorno controlado que no sobrescriba producción.
3. Registrar inicio, fin, operador y versión de herramientas.
4. Comprobar integridad mediante hashes u otros controles adecuados.
5. Validar legibilidad, estructura, permisos y dependencias.
6. Comparar resultado con RPO/RTO definidos cuando existan.
7. Documentar fallos, acciones correctivas y aprobación de cierre.

No declarar recuperación exitosa si solo se verificó que existe un archivo de respaldo.

## 6. Conservación extraordinaria (legal hold)

Al recibir instrucción de autoridad competente, asesoría jurídica o decisión autorizada de preservar información por investigación, controversia o litigio:
- Abrir registro de conservación extraordinaria.
- Delimitar personas, sistemas, fechas, categorías y documentos.
- Notificar a custodios pertinentes y solicitar confirmación.
- Suspender procesos de eliminación aplicables.
- Preservar evidencia de cumplimiento y excepciones.
- Revisar alcance periódicamente con asesoría competente.
- Levantar la suspensión únicamente con autorización documentada y evaluación de obligaciones vigentes.

## 7. Incidentes

Registrar cada incidente con identificador, detección, reportante, fecha/hora, sistemas y registros afectados, clasificación, impacto conocido, medidas de contención, evidencia preservada, escalamiento, evaluaciones profesionales, comunicaciones autorizadas, recuperación, causa confirmada (si se determina), acciones correctivas y cierre.

La comunicación externa debe estar autorizada y basada en hechos confirmados. No publicar datos personales, credenciales ni detalles técnicos sensibles.

## 8. Excepciones

Registrar requisito, motivo, riesgo, control compensatorio, responsable, autorizador, revisión profesional, vencimiento y cierre. Si la excepción implica obligación legal o impedimento profesional, no se concede: se detiene la actividad afectada y se solicita asesoría competente.

## 9. Evidencias mínimas de ejecución

La evidencia puede incluir logs exportados, reportes de respaldo, resultados de restauración, registros de permisos, manifiestos hash, actas de revisión y registros de incidentes. Debe conservarse con fecha, responsable, alcance y ubicación autorizada.

## 10. Estado de implementación

Cada actividad se etiqueta PENDIENTE, IMPLEMENTADA, EN PRUEBA o VERIFICADA. VERIFICADA requiere evidencia objetiva, fecha, alcance, responsable y resultado. Este procedimiento no demuestra por sí mismo que las actividades estén implementadas.
