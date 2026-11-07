# Convenciones de commits

> **Estado:** EN DESARROLLO — propuesta pendiente de aprobación.

## Formato

Usar el formato:

```text
tipo(ámbito): resumen imperativo y breve
```

Tipos recomendados:

| Tipo | Uso |
|---|---|
| docs | Documentación, políticas, guías y registros |
| research | Incorporación o actualización de investigación |
| decision | Registro o actualización de decisiones |
| feat | Nueva funcionalidad o capacidad |
| fix | Corrección de errores |
| refactor | Reorganización sin cambiar el comportamiento esperado |
| test | Pruebas y validaciones |
| chore | Mantenimiento, configuración o tareas auxiliares |
| security | Cambios relacionados con seguridad |

Ejemplos:

```text
docs(governance): add document control policy
research(zivaid): add source register for identity study
decision(architecture): record identity graph alternatives
fix(readme): correct repository navigation
chore(github): add pull request template
```

## Reglas

1. Un commit debe representar un cambio lógico y acotado.
2. El mensaje debe explicar qué cambia; la descripción del PR explica por qué.
3. No mezclar en un mismo commit investigaciones no relacionadas, cambios de política y modificaciones técnicas independientes.
4. No incluir secretos, credenciales ni archivos temporales.
5. No presentar como aprobado un documento que sigue en borrador.
6. En trabajos relevantes, el cuerpo del Pull Request debe indicar el identificador de investigación, decisión o issue relacionado.
7. Preferir commits pequeños y descriptivos; evitar mensajes genéricos como `update`, `changes` o `final`.

## Ramas

Convención sugerida:

- `docs/<tema>`
- `research/<id>-<tema>`
- `decision/<tema>`
- `feat/<tema>`
- `fix/<tema>`
- `chore/<tema>`

Ejemplos: `research/zivaid-001-identity-assurance`, `docs/governance-policy`.

## Relación con Issues y Pull Requests

- Issue: registra la necesidad, pregunta o tarea.
- Branch: contiene el trabajo aislado.
- Commit: registra una unidad concreta de cambio.
- Pull Request: presenta el cambio, su contexto, evidencia y revisión.
- Merge: incorpora el cambio a la rama principal tras cumplir los controles establecidos.

## Autoría y automatización

Los commits deben conservar la autoría real proporcionada por GitHub. La asistencia de IA debe declararse en el Pull Request cuando haya contribuido materialmente al contenido. La IA no debe atribuirse una aprobación humana ni suplantar a un responsable institucional.
