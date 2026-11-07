# Política de integridad, conservación y respaldo documental

> **Estado:** EN DESARROLLO — propuesta para revisión y aprobación interna.  
> **Ámbito:** documentación, investigaciones, fuentes, evidencias, decisiones y aprobaciones de ZivaLatam.  
> **Responsable actual:** responsable general del proyecto, conforme a la matriz de gobierno aprobada en conversación; la formalización documental de esa matriz sigue pendiente.

## 1. Objetivo

Proteger la autenticidad, integridad, disponibilidad, confidencialidad y trazabilidad de los registros de ZivaLatam durante todo su ciclo de vida: creación, revisión, aprobación, actualización, archivo y eventual eliminación autorizada.

## 2. Principios obligatorios

1. **No alterar evidencia original:** conservar el original recibido o consultado cuando sea legal y técnicamente posible. Trabajar sobre copias cuando sea necesario analizar o anotar.
2. **No borrar el historial:** las correcciones se documentan mediante nuevas versiones, notas de rectificación o registros de sustitución.
3. **Identificar cada registro:** utilizar la nomenclatura documental única definida en `README.md` y mantener el identificador durante toda su vida.
4. **Conservar contexto:** registrar procedencia, autor o entidad, fecha de recepción o consulta, versión, responsable, permisos y relaciones con decisiones.
5. **Aplicar mínimo privilegio:** limitar el acceso según la sensibilidad y la función de cada persona.
6. **No confundir Git con respaldo integral:** el historial del repositorio aporta trazabilidad, pero por sí solo no constituye una estrategia de respaldo independiente ni garantiza recuperación.
7. **No declarar controles no implementados:** todo control técnico debe marcarse como pendiente hasta contar con evidencia de configuración y prueba.

## 3. Clasificación de la información

Antes de almacenar un registro, asignar una categoría:

| Categoría | Ejemplos | Tratamiento mínimo |
|---|---|---|
| Pública | Material autorizado para difusión | Puede publicarse tras aprobación correspondiente |
| Interna | Procedimientos y trabajo institucional no público | Acceso a personas autorizadas |
| Confidencial | Contratos no públicos, estrategia sensible, información comercial reservada | Acceso restringido y ubicación aprobada |
| Restringida / sensible | Datos personales, credenciales, secretos, información legalmente protegida | Evitar el repositorio ordinario; usar sistemas adecuados y acceso estrictamente limitado |

La clasificación no reemplaza las obligaciones legales aplicables ni una evaluación profesional de privacidad, seguridad o cumplimiento.

## 4. Registro de procedencia y conservación de originales

Para cada fuente o evidencia relevante registrar, como mínimo:

- Identificador documental y título.
- Autor, entidad emisora o custodio, si se conoce.
- URL, ubicación o referencia de origen.
- Fecha de publicación, cuando conste.
- Fecha de consulta, recepción o captura.
- Persona que incorporó el registro.
- Tipo de fuente y jurisdicción o ámbito.
- Afirmaciones que respalda y localizador verificable (página, sección, párrafo u otro).
- Estado de verificación y limitaciones conocidas.
- Restricciones de licencia, privacidad, confidencialidad o redistribución.

Conservar el archivo original en su formato recibido cuando exista autorización y sea apropiado. Si no puede almacenarse por derechos, privacidad, seguridad o restricciones contractuales, conservar metadatos suficientes, una referencia estable y la explicación de la limitación. No eludir controles de acceso ni reproducir material protegido sin autorización.

## 5. Integridad criptográfica

Cuando se implemente el procedimiento técnico, calcular un hash criptográfico SHA-256 para cada archivo original o evidencia digital que requiera control de integridad.

El registro del hash debe incluir:
- Identificador del archivo y nombre original.
- Algoritmo utilizado.
- Valor hash completo.
- Fecha de cálculo.
- Herramienta o método utilizado.
- Responsable del cálculo.
- Relación con la ubicación del original y sus copias.

Un hash permite detectar cambios respecto de una referencia anterior; no demuestra por sí solo quién creó el archivo, cuándo fue creado ni si su contenido es verdadero. No afirmar que existe sello de tiempo cualificado, firma electrónica o custodia inmutable sin una solución implementada y verificada.

## 6. Versiones, correcciones y documentos sustituidos

- Mantener un historial de cambios mediante commits y Pull Requests.
- Cada versión aprobada debe asociarse a su identificador, versión o commit exacto y registro de aprobación.
- Las correcciones materiales deben describir qué cambió, por qué, quién lo solicitó y quién autorizó el cambio.
- No sobrescribir silenciosamente una evidencia, una aprobación ni un documento histórico.
- Marcar documentos reemplazados como SUPERADOS e indicar el documento sucesor.
- Marcar documentos retirados sin reemplazo como ARCHIVADOS, conservando su historial y motivo.
- Si un cambio afecta el alcance de una aprobación, solicitar una nueva aprobación antes de tratar la nueva versión como vigente.

