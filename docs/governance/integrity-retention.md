# Política de integridad, conservación y respaldo documental

> **Estado:** EN DESARROLLO — propuesta para revisión y aprobación interna.  
> **Ámbito:** documentación, investigaciones, fuentes, evidencias, decisiones, aprobaciones, revisiones y registros bajo control de ZivaLatam.  
> **Versión:** 0.3.0 — revisión de controles y límites.

## 1. Objetivo

Establecer requisitos para proteger la integridad, disponibilidad, confidencialidad y trazabilidad de los registros durante su ciclo de vida. Debe poder reconstruirse qué se conserva, de dónde provino, quién lo incorporó, qué transformaciones experimentó, quién accedió y bajo qué autorización se modificó, trasladó, archivó o eliminó.

Esta política define requisitos; los procedimientos y registros asociados describen su ejecución. La política no demuestra que los controles estén implementados.

## 2. Alcance y límites

Aplica a documentos institucionales, investigaciones, fuentes, evidencias digitales y físicas, decisiones, aprobaciones, revisiones profesionales, contratos, registros operativos y respaldos bajo control del proyecto, cualquiera sea el sistema autorizado donde se encuentren.

No sustituye obligaciones legales, regulatorias o contractuales, ni el criterio de profesionales competentes en privacidad, ciberseguridad, auditoría, contabilidad o conservación. No acredita licencia, certificación, personalidad jurídica, operación comercial ni capacidad técnica.

## 3. Principios

1. Preservar el original cuando sea lícito y técnicamente posible; analizar sobre copias.
2. Registrar eventos relevantes de custodia y transformación.
3. No sobrescribir silenciosamente documentos, evidencias ni registros históricos.
4. Asignar identificadores únicos y no reutilizables.
5. Conservar procedencia, fechas, responsables, clasificación, permisos, versiones y restricciones.
6. Aplicar mínimo privilegio y necesidad de conocer.
7. Declarar limitaciones de segregación cuando una sola persona concentre funciones; no simular independencia.
8. Mantener respaldos independientes del repositorio principal y probar restauraciones.
9. No declarar controles activos o VERIFICADOS sin evidencia objetiva, fechada y atribuible.
10. Comunicar con precisión el estado real de los controles, protegiendo información sensible.

## 4. Clasificación

| Categoría | Ejemplos | Tratamiento mínimo |
|---|---|---|
| Pública | Material autorizado para difusión | Revisar exactitud, derechos y autorización de publicación |
| Interna | Procedimientos y trabajo no público | Acceso a personas autorizadas |
| Confidencial | Contratos, estrategia o información comercial reservada | Acceso restringido y almacenamiento aprobado |
| Restringida/sensible | Datos personales, credenciales, secretos o información legalmente protegida | Evitar repositorios ordinarios; controles reforzados y revisión especializada |

Clasificar según contenido, contexto, impacto, obligaciones y derechos de terceros. Ante duda, aplicar provisionalmente la categoría más protectora. La clasificación no reemplaza una evaluación legal o de privacidad.

## 5. Procedencia y originales

Para cada fuente o evidencia relevante registrar:

- ID, título, tipo, descripción y autor/entidad emisora, si se conoce.
- URL, ubicación o referencia de origen.
- Fecha de publicación o actualización, si consta; fecha y hora de consulta, recepción o captura, con zona horaria cuando sea relevante.
- Persona que incorporó el registro y método de obtención.
- Jurisdicción, idioma y versión.
- Afirmaciones respaldadas y localizador verificable.
- Estado de verificación, limitaciones e incertidumbres.
- Derechos, licencia, confidencialidad, privacidad y restricciones.
- Ubicación del original y copias autorizadas.

Conservar el original en su formato recibido cuando exista autorización y sea apropiado. Si no puede almacenarse por derechos, privacidad, seguridad o contrato, conservar metadatos suficientes, referencia estable y motivo de la limitación. No eludir controles de acceso ni reproducir material protegido sin autorización.

## 6. Cadena de custodia y transformaciones

Para evidencia cuyo valor dependa de su integridad, registrar cada evento significativo: recepción, captura, descarga, transferencia, duplicación, conversión, extracción, redacción, anotación, análisis, hash, cambio de ubicación, acceso excepcional, restauración, archivo y eliminación.

Cada evento debe identificar objeto, fecha/hora y zona horaria, actor, acción, origen/destino, motivo, autorización, método/herramienta, resultado y referencia al expediente.

