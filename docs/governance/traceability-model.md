# Modelo mínimo de trazabilidad documental

> **Estado:** EN DESARROLLO — propuesta pendiente de aprobación.

## Cadena de trazabilidad

```text
Necesidad / pregunta
  -> Issue
  -> Investigación / expediente
  -> Fuente primaria o secundaria
  -> Evidencia extraída
  -> Análisis / hallazgo
  -> Decisión (ADR o registro equivalente)
  -> Pull Request
  -> Revisión y aprobación
  -> Commit / merge
  -> Versión publicada
```

Cada salto debe ser navegable mediante identificadores y enlaces estables. Si un vínculo no existe, se debe indicar expresamente; no se debe inferir.

## Identificadores

Usar los identificadores oficiales definidos en el documento principal de gobierno:

- Investigación: `ZIVA-INV-001`
- Fuente o evidencia: `ZIVA-EVD-001`
- Decisión: `ZIVA-ADR-001`
- Aprobación: `ZIVA-APR-001`
- Política: `ZIVA-POL-001`
- Procedimiento: `ZIVA-PRO-001`
- Revisión profesional: `ZIVA-REV-001`
- Issue: número nativo de GitHub más URL.
- Pull Request: número nativo de GitHub más URL.

Los ejemplos ilustran el formato; los números reales se asignarán secuencialmente en el registro correspondiente. No reutilizar identificadores. Si un registro se retira, conservarlo como superado o archivado.

## Metadatos mínimos de una investigación

- ID y título.
- Estado: BORRADOR, EN REVISIÓN, APROBADO, RECHAZADO, SUPERADO o ARCHIVADO.
- Responsable y fecha de inicio/actualización.
- Pregunta, alcance y exclusiones.
- Método y criterios de selección.
- Registro de fuentes.
- Evidencias y hallazgos.
- Limitaciones, incertidumbres y conflictos de interés, cuando correspondan.
- Decisiones relacionadas.
- Issues, PRs y commits relacionados.
- Aprobación y versión vigente, si existen.

## Registro de fuentes y evidencias

Cada fuente o evidencia debe incluir ID, autor o entidad, título, URL/ubicación, fecha de publicación (si consta), fecha de consulta, tipo, jurisdicción/ámbito, afirmación que respalda, fragmento o localizador verificable, evaluación de confiabilidad y estado de verificación.

Conservar el documento original o una referencia estable cuando las licencias, privacidad y seguridad lo permitan. No copiar material protegido de forma incompatible con sus condiciones. Registrar hash criptográfico para originales cuando se implemente el procedimiento de conservación.

## Clasificación de afirmaciones

- **VERIFICADO:** contrastado con evidencia identificable y suficiente para el alcance declarado.
- **REPORTADO:** comunicado por una persona o entidad, aún no corroborado de forma independiente.
- **HIPÓTESIS:** explicación o supuesto pendiente de prueba.
- **PROPUESTO:** alternativa o recomendación no aprobada.
- **APROBADO:** decisión formalmente autorizada; no significa necesariamente que todos sus hechos subyacentes estén verificados.

## Integridad y conservación

No editar silenciosamente evidencia histórica. Corregir mediante nueva versión o nota de rectificación. Restringir información confidencial; almacenar secretos fuera del repositorio. Los enlaces externos pueden cambiar o desaparecer, por lo que las investigaciones críticas deben conservar metadatos suficientes para recuperar y evaluar la fuente.

## Límites actuales

Este modelo define el procedimiento documental. No se ha implementado todavía un sistema automático de captura de fuentes, sellado de tiempo, hash, respaldo externo, firma electrónica ni archivo de evidencia inmutable. Esos controles quedan para etapas posteriores.
