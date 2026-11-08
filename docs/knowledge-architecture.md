# ZivaLatam — Arquitectura del Conocimiento Institucional

| Campo | Valor |
|---|---|
| Identificador | `ZIVA-KNO-001` |
| Versión | 0.2 |
| Estado | APROBADA — APR-004 |
| Dominio | Gobierno del conocimiento |
| Responsable | Por designar formalmente |
| Fecha de elaboración | 2026-11-08 |
| Revisión | Aprobación institucional registrada el 2026-11-08 mediante APR-004 |
| Sustituye | Propuesta conceptual 0.1, no publicada como norma vigente |

## 1. Objetivo

Establecer una arquitectura documental que permita conservar, localizar, comprender, relacionar y reutilizar el conocimiento de ZivaLatam a medida que la iniciativa evolucione desde su etapa conceptual hacia investigación, diseño, desarrollo y operación.

La arquitectura debe servir tanto a la dirección institucional como a investigadores, especialistas, arquitectos y desarrolladores. Debe reducir la dependencia de conversaciones individuales, evitar duplicaciones y permitir reconstruir por qué se adoptó una decisión y qué evidencia la respalda.

## 2. Principios de diseño

1. **Localizable:** un lector debe poder llegar a la información por área, producto, capacidad, problema, decisión, identificador o estado.
2. **Reutilizable:** cada conocimiento tiene una ubicación principal y se referencia desde otros contextos; no se mantienen copias divergentes.
3. **Trazable:** los documentos relevantes enlazan sus fuentes, evidencias, decisiones, responsables y versiones.
4. **Comprensible por sí mismo:** cada expediente explica su propósito, alcance, estado, términos y relaciones, sin exigir conocer conversaciones previas.
5. **Progresivo:** la estructura crece con el contenido real; no se crean directorios vacíos para representar planes futuros.
6. **Orientado al lector:** la navegación responde a tareas y preguntas reales, además de la clasificación temática.
7. **Docs-as-code:** texto versionado, cambios revisables, enlaces comprobables y mantenimiento junto con los cambios institucionales o técnicos.
8. **Integridad institucional:** una propuesta, una aprobación, una implementación y una verificación son estados distintos y deben demostrarse por separado.

## 3. Modelo de información: dominio y necesidad del lector

La arquitectura combina dos ejes:

- **Dominios:** fundación, ecosistema, capacidades, productos, casos de uso, investigación, arquitectura, estrategia, historia y gobierno.
- **Necesidades del lector:** aprender, ejecutar una tarea, consultar una referencia precisa y comprender el contexto o las razones de una decisión.

Para documentación técnica y de desarrolladores se adopta como guía el modelo Diátaxis:
- Tutoriales: aprendizaje guiado mediante una experiencia práctica.
- Guías prácticas: instrucciones para completar una tarea concreta.
- Referencia: descripción precisa de interfaces, parámetros, formatos, contratos y comportamiento.
- Explicación: contexto, fundamentos, alternativas y razones.

Diátaxis se utiliza como criterio de clasificación editorial, no como obligación de crear cuatro carpetas para todo el repositorio. Un expediente puede enlazar documentos de distintos tipos cuando el lector lo necesite.

## 4. Estructura objetivo del repositorio

La siguiente estructura es una guía de evolución, no una instrucción para crear de inmediato todos los directorios. Solo se incorporarán carpetas cuando haya contenido que mantener.

```text
zivalatam-master/
├── README.md
├── .github/
│   └── pull_request_template.md
├── docs/
│   ├── README.md                    # Portal de conocimiento
│   ├── knowledge-architecture.md    # Esta arquitectura
│   ├── knowledge-map.md             # Mapa de áreas y relaciones
│   ├── master-index.md              # Índice y catálogo documental
│   ├── glossary.md                  # Vocabulario controlado
│   ├── current-priorities.md        # Focos y pendientes documentales
│   ├── foundation/                  # Identidad, propósito, historia y principios
│   ├── ecosystem/                   # Ecosistema, portafolio y relaciones
│   ├── capabilities/                # Capacidades transversales
│   ├── products/                    # Expedientes de productos y módulos
│   ├── use-cases/                   # Problemas, usuarios y casos de uso
│   ├── research/                    # Investigación y evidencias
│   ├── architecture/                # Modelos y especificaciones técnicas
│   ├── strategy/                    # Estrategia y modelo de negocio
│   └── governance/                  # Gobierno existente, ADR, APR y políticas
└── templates/
    ├── knowledge-record-template.md
    └── research-template.md
```

La historia y las iniciativas anteriores se conservarán como parte de los expedientes de fundación o historia cuando se consoliden. No se crean ahora carpetas para WAKU, ZAFU ni productos que todavía no tengan expedientes completos.

## 5. Portal, índices y rutas de acceso

El portal `docs/README.md` es la puerta de entrada. El índice maestro responde dónde está cada expediente; el mapa explica cómo se relacionan los dominios; el glosario normaliza términos; y el registro de prioridades permite retomar el trabajo.

Cada directorio que llegue a existir deberá tener un README que explique:
- qué contiene y qué no contiene;
- para quién está pensado;
- cómo se organiza;
- cuáles son sus documentos principales;
- qué otras áreas se relacionan;
- quién mantiene el contenido, cuando exista responsable designado.

Los README de directorio son guías locales, no duplicados del portal general.

## 6. Ficha y metadatos de los expedientes

Los expedientes sustantivos deben incorporar metadatos consistentes. La plantilla común establece como mínimo:

