# Revisión y aprobación documental

> **Estado:** EN DESARROLLO — propuesta pendiente de aprobación institucional.

## Objetivo

Evitar que la creación técnica de un archivo se confunda con su validación o aprobación institucional.

## Flujo obligatorio propuesto

1. **Preparación:** identificar el objetivo, alcance, autor/responsable y documentos afectados.
2. **Trabajo aislado:** crear una rama desde `main`; no desarrollar directamente sobre `main`.
3. **Presentación:** abrir un Pull Request con resumen, justificación, evidencia, riesgos y referencias a Issues/ADRs.
4. **Revisión:** comprobar exactitud, coherencia, fuentes, seguridad, estado documental y cumplimiento de las convenciones.
5. **Corrección:** responder observaciones y actualizar la rama.
6. **Aprobación:** una persona con autoridad expresamente designada registra su aprobación en GitHub y, cuando corresponda, en el registro de aprobaciones.
7. **Integración:** realizar merge solo después de la aprobación requerida y de superar los controles aplicables.
8. **Cierre:** actualizar índices, estado documental y referencias cruzadas.

## Separación de funciones

- **Autor:** prepara el cambio y responde por su integridad.
- **Revisor:** examina el contenido y deja observaciones.
- **Aprobador:** persona con autoridad institucional para autorizar la incorporación o vigencia.
- **Mantenedor:** administra el repositorio y aplica las reglas técnicas.

Una misma persona puede desempeñar más de una función solo cuando la política institucional lo permita y quede explícito. Para políticas, decisiones estratégicas, gobierno, cumplimiento y seguridad se recomienda revisión independiente.

ChatGPT puede preparar, analizar, proponer y ejecutar cambios técnicos autorizados. No puede otorgar aprobación institucional en nombre del usuario, de un órgano de gobierno o de un responsable humano.

## Criterios mínimos de revisión

- Objetivo y alcance claros.
- Afirmaciones respaldadas por fuentes o marcadas como hipótesis.
- Fechas, versiones e identificadores consistentes.
- Diferenciación entre APROBADO, EN DESARROLLO y VERIFICADO.
- Riesgos, limitaciones y dependencias documentados.
- Ausencia de secretos y datos innecesarios.
- Enlaces y referencias funcionales.
- Impacto sobre documentos relacionados identificado.

## Estados del Pull Request

- Draft: trabajo incompleto; no solicitar aprobación final.
- Ready for review: contenido preparado para revisión.
- Changes requested: requiere correcciones.
- Approved: revisión registrada por revisor autorizado.
- Merged: cambio integrado; no implica por sí solo aprobación institucional si esta no fue otorgada.

## Regla de protección de main

Se recomienda configurar en GitHub protección de la rama `main` con:

- Pull Request obligatorio.
- Al menos una aprobación humana antes del merge.
- Descartar aprobaciones obsoletas cuando cambie sustancialmente el PR.
- Bloquear force-push y eliminación de la rama.
- Exigir controles automáticos cuando se incorporen.
- Restringir bypass a responsables expresamente autorizados.

**Estado técnico:** esta política es una recomendación documental. La protección de rama no se ha configurado ni verificado todavía y deberá comprobarse en la configuración de GitHub.

## Evidencia de aprobación

Toda aprobación institucional debe registrar, como mínimo, documento y versión, persona/órgano aprobador, rol o autoridad, fecha, decisión, alcance y condiciones. El registro de GitHub complementa el expediente; no reemplaza la identificación de la autoridad competente.


## Control compensatorio temporal mientras exista un único titular

Mientras ZivaLatam opere con una sola persona titular y responsable de las decisiones institucionales, se permite distinguir una cuenta institucional principal y una cuenta operativa secundaria, sin presentar esa distinción como separación de funciones entre personas.

Según declaración expresa del titular del proyecto:

- **Cuenta institucional principal y administradora del repositorio:** `ZivaLatam-Oficial`.
- **Cuenta secundaria bajo propiedad y control del mismo titular:** `lusdrey523`.

Esta relación se documenta como una declaración del titular; no constituye por sí sola una verificación independiente de identidad, titularidad o control realizada por GitHub.

### Límites obligatorios

1. Ambas cuentas se consideran controladas por la misma persona mientras no exista evidencia documentada de un cambio.
2. El uso de `lusdrey523` para ejecutar un merge autorizado puede servir como separación operativa de credenciales o tareas, si los permisos y las reglas de GitHub lo permiten; no crea independencia funcional.
3. Ninguna de las dos cuentas podrá utilizarse para simular una revisión independiente de la otra ni para eludir la restricción de autoaprobación de GitHub.
4. La aprobación institucional corresponde al titular y debe quedar registrada por separado mediante un expediente `APR`, indicando persona responsable, decisión, alcance, fecha y versión.
5. El merge se ejecutará únicamente después de la autorización institucional documentada y de cumplir los controles aplicables. El uso de una cuenta secundaria no sustituye dicha autorización.
6. Al incorporarse colaboradores, deberá revisarse esta medida y establecerse una separación real de funciones, permisos y revisiones según los riesgos y responsabilidades.

**Naturaleza del control:** compensatorio y temporal. No equivale a revisión independiente, doble control humano ni auditoría externa.
