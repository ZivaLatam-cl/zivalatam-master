# Política de integridad, conservación y respaldo documental

> **Estado:** EN DESARROLLO — propuesta para revisión y aprobación interna.  
> **Ámbito:** documentación, investigaciones, fuentes, evidencias, decisiones, aprobaciones y registros de ZivaLatam.  
> **Responsable actual:** responsable general del proyecto, conforme a decisiones internas expresadas; su consolidación documental sigue pendiente.  
> **Versión:** 0.2.0 — propuesta ampliada.

## 1. Objetivo y resultado esperado

Proteger la autenticidad, integridad, disponibilidad, confidencialidad y trazabilidad de los registros de ZivaLatam durante todo su ciclo de vida. La organización deberá poder reconstruir qué información conserva, de dónde provino, quién la incorporó, qué transformaciones experimentó, quién accedió a ella, qué decisiones sustentó y bajo qué autorización se modificó, trasladó, archivó o eliminó.

Esta política establece obligaciones y principios. Los procedimientos y registros asociados describen cómo ejecutarlos y cómo demostrar su cumplimiento.

## 2. Alcance y límites

Aplica a documentos institucionales, investigaciones, fuentes, evidencias digitales y físicas, decisiones, aprobaciones, revisiones profesionales, contratos, registros operativos y copias de respaldo bajo control de ZivaLatam, cualquiera sea el sistema autorizado donde se encuentren.

No sustituye obligaciones legales, regulatorias, contractuales ni criterios profesionales de privacidad, ciberseguridad, auditoría, contabilidad o conservación. Tampoco acredita por sí misma que una licencia, certificación, control técnico o capacidad operativa exista.

## 3. Principios obligatorios

1. **Preservación del original:** conservar el original recibido o consultado cuando sea legal, lícito y técnicamente posible. Analizar sobre copias.
2. **Trazabilidad de custodia:** registrar eventos relevantes de recepción, acceso, transferencia, copia, transformación, verificación, archivo y eliminación.
3. **Historial íntegro:** no sobrescribir silenciosamente documentos, evidencias, aprobaciones ni registros históricos.
4. **Identificación permanente:** asignar identificadores únicos, no reutilizables, conforme al sistema documental institucional.
5. **Contexto suficiente:** conservar procedencia, fechas, responsables, clasificación, permisos, versiones, restricciones y relaciones con decisiones.
6. **Mínimo privilegio y necesidad de conocer:** conceder únicamente los accesos indispensables y por el tiempo necesario.
7. **Separación de funciones:** distinguir autoría, custodia, revisión profesional y aprobación institucional. Cuando la estructura de una sola persona impida una segregación real, declarar la limitación y establecer controles compensatorios; no simular independencia.
8. **Respaldo independiente:** el historial de Git no sustituye una estrategia de respaldo separada y probada.
9. **Evidencia de implementación:** no declarar un control como activo o VERIFICADO sin prueba suficiente, fechada y atribuible.
10. **Transparencia responsable:** comunicar con precisión el estado real de los controles, sin revelar información confidencial, datos personales, secretos ni detalles que aumenten el riesgo de seguridad.

## 4. Clasificación de la información

Toda información incorporada debe clasificarse antes de su almacenamiento o difusión.

| Categoría | Ejemplos | Tratamiento mínimo |
|---|---|---|
| Pública | Material expresamente autorizado para difusión | Revisión de exactitud, derechos y aprobación de publicación |
| Interna | Procedimientos y trabajo institucional no público | Acceso a personas autorizadas |
| Confidencial | Contratos no públicos, estrategia sensible, información comercial reservada | Acceso restringido, almacenamiento aprobado y registro de divulgación |
| Restringida / sensible | Datos personales, credenciales, secretos, información legalmente protegida | Evitar repositorios ordinarios; sistemas adecuados, controles reforzados y revisión especializada |

La clasificación debe considerar contenido, contexto, impacto de divulgación, obligaciones aplicables y derechos de terceros. Si existe duda, aplicar provisionalmente la categoría más protectora y solicitar evaluación competente. La clasificación no reemplaza una evaluación legal o de privacidad.

