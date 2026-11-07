# Gobierno documental de ZivaLatam

> **Estado:** APROBADO — aprobaciones institucionales registradas en ZIVA-APR-001 y ZIVA-APR-002.  
> **Ámbito:** repositorio maestro `ZivaLatam-cl/zivalatam-master`.  
> **Versión:** 0.2.1 — base de gobierno documental.

## Propósito y alcance

Establecer una forma única, verificable y reproducible de crear, investigar, revisar, aprobar, publicar y conservar documentación institucional de ZivaLatam. Este marco regula el expediente documental; no constituye por sí mismo una entidad jurídica, licencia, certificación, sistema de control implementado ni prueba de operación comercial.

El repositorio maestro es el registro oficial de los documentos que hayan sido incorporados conforme al procedimiento y aprobados cuando corresponda. La existencia de un archivo en una rama o Pull Request no lo convierte en política vigente.

## Principios

1. **Fuente oficial controlada:** `main` contiene la versión institucional publicada. Ramas y Pull Requests son espacios de trabajo y revisión, no fuentes vigentes.
2. **Evidencia antes que afirmaciones:** distinguir hechos verificados, información reportada, hipótesis y propuestas.
3. **Trazabilidad de extremo a extremo:** vincular conclusiones con fuentes, análisis, responsable, revisión, decisión y versión.
4. **Aprobación explícita:** no inferir aprobación por redacción, commit, publicación, comentario, aprobación técnica o merge.
5. **Historial preservado:** realizar cambios mediante ramas y Pull Requests; no reescribir historial publicado salvo procedimiento excepcional autorizado y documentado.
6. **Mínimo privilegio:** conceder únicamente permisos necesarios, con revisión y revocación cuando cambien las funciones.
7. **Protección de información:** no incorporar contraseñas, tokens, claves privadas, datos personales innecesarios ni secretos comerciales sin controles adecuados.
8. **Transparencia de estado:** diferenciar propuesta, aprobación interna, implementación y verificación con evidencia.
9. **Revisión competente:** materias jurídicas, regulatorias, privacidad, seguridad y otras especialidades requieren profesionales competentes cuando el riesgo o la ley lo exijan.

## Fuente documental y ramas

- `main`: registro institucional publicado, sujeto a las aprobaciones aplicables.
- Rama de trabajo: espacio aislado para preparar cambios.
- Pull Request: expediente de propuesta, discusión, revisión y autorización de integración.
- Commit: unidad versionada de cambio; no representa por sí solo una aprobación.
- Merge: integración técnica; no sustituye la aprobación institucional ni revisiones profesionales pendientes.

La aprobación institucional se acredita mediante el registro APR vinculado a la versión exacta. La integración técnica en `main` no acredita por sí sola implementación ni verificación.

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

La estructura podrá ampliarse mediante Pull Request. Las investigaciones específicas deberán organizarse en expedientes propios con identificador único, alcance, metodología, fuentes, hallazgos, limitaciones y decisiones relacionadas.

## Sistema de identificación documental

Cada registro tendrá un identificador único, permanente y no reutilizable:

| Tipo documental | Prefijo | Ejemplo |
|---|---|---|
| Políticas institucionales | `POL` | `ZIVA-POL-001` |
| Investigaciones | `INV` | `ZIVA-INV-001` |
| Fuentes y evidencias | `EVD` | `ZIVA-EVD-001` |
| Decisiones institucionales | `ADR` | `ZIVA-ADR-001` |
| Aprobaciones | `APR` | `ZIVA-APR-001` |
| Procedimientos | `PRO` | `ZIVA-PRO-001` |
| Revisiones profesionales | `REV` | `ZIVA-REV-001` |

La numeración será secuencial dentro de cada categoría. Los identificadores retirados, superados o archivados no se asignarán nuevamente. Los ejemplos no reservan ni asignan números reales. El ID permanece estable aunque cambie el título o la versión.

## Estados documentales

| Estado | Significado |
|---|---|
| BORRADOR | Contenido en elaboración |
| EN REVISIÓN | Presentado formalmente para revisión |
| APROBADO | Aprobación explícita registrada por autoridad designada |
| RECHAZADO | Revisado y no aprobado; conservar motivo |
| SUPERADO | Reemplazado por una versión o decisión posterior |
| ARCHIVADO | Conservado sin vigencia operativa |

Los estados **APROBADO**, **IMPLEMENTADO** y **VERIFICADO** no son intercambiables. La aprobación autoriza un contenido dentro de un alcance; la implementación acredita que se ejecutó; la verificación exige evidencia objetiva del resultado.

## Documentos relacionados

- [Convenciones de commits](commit-conventions.md)
- [Revisión y aprobación](review-and-approval.md)
- [Modelo de trazabilidad](traceability-model.md)
- [Registro de decisiones](decision-records/README.md)
- [Registro de aprobaciones](approvals/README.md)

## Control de cambios y límites actuales

Toda modificación de estas reglas debe pasar por Pull Request. La protección de `main`, revisiones obligatorias y controles automáticos solo se considerarán activos cuando su configuración haya sido comprobada en GitHub.

Este marco está APROBADO para el gobierno documental interno de ZivaLatam. Su aprobación no demuestra que los controles descritos estén implementados ni que ZivaLatam tenga una estructura societaria o regulatoria determinada.
