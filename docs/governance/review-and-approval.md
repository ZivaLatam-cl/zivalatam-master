# Revisión y aprobación documental

> **Estado:** APROBADO — procedimiento institucional.

## Objetivo

Evitar que la creación técnica de un archivo, la revisión de contenido, la aprobación institucional y la integración en Git se confundan entre sí.

## Flujo institucional

1. **Preparación:** identificar objetivo, alcance, autor/responsable, clasificación y documentos afectados.
2. **Trabajo aislado:** crear una rama desde la base acordada; no desarrollar directamente sobre `main`.
3. **Presentación:** abrir un Pull Request con resumen, justificación, evidencia, riesgos, dependencias e Issues/ADRs relacionados.
4. **Revisión técnica/documental:** comprobar exactitud, coherencia, fuentes, seguridad, estado documental, enlaces y cambios relacionados.
5. **Revisión especializada:** solicitar revisión profesional independiente cuando la materia, riesgo, ley o compromiso externo lo requiera. Registrar alcance, versión examinada, fecha, observaciones y conclusión.
6. **Corrección:** responder observaciones y actualizar la rama; cambios sustanciales requieren repetir las revisiones afectadas.
7. **Aprobación institucional:** la autoridad designada registra decisión, alcance, condiciones, versión exacta y fecha mediante un registro `APR`.
8. **Integración:** realizar merge solo después de la autorización institucional requerida y de superar los controles técnicos aplicables.
9. **Cierre:** verificar el commit integrado, actualizar índices, estados y referencias cruzadas.

## Funciones y límites

- **Autor/responsable:** prepara el cambio, declara su origen y responde por su integridad.
- **Revisor técnico/documental:** examina coherencia, exactitud, trazabilidad y controles; no adquiere por ello autoridad institucional.
- **Profesional competente:** emite una revisión dentro de su especialidad y alcance; no se presume por la intervención de una IA.
- **Aprobador institucional:** autoriza la incorporación o vigencia dentro de sus facultades documentadas.
- **Mantenedor:** administra el repositorio y aplica controles técnicos; no sustituye al aprobador.
- **Asistente de IA:** puede investigar, redactar, analizar y ejecutar cambios autorizados; no es persona independiente, no emite certificaciones y no aprueba en nombre del titular o de un profesional.

Una persona puede acumular funciones por necesidad operativa solo si la limitación queda declarada y se aplican controles compensatorios. No describir como independiente una revisión realizada por la misma persona que preparó o aprobó el contenido.

## Situación operativa declarada

Mientras el proyecto esté bajo la responsabilidad de un único titular, la aprobación institucional interna corresponde a ese titular, dentro de sus facultades y sin sustituir revisión profesional, requisitos legales ni decisiones de autoridades externas. Esta asignación describe el gobierno interno del proyecto; no acredita por sí sola la constitución de una persona jurídica, un cargo societario ni facultades de representación frente a terceros.

Según declaración expresa del titular del proyecto:

- **Cuenta institucional principal y administradora del repositorio:** `ZivaLatam-Oficial`.
- **Cuenta secundaria bajo propiedad y control del mismo titular:** `lusdrey523`.

La relación entre ambas cuentas se documenta como declaración del titular, no como verificación independiente de identidad, titularidad o control realizada por GitHub.

### Control compensatorio temporal de cuentas

1. Ambas cuentas se consideran controladas por la misma persona mientras no exista evidencia documentada de un cambio.
2. La cuenta secundaria puede ejecutar un merge previamente autorizado si los permisos y reglas de GitHub lo permiten; esto solo separa una operación, no crea independencia funcional.
3. Ninguna cuenta puede usarse para simular una revisión independiente de la otra ni para eludir la restricción de autoaprobación de GitHub.
4. La aprobación institucional se registra separadamente mediante un expediente `APR`, identificando responsable, decisión, alcance, fecha y versión/commit exacto.
5. No compartir contraseñas, códigos MFA, tokens ni claves entre personas o incorporarlos al repositorio. Cada cuenta debe mantener sus propios factores de autenticación.
6. Al incorporarse colaboradores, revisar permisos, titularidad, recuperación y separación real de funciones.

**Naturaleza:** control compensatorio temporal, no doble control humano, revisión independiente ni auditoría externa.

## Criterios mínimos de revisión

- Objetivo, alcance, exclusiones y estado claros.
- Afirmaciones respaldadas o etiquetadas como REPORTADO, HIPÓTESIS o PROPUESTO.
- Fuentes pertinentes, fechadas y localizables.
- Identificadores, versiones y enlaces consistentes.
- Riesgos, limitaciones, dependencias y conflictos documentados.
- Ausencia de secretos y datos personales innecesarios.
- Impacto sobre documentos relacionados identificado.
- Controles descritos como pendientes cuando no exista evidencia de implementación.

## Estados del Pull Request

- **Draft:** trabajo incompleto.
- **Ready for review:** contenido presentado para revisión.
- **Changes requested:** requiere correcciones.
- **Approved:** revisión de GitHub registrada por una persona distinta del autor cuando así lo exijan las reglas; no equivale automáticamente a aprobación institucional.
- **Merged:** cambio integrado; no implica por sí solo aprobación institucional ni revisión profesional.

## Protección de `main`

Se recomienda configurar y verificar, según el plan y capacidades disponibles de GitHub:

- Pull Request obligatorio.
- Aprobación humana distinta del autor cuando sea viable.
- Descartar aprobaciones obsoletas ante cambios sustanciales.
- Bloquear force-push y eliminación de `main`.
- Exigir checks automatizados cuando existan.
- Restringir bypass y documentar quién puede usarlo.

**Estado técnico conocido:** la protección de rama no se ha comprobado como activa. No afirmar que está configurada hasta verificar la configuración efectiva del repositorio.

## Evidencia de aprobación

Cada registro `APR` debe incluir documento y versión exacta, commit SHA o tag, autoridad, persona/órgano, fecha, decisión, alcance, condiciones, referencias a revisión y evidencia de autorización. La aprobación en GitHub puede complementar el expediente, pero no reemplaza la identificación de la autoridad competente.