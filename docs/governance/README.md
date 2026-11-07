# Gobierno documental de ZivaLatam

> **Estado:** EN DESARROLLO — propuesta pendiente de aprobación institucional.  
> **Ámbito:** repositorio maestro `ZivaLatam-cl/zivalatam-master`.  
> **Versión:** 0.1.0 (borrador inicial).

## Propósito

Establecer una forma única, verificable y reproducible de crear, revisar, aprobar y conservar documentación institucional, investigaciones y decisiones de ZivaLatam.

## Principios

1. **Una fuente oficial:** este repositorio es el registro documental maestro. Notion, correo y otros servicios pueden facilitar el trabajo, pero no sustituyen el registro aprobado aquí.
2. **Evidencia antes que afirmaciones:** distinguir hechos verificados, información reportada, hipótesis y propuestas.
3. **Trazabilidad de extremo a extremo:** cada conclusión relevante debe poder vincularse con sus fuentes, análisis, responsable, revisión y decisión.
4. **Aprobación explícita:** un documento no se considera aprobado por haber sido redactado, subido o comprometido.
5. **Historial preservado:** los cambios se realizan mediante commits y Pull Requests; no se reescribe el historial publicado salvo procedimiento excepcional documentado.
6. **Mínimo privilegio:** cada colaborador recibe solo los permisos necesarios.
7. **Protección de información:** no incorporar contraseñas, tokens, claves privadas, datos personales innecesarios ni secretos comerciales sensibles sin controles adecuados.

## Estructura documental inicial

```text
.github/
  pull_request_template.md
docs/
  governance/
    README.md
    commit-conventions.md
    review-and-approval.md
    traceability-model.md
    decision-records/
      README.md
      ADR-TEMPLATE.md
    approvals/
      README.md
      APPROVAL-TEMPLATE.md
```

La estructura podrá ampliarse mediante Pull Request. Las investigaciones específicas deberán organizarse bajo un directorio propio acordado, con identificador único y expediente de fuentes, metodología, hallazgos y limitaciones.

## Sistema de identificación documental

Cada registro tendrá un identificador único, permanente y no reutilizable, con la siguiente nomenclatura:

| Tipo documental | Prefijo | Ejemplo |
|---|---|---|
| Políticas institucionales | `POL` | `ZIVA-POL-001` |
| Investigaciones | `INV` | `ZIVA-INV-001` |
| Fuentes y evidencias | `EVD` | `ZIVA-EVD-001` |
| Decisiones institucionales | `ADR` | `ZIVA-ADR-001` |
| Aprobaciones | `APR` | `ZIVA-APR-001` |
| Procedimientos | `PRO` | `ZIVA-PRO-001` |
| Revisiones profesionales | `REV` | `ZIVA-REV-001` |

La numeración será secuencial dentro de cada categoría. Los identificadores retirados, superados o archivados no se asignarán nuevamente. El identificador deberá mantenerse estable durante toda la vida del registro, aunque cambie su título o versión.

## Estados documentales

| Estado | Significado |
|---|---|
| BORRADOR | Contenido en elaboración, no revisado |
| EN REVISIÓN | Presentado formalmente para revisión |
| APROBADO | Aprobación explícita registrada por autoridad designada |
| RECHAZADO | Revisado y no aprobado; conservar motivo |
| SUPERADO | Reemplazado por una versión o decisión posterior |
| ARCHIVADO | Conservado sin vigencia operativa |

Los estados **APROBADO** y **VERIFICADO** no son intercambiables. Una afirmación puede estar verificada sin que la política o documento que la contiene esté aprobado.

## Documentos relacionados

- [Convenciones de commits](commit-conventions.md)
- [Revisión y aprobación](review-and-approval.md)
- [Modelo de trazabilidad](traceability-model.md)
- [Registro de decisiones](decision-records/README.md)
- [Registro de aprobaciones](approvals/README.md)

## Control de cambios

Toda modificación de estas reglas debe pasar por Pull Request y quedar reflejada en el historial de Git. Este documento permanece como propuesta hasta que exista aprobación institucional registrada.