- Mantener original separado de copias de trabajo cuando sea viable.
- Identificar cada copia y su relación con el original.
- Documentar herramientas, versiones, parámetros y limitaciones de transformaciones relevantes.
- No presentar una copia transformada como original.
- Ante alteración no explicada, preservar el estado encontrado, registrar incidencia y suspender el uso como evidencia confiable hasta evaluación.
- Rectificar registros mediante un nuevo evento, sin borrar el anterior.

Un registro interno mejora la trazabilidad, pero no equivale automáticamente a cadena de custodia judicial, certificación notarial ni prueba de admisibilidad. La suficiencia jurídica depende de la jurisdicción y el uso, y requiere evaluación profesional.

## 7. Integridad criptográfica y tiempo

Cuando el control técnico esté implementado, calcular SHA-256 para archivos originales o evidencias digitales que requieran control de integridad. Registrar ID, nombre, tamaño, algoritmo, valor completo, fecha/hora, zona horaria, herramienta/versión, responsable, ubicación y relación con copias.

Verificar el hash al recibir, transferir, restaurar o utilizar evidencia crítica, según procedimiento. Proteger los manifiestos de hashes de alteración y conservarlos separados del objeto cuando sea viable.

Un hash permite detectar diferencias respecto de una referencia; por sí solo no demuestra autoría, origen, fecha cierta, veracidad, legitimidad ni custodia continua. La fecha de un registro del sistema tampoco equivale necesariamente a un sello de tiempo confiable. No afirmar firma electrónica, sello de tiempo cualificado, archivo inmutable o certificación sin solución implementada, evaluada y verificada.

## 8. Inventario maestro

Mantener índice de documentos, fuentes y evidencias relevantes con ID, título, tipo, clasificación, estado, versión, custodio, ubicación autorizada, alta, retención, relaciones, restricciones y última revisión. No replicar contenido sensible ni secretos. Para información restringida, conservar solo metadatos y referencia a un sistema seguro cuando corresponda.

## 9. Versiones y correcciones

- Mantener historial mediante commits y Pull Requests.
- Asociar cada versión aprobada con ID, versión, commit SHA o referencia inmutable y registro APR.
- Describir qué cambió, por qué, quién lo solicitó y quién autorizó cambios materiales.
- Marcar reemplazados como SUPERADOS e indicar sucesor; retirar sin reemplazo como ARCHIVADOS.
- Si un cambio afecta alcance, obligaciones, riesgos o conclusiones, evaluar nueva aprobación.
- Preservar versiones anteriores y emitir rectificación proporcional al impacto.

## 10. Accesos y ciclo de vida de cuentas

Todo acceso debe tener finalidad, autorizador, alcance, sistema, nivel de permiso, duración y fecha de revisión. Revisar ante cambios de función, incidentes o salida de personas.

Al finalizar una relación o cambiar responsabilidades, revocar accesos innecesarios, recuperar activos, transferir custodia, rotar secretos compartidos que pudieran haberse expuesto y conservar evidencia de baja. Usar cuentas individuales y autenticación reforzada cuando esté disponible. Nunca publicar credenciales en el repositorio.

Los accesos de proveedores y profesionales deben limitarse por contrato, función, duración y necesidad. Definir confidencialidad, devolución y eliminación con asesoría competente cuando corresponda.

## 11. Respaldo, continuidad y recuperación

La estrategia debe ser independiente del repositorio principal y considerar:

1. Copias periódicas de contenido, metadatos, historial y configuraciones necesarias.
2. Separación lógica y, cuando sea viable, física o administrativa.
3. Protección contra borrado accidental, compromiso de credenciales, ransomware y alteración.
4. Cifrado en tránsito y reposo cuando corresponda, con gestión separada de claves.
5. Registro de fecha, alcance, responsable, ubicación, resultado y errores.
6. Pruebas documentadas de restauración, integridad y accesibilidad.
7. Priorización de servicios y registros críticos.
8. RPO, RTO, frecuencia y retención definidos según criticidad, obligaciones, presupuesto y capacidad.

**Estado actual:** proveedor, ubicación independiente, calendario, retención, RPO/RTO y pruebas de restauración no están definidos ni verificados por esta política. No afirmar que existen respaldos operativos hasta configurar y probar el mecanismo.

## 12. Retención, legal hold y eliminación