- ID estable y no reutilizable;
- título y tipo documental;
- dominio principal;
- estado y versión;
- fechas de creación y actualización;
- responsable o estado de asignación;
- propósito, alcance y limitaciones;
- relaciones con otros expedientes;
- fuentes y evidencias;
- etiquetas descriptivas.

Los metadatos en Markdown son texto mantenible por Git. No se presume que GitHub los indexe como campos estructurados ni que proporcione filtros relacionales automáticamente. La búsqueda avanzada o automatización podrá evaluarse cuando el volumen lo justifique.

## 7. Identificadores y vocabulario

Se reutilizarán las categorías ya incorporadas en el gobierno documental: `POL`, `INV`, `EVD`, `ADR`, `APR`, `PRO` y `REV`. No se reasignan ni renumeran identificadores existentes.

Los identificadores de productos, capacidades, casos de uso u otros objetos de conocimiento requieren una decisión posterior antes de convertirse en convención institucional. Mientras tanto, sus nombres se normalizan mediante el glosario y el índice, sin inventar identificadores oficiales.

## 8. Relaciones y reutilización

Los expedientes deben enlazarse cuando exista una relación sustantiva. Relaciones recomendadas:

- problema o necesidad → segmento y caso de uso;
- caso de uso → capacidades requeridas;
- capacidad → producto o módulo que podría utilizarla;
- investigación → hallazgo y evidencia;
- evidencia → requisito o decisión que respalda;
- decisión → documentos y componentes afectados;
- cambio → versión anterior y registro que lo autoriza.

La relación debe explicarse; un enlace sin contexto no siempre es suficiente. Si una investigación sirve a varios productos, se mantiene una sola investigación principal y se referencia desde cada producto.

## 9. Calidad, estados y confianza

Cada afirmación relevante debe poder distinguirse como:
- hecho verificado con fuente;
- declaración del fundador o de un colaborador;
- fuente externa aún no validada;
- hipótesis;
- análisis;
- propuesta;
- decisión aprobada;
- implementación documentada;
- resultado verificado.

No se debe convertir una declaración testimonial en hecho externo comprobado. La aprobación de un documento no demuestra que la capacidad descrita esté implementada. La evidencia debe tener fecha, origen y alcance.

## 10. Documentación para desarrolladores

Cuando existan componentes técnicos definidos, sus expedientes deberán separar:
- explicación de arquitectura y decisiones;
- tutoriales de inicio;
- guías para tareas frecuentes;
- referencia de API, esquemas, eventos, errores, permisos y versiones;
- requisitos de seguridad, privacidad, interoperabilidad y compatibilidad;
- ejemplos verificables y resultados esperados.

No se documentarán endpoints, contratos, tecnologías ni capacidades como existentes hasta que estén decididos y respaldados por artefactos técnicos reales.

## 11. Capacidades reales de GitHub y límites

Esta arquitectura utiliza funciones documentadas de GitHub: README por directorio, Markdown, enlaces relativos, historial Git, ramas y Pull Requests. Estas funciones permiten construir una documentación navegable sin introducir un generador de sitios ni una base de datos externa.

Límites relevantes:
- Los metadatos escritos en Markdown no se convierten automáticamente en filtros estructurados.
- Los enlaces relativos facilitan navegación en GitHub y clones locales, pero deben comprobarse tras mover o renombrar archivos.
- CODEOWNERS y revisiones obligatorias solo deben declararse activos después de comprobar su configuración.
- GitHub Pages es una opción de publicación separada; no se habilitará para contenido privado sin evaluar visibilidad, plan, permisos y exposición pública.
- No se presupone que la búsqueda de GitHub sustituya un índice curado.

## 12. Mantenimiento y control de cambios

Los cambios se presentan mediante Pull Request, siguiendo el gobierno documental vigente. Las modificaciones que cambien reglas institucionales requieren la aprobación que corresponda y su registro APR. Las propuestas de estructura o contenido pueden revisarse en PR sin declarar aprobadas las reglas.

Toda incorporación sustantiva debe verificar:
- enlaces internos y referencias;
- coherencia con glosario e índice;
- estado y versión;
- fuentes y limitaciones;
- relaciones con documentos afectados;
- ausencia de secretos y datos personales innecesarios.

## 13. Secuencia de implantación

1. Portal, mapa, índice, glosario y prioridades.
2. Fichas documentales y expedientes fundacionales consolidados.
3. Ecosistema, capacidades y portafolio.
4. Casos de uso e investigaciones.
5. Arquitectura y documentación técnica cuando haya decisiones y artefactos verificables.
6. Comprobaciones automáticas y herramientas adicionales cuando el volumen y el riesgo lo justifiquen.

## 14. Fuentes de referencia

- [Diátaxis — The Diátaxis framework](https://diataxis.fr/): clasificación de documentación por necesidades del lector.
- [Write the Docs — Documentation guide](https://www.writethedocs.org/guide/): prácticas de documentación, mantenimiento y colaboración.
- [GitHub Docs — About READMEs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes).
- [GitHub Docs — Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).
- [GitHub Docs — About protected branches](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/about-protected-branches).
- [GitHub Docs — GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site).

Las fuentes anteriores son referencias de diseño. La interpretación de las funciones disponibles debe contrastarse con la configuración y el plan real del repositorio antes de activar controles o publicar documentación.

## 15. Aprobación y límites

Esta versión 0.2 queda aprobada como arquitectura documental institucional mediante ZIVA-APR-004, dentro del alcance y las exclusiones allí registrados. Su aprobación no activa automatizaciones, protección de ramas, publicación web, CODEOWNERS, responsables formales ni controles técnicos; tampoco acredita implementación de sistemas o capacidades de negocio. Los cambios materiales futuros deberán someterse al procedimiento de revisión y aprobación vigente.
