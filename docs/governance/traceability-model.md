# Modelo mínimo de trazabilidad documental

> **Estado:** APROBADO — modelo institucional de trazabilidad.

## Cadena de trazabilidad

```text
Necesidad / pregunta
  -> Issue
  -> Investigación / expediente
  -> Fuente primaria o secundaria
  -> Evidencia localizada
  -> Análisis / hallazgo
  -> Decisión (ADR o registro equivalente)
  -> Pull Request
  -> Revisión técnica y profesional, cuando corresponda
  -> Aprobación institucional (APR)
  -> Commit / merge
  -> Versión publicada
  -> Verificación de implementación, si aplica
```

Cada salto debe ser navegable mediante identificadores y enlaces estables. Si un vínculo no existe, debe indicarse expresamente; no se debe inferir ni reconstruir retrospectivamente sin evidencia.

## Identificadores

Usar los identificadores definidos en el documento principal:

- Investigación: `ZIVA-INV-NNN`
- Fuente o evidencia: `ZIVA-EVD-NNN`
- Decisión: `ZIVA-ADR-NNN`
- Aprobación: `ZIVA-APR-NNN`
- Política: `ZIVA-POL-NNN`
- Procedimiento: `ZIVA-PRO-NNN`
- Revisión profesional: `ZIVA-REV-NNN`
- Issue y Pull Request: número nativo de GitHub y URL.

Los números son secuenciales por categoría y se asignan al crear el registro, no al redactar ejemplos. No reutilizar identificadores. Los registros retirados permanecen como SUPERADOS o ARCHIVADOS.

## Metadatos mínimos de una investigación

- ID, título, versión y estado.
- Responsable y fechas de creación/actualización.
- Pregunta, objetivo, alcance, exclusiones y jurisdicciones.
- Método, criterios de selección y fecha de corte.
- Registro de fuentes y evidencia examinada.
- Hallazgos separados de interpretación y recomendación.
- Limitaciones, incertidumbres, supuestos y conflictos de interés pertinentes.
- Decisiones, riesgos y dependencias relacionadas.
- Issues, PRs, commits y documentos vinculados.
- Revisión profesional y aprobación, si existen; no completar estos campos por inferencia.

## Registro mínimo de fuentes y evidencias

Cada fuente debe registrar, según corresponda:

- ID, autor o entidad emisora, título y tipo.
- URL o ubicación, versión y jurisdicción/ámbito.
- Fecha de publicación o actualización, si consta.
- Fecha de consulta, recepción o captura, con zona horaria cuando sea relevante.
- Afirmación concreta que respalda y localizador reproducible (página, sección, párrafo, tabla o identificador).
- Extracto mínimo necesario o descripción fiel; respetar derechos, licencias y restricciones.
- Evaluación de autoridad, actualidad, pertinencia y limitaciones.
- Estado de verificación y responsable de la evaluación.
- Relación con otras fuentes, discrepancias y evidencia contraria.

No usar una fuente para respaldar afirmaciones que no contiene. Si una fuente secundaria resume una norma o estándar, preferir y buscar la fuente primaria para conclusiones relevantes. Registrar las fechas de consulta para datos susceptibles de cambio.

## Clasificación de afirmaciones

- **VERIFICADO:** contrastado con evidencia identificable, suficiente y pertinente para el alcance y fecha declarados.
- **REPORTADO:** comunicado por una persona o entidad, sin corroboración suficiente.
- **HIPÓTESIS:** explicación o supuesto pendiente de prueba.
- **PROPUESTO:** alternativa o recomendación no aprobada.
- **APROBADO:** decisión formalmente autorizada; no implica que sus premisas estén verificadas ni que esté implementada.

La etiqueta VERIFICADO debe indicar qué se verificó, con qué evidencia, por quién, cuándo y dentro de qué límites. No extender una verificación más allá de su alcance.

## Integridad, conservación y correcciones

No editar silenciosamente evidencia histórica. Corregir mediante nueva versión o nota de rectificación, preservando el vínculo con el contenido anterior. Distinguir fecha de publicación de una fuente, fecha de consulta y fecha de incorporación al repositorio.

Un hash permite comparar bytes de dos objetos; por sí solo no acredita autoría, origen, fecha cierta, veracidad del contenido ni custodia continua. Un enlace externo puede cambiar o desaparecer. Para investigaciones críticas, conservar metadatos suficientes y una copia autorizada cuando sea legal y técnicamente posible.

## Límites actuales

Este modelo establece el procedimiento institucional de trazabilidad. No acredita que estén implementados captura automática, sellado de tiempo confiable, firma electrónica, hash automatizado, respaldo externo, archivo inmutable ni un sistema de gestión de evidencias. Su implementación deberá tener responsable, alcance, pruebas y evidencia fechada.