## 7. Respaldo y recuperación

La estrategia de respaldo deberá ser independiente del repositorio principal y contemplar:

1. Copias periódicas del contenido y del historial necesario.
2. Almacenamiento separado del entorno principal, con controles de acceso.
3. Protección de copias frente a borrado accidental, compromiso de credenciales o alteración no autorizada.
4. Registro de fecha, alcance, responsable y resultado de cada respaldo.
5. Pruebas periódicas de restauración, documentando resultado, incidencias y acciones correctivas.
6. Definición posterior de frecuencia, retención, RPO y RTO según criticidad y capacidad operativa.

**Estado actual:** la frecuencia de respaldo, el proveedor, la ubicación independiente, la retención y las pruebas de restauración no están definidos ni verificados por esta política. No se afirmará que hay respaldos operativos hasta que se configure y pruebe el mecanismo elegido.

## 8. Retención y eliminación autorizada

No establecer plazos universales sin evaluar el tipo de registro, jurisdicción, obligaciones legales, contratos, litigios potenciales y necesidades operativas.

Para cada clase documental se deberá definir:
- Responsable de conservación.
- Plazo o criterio de retención.
- Evento que inicia el cómputo.
- Requisitos legales o contractuales aplicables.
- Suspensión de eliminación por auditoría, investigación, litigio o requerimiento de autoridad.
- Método de eliminación segura y evidencia de su ejecución.

La eliminación requiere autorización expresa del responsable general y revisión profesional cuando existan obligaciones legales, regulatorias, laborales, contables, tributarias o de privacidad. La eliminación de una copia no debe destruir indebidamente registros sujetos a conservación obligatoria.

## 9. Incidentes de integridad o acceso

Ante pérdida, alteración no autorizada, divulgación indebida, corrupción o indisponibilidad:

1. Restringir accesos o aislar el recurso afectado cuando sea seguro hacerlo.
2. Preservar registros, evidencias y marcas de tiempo disponibles.
3. Registrar fecha de detección, alcance conocido, sistemas y documentos afectados.
4. Informar al responsable general y solicitar apoyo especializado según la naturaleza del incidente.
5. Evaluar obligaciones de notificación y respuesta con profesionales competentes.
6. Documentar recuperación, decisiones, impacto y medidas para evitar recurrencia.

No modificar ni destruir evidencias del incidente durante la investigación.

## 10. Responsabilidades

- **Responsable general de ZivaLatam:** autoriza internamente esta política, define responsables, decide accesos y autoriza disposiciones documentales, sin sustituir revisiones profesionales obligatorias.
- **Custodio documental, cuando se designe:** mantiene índices, metadatos, versiones y registros de conservación dentro del alcance delegado.
- **Profesionales competentes:** revisan las materias de su especialidad y dejan constancia de alcance, observaciones y conclusión.
- **Colaboradores autorizados:** cumplen las reglas de clasificación, acceso, conservación y reporte de incidentes.
- **Herramientas de IA:** pueden asistir en clasificación, análisis, redacción y controles propuestos; no certifican por sí mismas autenticidad, cumplimiento legal ni aprobación institucional.

Mientras no se designe un custodio adicional, el responsable general coordina la custodia documental, sin que ello implique asumir funciones profesionales especializadas.

## 11. Controles pendientes de implementación y verificación

Esta política no acredita que los siguientes controles estén activos:

- Respaldo independiente automatizado.
- Calendario y retención de copias.
- Pruebas documentadas de restauración.
- Registro automatizado de hashes SHA-256.
- Gestión formal de claves y secretos.
- Clasificación técnica y permisos por carpeta o sistema.
- Registro centralizado de incidentes.
- Calendario de retención por categoría documental.
- Archivo inmutable o almacenamiento con protección contra alteración.
- Firma electrónica o sellado de tiempo, cuando corresponda.

Cada control deberá pasar por definición, implementación, prueba y registro de evidencia antes de marcarse como VERIFICADO.

## 12. Aprobación y revisión

Esta política permanece en estado EN DESARROLLO hasta que el responsable general la apruebe expresamente y el registro correspondiente identifique la versión exacta. Las materias jurídicas, regulatorias, de privacidad, seguridad o retención legal deberán recibir revisión profesional cuando corresponda.

Revisar esta política cuando cambien las operaciones, herramientas, jurisdicciones, riesgos, obligaciones o estructura de responsabilidades de ZivaLatam.
