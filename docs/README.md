# ZivaLatam — Portal de conocimiento institucional

> **Estado:** APROBADO — portal de navegación institucional, versión 0.2 (APR-004)  
> **Repositorio:** `ZivaLatam-cl/zivalatam-master`  
> **Fuente documental:** `main` es la referencia documental institucional. Este portal forma parte de la arquitectura del conocimiento aprobada mediante APR-004.

Bienvenido al punto de entrada del conocimiento institucional de ZivaLatam. Este portal está diseñado para que una persona pueda comprender el proyecto, localizar un documento, seguir la evidencia de una decisión y reutilizar conocimiento sin depender de conversaciones anteriores ni conocer de antemano la estructura del repositorio.

## Encuentra lo que necesitas

| Si necesitas… | Empieza aquí |
|---|---|
| Entender cómo se organiza el conocimiento | [Arquitectura del conocimiento](knowledge-architecture.md) |
| Reconstruir el origen y las etapas anteriores a ZivaLatam | [Historia y evolución](foundation/history-and-evolution.md) |
| Consultar el antecedente experimental de BREGPersonal | [Expediente BREGPersonal](ecosystem/historical-initiatives/bregpersonal.md) |
| Saber qué áreas y relaciones componen el ecosistema | [Mapa de conocimiento](knowledge-map.md) |
| Encontrar un documento por tema, identificador o estado | [Índice maestro](master-index.md) |
| Comprender los términos y nombres institucionales | [Glosario](glossary.md) |
| Retomar el trabajo y conocer los próximos focos | [Prioridades documentales](current-priorities.md) |
| Conocer las reglas para crear, revisar y aprobar documentos | [Gobierno documental](governance/README.md) |

## Navegación por área

- **Fundación institucional:** identidad, historia, propósito, misión, visión y principios. Se incorporará cuando los expedientes estén preparados y revisados.
- **Ecosistema:** capacidades compartidas, productos, módulos, relaciones y evolución.
- **Investigación y evidencia:** estudios, normas, estándares, fuentes y evaluaciones.
- **Casos de uso y mercados:** problemas, segmentos, procesos y validación.
- **Arquitectura:** modelos conceptuales, decisiones, especificaciones y documentación para desarrolladores.
- **Estrategia:** modelo de negocio, prioridades, expansión y alianzas.
- **Gobierno:** reglas documentales, decisiones y aprobaciones ya incorporadas.

Las áreas futuras no se representan como carpetas vacías. Se crean cuando exista contenido real y un responsable o propósito documental identificable.

## Cómo leer los estados

No confundas el estado de un documento con el estado de una capacidad:

- **Propuesto:** idea o alternativa en consideración.
- **Borrador:** contenido en elaboración.
- **En revisión:** presentado para revisión.
- **Aprobado:** aprobación explícita registrada para un alcance y versión determinados.
- **Implementado:** puesto en funcionamiento, con evidencia.
- **Verificado:** comprobado mediante evidencia objetiva.
- **Superado / archivado:** reemplazado o conservado sin vigencia.

Una propuesta aprobada como criterio de diseño no significa que exista un producto implementado. Consulta el [marco de gobierno documental](governance/README.md).

## Reglas de navegación y reutilización

1. Cada tema tiene un expediente principal; los demás documentos lo enlazan.
2. Los índices son mapas de acceso, no copias del contenido.
3. Las investigaciones identifican fuentes, metodología, fecha, alcance y limitaciones.
4. Las decisiones enlazan las investigaciones y requisitos que las motivan, así como los documentos afectados.
5. Los nombres de productos y módulos se escriben de forma consistente con el glosario.
6. Los enlaces internos se escriben como rutas relativas para funcionar en GitHub y en clones locales.
7. Si un dato no está confirmado, se marca como declaración, hipótesis, análisis o propuesta.

## Plantillas

- [Ficha de conocimiento](../templates/knowledge-record-template.md)
- [Ficha de investigación](../templates/research-template.md)

## Gobierno y contribución

Los cambios se preparan mediante ramas y Pull Requests. La integración en `main` no sustituye las aprobaciones institucionales ni las revisiones profesionales requeridas. No incorporar secretos, credenciales, claves privadas ni datos personales innecesarios.

Consulta [README del repositorio](../README.md) para el alcance institucional, [gobierno documental](governance/README.md) para el procedimiento vigente y [APR-004](governance/approvals/ZIVA-APR-004-knowledge-architecture.md) para el registro de aprobación de esta arquitectura.