## 5. Registro de procedencia y conservación de originales

Para cada fuente o evidencia relevante registrar, como mínimo:

- Identificador, título, tipo y descripción.
- Autor, entidad emisora, custodio o remitente, si se conoce.
- URL, ubicación o referencia de origen.
- Fecha de publicación, si consta; fecha y hora de consulta, recepción o captura, con zona horaria cuando sea relevante.
- Persona que incorporó el registro y método de obtención.
- Jurisdicción o ámbito, idioma y versión.
- Afirmaciones que respalda y localizador verificable (página, sección, párrafo u otro).
- Estado de verificación, limitaciones, incertidumbres y posibles conflictos.
- Derechos, licencia, confidencialidad, privacidad y restricciones de redistribución.
- Ubicación del original y de las copias autorizadas.

Conservar el archivo original en su formato recibido cuando exista autorización y sea apropiado. Si no puede almacenarse por derechos, privacidad, seguridad o restricciones contractuales, conservar metadatos suficientes, referencia estable y explicación de la limitación. No eludir controles de acceso ni reproducir material protegido sin autorización.

## 6. Cadena de custodia y transformaciones

Toda evidencia cuyo valor pueda depender de su integridad debe contar con un registro de custodia. Registrar cada evento significativo con fecha y hora, actor, acción, objeto, origen y destino, motivo, autorización, resultado y referencia a la evidencia relacionada.

Se consideran eventos relevantes: recepción, captura, descarga, transferencia, duplicación, conversión de formato, extracción, redacción, anotación, análisis, cálculo de hash, cambio de ubicación, acceso excepcional, restauración, archivo y eliminación.

- Mantener el original separado de copias de trabajo cuando sea viable.
- Identificar cada copia y su relación con el original.
- Documentar herramientas, parámetros y limitaciones de las transformaciones que puedan afectar el contenido.
- No presentar una copia transformada como original.
- Si se detecta una alteración no explicada, preservar el estado encontrado, registrar la incidencia y suspender su uso como evidencia confiable hasta evaluación.
- Restringir la edición de registros de custodia; toda rectificación debe ser un nuevo evento que preserve el dato anterior y explique el motivo.

Un registro interno de custodia mejora la trazabilidad, pero no equivale automáticamente a cadena de custodia judicial, certificación notarial ni prueba de admisibilidad. La suficiencia jurídica debe evaluarse profesionalmente según jurisdicción y uso.

## 7. Integridad criptográfica

Cuando se implemente el procedimiento técnico, calcular SHA-256 para cada archivo original o evidencia digital que requiera control de integridad. Registrar identificador, nombre, tamaño, algoritmo, valor completo, fecha/hora y zona horaria, herramienta/versión, responsable, ubicación y relación con las copias.

Verificar hashes al recibir, transferir, restaurar o antes de utilizar evidencia crítica, según el procedimiento aplicable. Guardar los manifiestos de hashes separados del conjunto cuya integridad se desea proteger y restringir su modificación.

Un hash detecta diferencias respecto de una referencia; no demuestra por sí solo autoría, fecha de creación, veracidad ni legitimidad del contenido. No afirmar firma electrónica, sello de tiempo cualificado, custodia inmutable o certificación sin solución implementada y verificada.

## 8. Inventario maestro y localización

Mantener un índice maestro de documentos, fuentes y evidencias relevantes con identificador, título, tipo, clasificación, estado, versión, custodio, ubicación autorizada, fecha de alta, retención aplicable, relaciones, restricciones y fecha de última revisión.

El índice no debe replicar innecesariamente contenido sensible ni almacenar secretos. Para información restringida puede conservar solo metadatos y una referencia a un sistema seguro. Cada registro debe tener una ubicación oficial identificable y un responsable de custodia.

## 9. Versiones, correcciones y documentos sustituidos