No fijar plazos universales sin evaluar tipo de registro, jurisdicción, obligaciones, contratos, controversias y necesidad operativa. Para cada clase definir responsable, plazo o criterio, evento inicial, fundamento, suspensión, método de eliminación y evidencia.

Ante requerimiento de autoridad, litigio real o razonablemente previsible, auditoría, investigación o instrucción jurídica competente, evaluar y activar una conservación extraordinaria (*legal hold*) con alcance delimitado. Registrar autoridad/instrucción, motivo, fecha, sistemas, custodios, notificaciones, confirmaciones, revisiones y liberación formal. No suspender ni reanudar eliminación por una instrucción ambigua: escalar para determinar alcance y competencia.

La eliminación requiere autorización expresa del responsable interno y revisión profesional cuando existan obligaciones legales, regulatorias, laborales, contables, tributarias o de privacidad. Documentar qué, por qué, cuándo, método, ejecutor y autorizador. No destruir registros sujetos a conservación obligatoria. Tratar copias residuales en respaldos conforme al ciclo técnico y obligaciones aplicables.

## 13. Incidentes

Ante pérdida, alteración, divulgación indebida, corrupción, acceso no autorizado o indisponibilidad:

1. Contener sin destruir evidencia ni agravar el impacto.
2. Preservar archivos, logs, bitácoras y marcas de tiempo disponibles.
3. Registrar detección, alcance conocido, sistemas y registros afectados.
4. Informar al responsable general y escalar a especialistas según naturaleza.
5. Evaluar con profesionales las obligaciones de notificación, plazos y comunicaciones.
6. Recuperar desde fuentes verificadas y documentar pruebas.
7. Registrar impacto, decisiones, acciones correctivas y lecciones.

No atribuir públicamente causas ni responsabilidades sin evidencia suficiente. No alterar ni destruir evidencia del incidente.

## 14. Excepciones

Toda desviación temporal requiere requisito afectado, motivo, alcance, riesgo, controles compensatorios, responsable, autorización, revisión profesional cuando corresponda, vencimiento y condición de cierre. Una excepción no dispensa obligaciones legales, regulatorias o contractuales ni impedimentos profesionales. Si el riesgo no puede aceptarse o mitigarse, detener la actividad afectada.

## 15. Responsabilidades y segregación

- **Responsable general:** aprobación interna y decisiones dentro de sus facultades; no sustituye profesionales ni autoridades.
- **Custodio documental:** inventario, metadatos, custodia y registros delegados.
- **Responsable técnico:** implementación, prueba y evidencia de controles cuando sea designado.
- **Profesionales competentes:** revisión dentro de su especialidad y alcance.
- **Colaboradores:** cumplimiento y reporte.
- **IA:** apoyo analítico y documental; no certifica autenticidad, cumplimiento, revisión profesional ni aprobación institucional.

Mientras una persona concentre funciones, declararlo y aplicar controles compensatorios viables. Dos cuentas controladas por la misma persona no constituyen dos personas ni revisión independiente. Los detalles de las cuentas y límites operativos se mantienen en el procedimiento de revisión y aprobación.

## 16. Transparencia y divulgación

Toda comunicación a inversores, clientes o usuarios debe distinguir capacidades existentes y verificadas, controles en implementación, planes y objetivos. Antes de divulgar, revisar exactitud, vigencia, derechos, privacidad, confidencialidad, seguridad y autorización. No divulgar datos personales, secretos, vulnerabilidades explotables, credenciales ni documentos de terceros sin base legítima.

## 17. Controles pendientes

Esta política no acredita que estén activos respaldos independientes, calendario y retención, restauraciones probadas, hashes automatizados, inventario maestro operativo, cadena de custodia, gestión formal de secretos, permisos granulares, revisión periódica de accesos, registro centralizado de incidentes, legal hold, archivo inmutable, firma/sello de tiempo ni continuidad.

Cada control requiere definición, responsable, implementación, prueba, evidencia fechada, revisión y estado. Solo entonces podrá marcarse VERIFICADO.

## 18. Revisión y aprobación

Esta política permanece EN DESARROLLO hasta aprobación expresa y registro de la versión exacta. Las materias jurídicas, regulatorias, privacidad, ciberseguridad y retención legal requieren revisión profesional cuando corresponda. Revisar ante cambios materiales, incidentes relevantes o cambios de jurisdicción, sistemas y riesgos.