- Mantener historial de cambios mediante commits y Pull Requests en el repositorio maestro, cuando corresponda.
- Asociar cada versión aprobada con identificador, número de versión, commit o huella exacta y registro de aprobación.
- Describir qué cambió, por qué, quién lo solicitó y quién autorizó cambios materiales.
- No sobrescribir silenciosamente evidencia, aprobación ni documento histórico.
- Marcar documentos reemplazados como SUPERADOS e indicar sucesor.
- Marcar documentos retirados sin reemplazo como ARCHIVADOS, conservando historial y motivo.
- Si un cambio afecta alcance, obligaciones, riesgos o conclusiones de una aprobación, solicitar nueva aprobación antes de tratar la nueva versión como vigente.
- Las correcciones de errores deben preservar la versión anterior y dejar una nota de rectificación proporcional a su impacto.

## 10. Accesos, altas, cambios y bajas

Todo acceso debe tener una finalidad, responsable autorizante, alcance, sistema, nivel de permiso y, cuando proceda, fecha de expiración. Revisar los permisos periódicamente y ante cambios de función, incidentes o salida de una persona.

Al finalizar una relación o cambiar responsabilidades, revocar oportunamente los accesos que ya no correspondan, recuperar activos y documentación institucional, transferir custodia, rotar credenciales compartidas si existieran y conservar evidencia de la baja. Las cuentas y secretos deben ser individuales o gestionarse mediante mecanismos seguros; nunca publicar credenciales en el repositorio.

Los accesos de proveedores y profesionales deben limitarse por contrato, función, duración y necesidad. Las obligaciones de confidencialidad, devolución y eliminación deben definirse contractualmente con asesoría competente cuando corresponda.

## 11. Respaldo, continuidad y recuperación

La estrategia deberá ser independiente del repositorio principal y contemplar:

1. Copias periódicas de contenido, metadatos, historial y configuraciones necesarias para reconstrucción.
2. Separación lógica y, cuando sea viable, física o administrativa del entorno principal.
3. Protección contra borrado accidental, compromiso de credenciales, ransomware y alteración no autorizada.
4. Cifrado en tránsito y reposo cuando corresponda, con gestión separada y controlada de claves.
5. Registro de fecha, alcance, responsable, ubicación, resultado y errores de cada respaldo.
6. Pruebas documentadas de restauración, integridad y accesibilidad.
7. Procedimiento de continuidad y priorización de servicios y registros críticos.
8. Definición de RPO, RTO, frecuencia y retención según criticidad, obligaciones, presupuesto y capacidad operativa.

**Estado actual:** proveedor, ubicación independiente, calendario, retención, objetivos RPO/RTO y pruebas de restauración no están definidos ni verificados por esta política. No se afirmará que existen respaldos operativos hasta configurar y probar el mecanismo elegido.

## 12. Retención, suspensión de eliminación y disposición

No establecer plazos universales sin evaluar tipo de registro, jurisdicción, obligaciones legales, contratos, litigios potenciales y necesidades operativas. Para cada clase documental definir responsable, plazo o criterio, evento inicial, fundamento, suspensión, método de eliminación y evidencia de ejecución.

Ante auditoría, investigación, controversia, litigio real o razonablemente previsible, requerimiento de autoridad o instrucción profesional de conservación, suspender la eliminación de los registros relacionados (legal hold o conservación extraordinaria). Registrar alcance, autoridad que instruye, fecha, custodios notificados, confirmaciones y liberación formal. No reanudar la eliminación hasta que la suspensión haya sido levantada por quien tenga competencia y se hayan evaluado las obligaciones aplicables.

La eliminación requiere autorización expresa del responsable general y revisión profesional cuando existan obligaciones legales, regulatorias, laborales, contables, tributarias o de privacidad. Debe documentarse qué se eliminó, por qué, cuándo, mediante qué método, quién ejecutó y quién autorizó. No destruir registros sujetos a conservación obligatoria. Las copias residuales en respaldos se tratarán según el ciclo técnico documentado y las obligaciones aplicables.

## 13. Incidentes de integridad, confidencialidad o disponibilidad

Ante pérdida, alteración, divulgación indebida, corrupción, acceso no autorizado o indisponibilidad:

1. Contener el incidente sin destruir evidencia ni agravar el impacto.
2. Preservar registros, archivos, bitácoras y marcas de tiempo disponibles.
3. Registrar detección, alcance conocido, sistemas, datos y documentos afectados.
4. Informar al responsable general y solicitar apoyo especializado según la naturaleza.
5. Evaluar con profesionales competentes las obligaciones de notificación, plazos y comunicaciones.
6. Recuperar desde fuentes verificadas y documentar validaciones.
7. Registrar impacto, decisiones, acciones correctivas y lecciones aprendidas.

No atribuir públicamente causas o responsabilidades sin evidencia suficiente. No alterar ni destruir evidencia del incidente durante la investigación.

## 14. Excepciones y desviaciones

Toda desviación temporal de esta política requiere registro con requisito afectado, motivo, alcance, activos o documentos involucrados, riesgo, controles compensatorios, responsable, autorización, revisión profesional cuando corresponda, fecha de expiración y condición de cierre.

Una excepción no puede dispensar una obligación legal, regulatoria, contractual ni un impedimento profesional obligatorio. Si el riesgo no puede aceptarse o mitigarse, la actividad afectada debe detenerse. Las excepciones vencidas no se consideran vigentes automáticamente.

## 15. Responsabilidades y separación de funciones

- **Responsable general:** autoridad de aprobación interna, autoriza accesos y disposiciones dentro de sus competencias y asegura que las limitaciones estén declaradas. No sustituye profesionales ni autoridades públicas.
- **Custodio documental:** mantiene inventario, metadatos, custodia y registros dentro del alcance delegado.
- **Responsable técnico de respaldo/seguridad:** implementa, prueba y documenta controles técnicos cuando sea designado.
- **Profesionales competentes:** revisan materias de su especialidad y documentan alcance, versión examinada, fecha, observaciones y conclusión.
- **Colaboradores autorizados:** cumplen clasificación, acceso, conservación y reporte.
- **Herramientas de IA:** pueden asistir en análisis y controles; no certifican por sí mismas autenticidad, cumplimiento, revisión profesional ni aprobación institucional.

Mientras una sola persona concentre funciones, esa circunstancia debe declararse. Aplicar controles compensatorios viables, como historial inalterado, revisión externa cuando proceda, evidencia de autorizaciones y separación de credenciales. No describir como independiente una revisión realizada por la misma persona que elaboró el documento.

## 16. Transparencia y divulgación a terceros

ZivaLatam podrá comunicar políticas, estados de control, prácticas y compromisos aprobados mediante versiones públicas o resúmenes controlados. Antes de divulgar, revisar exactitud, vigencia, derechos, privacidad, confidencialidad, seguridad y aprobación.

La transparencia no autoriza divulgar datos personales, secretos, vulnerabilidades explotables, credenciales, información contractual reservada ni documentos de terceros sin base legítima. Toda afirmación dirigida a inversores, clientes o usuarios deberá distinguir claramente entre capacidades existentes y verificadas, controles en implementación, planes y objetivos. No presentar una política aprobada como prueba de que su implementación técnica ya ocurrió.

## 17. Controles pendientes de implementación y verificación

Esta política no acredita que estén activos: respaldo independiente, calendario y retención, pruebas de restauración, hashes automatizados, inventario maestro, cadena de custodia operativa, gestión formal de secretos, permisos granulares, revisión periódica de accesos, registro centralizado de incidentes, legal hold, archivo inmutable, firma o sellado de tiempo y procedimiento de continuidad.

Cada control pasa por definición, responsable, implementación, prueba, evidencia fechada, revisión y estado. Solo entonces podrá marcarse VERIFICADO.

## 18. Revisión y aprobación

Esta política permanece EN DESARROLLO hasta aprobación expresa del responsable general y registro de la versión exacta. Las materias jurídicas, regulatorias, privacidad, ciberseguridad y retención legal requieren revisión profesional cuando corresponda.

Revisar al menos ante cambios materiales en operaciones, sistemas, jurisdicciones, riesgos, estructura de responsabilidades o después de incidentes relevantes. La periodicidad concreta de revisión se establecerá en el procedimiento de control documental.
