# BREGPersonal — expediente histórico de concepto y experimentación

| Campo | Valor |
|---|---|
| Tipo documental | Expediente histórico de iniciativa / producto conceptual |
| Versión | 0.1 |
| Estado | BORRADOR — EN REVISIÓN DEL FUNDADOR |
| Dominio | Ecosistema / iniciativas históricas |
| Fuente principal | Declaraciones y reconstrucción del fundador, noviembre de 2026 |
| Fuentes complementarias | Repositorio personal público `breg-personal-ziva`, README y código revisados |
| Fecha de elaboración | 2026-11-08 |
| Naturaleza | Reconstrucción histórica; no es especificación vigente ni diseño aprobado de ZivaLatam |

> **Advertencia:** BREGPersonal fue una iniciativa conceptual y experimental anterior. Hubo versiones beta y código preliminar, pero el fundador indicó que no superaron pruebas técnicas y nunca se ofrecieron al público. No se acredita operación comercial, aprobación de créditos, custodia de fondos, integración bancaria, acuerdos con entidades financieras ni autorización regulatoria.

## 1. Identidad y propósito original

El nombre provisional correcto es **BREGPersonal**. Según el fundador, “BRE” proviene de su apellido Breto, “G” de Group y “Personal” expresaba que era una aplicación personal para organizar y controlar su propia información económica. El principio de que el titular mantuviera control sobre sus datos acompañó el concepto desde sus primeras exploraciones.

La idea inicial no era necesariamente prestar dinero. Consistía en reunir y organizar información económica —por ejemplo, boletas, comprobantes y resúmenes de actividad— para que una persona pudiera construir evidencia de ingresos y continuidad económica que no siempre quedaba reflejada en los mecanismos tradicionales.

Una orientación temprana contemplaba incorporar boletas y generar resúmenes diarios, semanales o quincenales de ingresos. El objetivo era ayudar a demostrar actividad e ingresos constantes; no existía todavía un sistema de crédito formalmente definido.

## 2. Evolución hacia el registro de actividad económica

Posteriormente, el concepto se adaptó a la actividad de reciclaje y recuperación de materiales que realizaba el fundador en Santiago. Este nicho fue una aplicación concreta posterior, no el único propósito original ni una definición universal del público objetivo.

La idea de registro contemplaba:
- materiales como latas de aluminio, chatarra, cobre, bronce, aluminio, ropa y calzado de segunda mano;
- cantidades recolectadas y vendidas;
- fechas y horas de venta;
- precios por tipo de material;
- ingresos totales por jornada y evolución de la actividad;
- historial económico organizado.

El fundador recuerda que una idea de ahorro/reserva contemplaba apartar el 15 % de los ingresos para un fondo de emergencias y que, al alcanzar determinados umbrales, se permitiría retirar el 75 % del presupuesto resguardado, manteniendo el 25 % como respaldo. Esta regla se conserva como recuerdo de una formulación conceptual; no se ha identificado en la versión de código revisada.

### 2.1 Diferencia con el artefacto de código localizado

En la beta examinada de `breg-personal-ziva`, el ingreso se registra como monto bruto de una jornada, con gastos y otros datos de actividad. No se encontró en esa versión un registro individual completo de cada venta con precio y hora, como el que recuerda el fundador.

El código de esa versión calcula una reserva Capital Semilla del 15 % sobre el ingreso neto (ingresos menos gastos). Esto difiere del recuerdo inicial del fundador, que se refería al 15 % del ingreso. La diferencia se registra, no se fuerza una conciliación sin evidencia de versiones adicionales.

En la versión examinada no se encontró la regla de retiro del 75 % dejando 25 % de respaldo. Esto no demuestra que nunca se hubiera considerado en otra iteración.

## 3. Evolución posterior: microfinanciamiento

En una etapa posterior, el fundador comenzó a considerar que las entidades financieras tradicionales podían no reconocer adecuadamente a personas cuya actividad económica no encajaba en sus modelos habituales. El concepto evolucionó desde el registro económico hacia un posible sistema de microcréditos apoyado en la información registrada por el usuario.

La idea explorada contemplaba:
- solicitudes de microcréditos basadas en el rendimiento económico registrado;
- un límite conceptual de hasta tres veces la capacidad de ingresos estimada;
- pagos flexibles que pudieran realizarse diaria, semanal, quincenal o mensualmente;
- adaptación de la frecuencia de pago a los ciclos reales de ingresos del usuario, para evitar que una única cuota al final del mes resultara difícil de cubrir.

El límite de tres veces fue una hipótesis conceptual, no una regla de crédito validada. No se definieron tasas aceptables, metodología de riesgo validada, capital disponible, política de provisiones, límites de endeudamiento ni modelo financiero completo.

El fundador no había determinado si el capital provendría de fondos propios, inversionistas o instituciones. La reconstrucción posterior precisó que la idea que llegó a explorar fue un marketplace P2P con prestamistas institucionales.

## 4. Modelo de marketplace P2P institucional imaginado

### 4.1 Tipo de prestamistas

La intención era que los prestamistas fueran principalmente empresas financieras y entidades especializadas, previamente registradas y habilitadas conforme al marco regulatorio que correspondiera. El fundador mencionó expresamente su intención de que estuvieran autorizadas por la CMF cuando correspondiera en Chile.

No se había determinado jurídicamente qué categorías de prestamistas podían participar, cuáles requerirían inscripción o autorización, ni si todos los prestamistas institucionales estarían sujetos a los mismos requisitos. La referencia a la CMF registra la intención de cumplimiento del fundador, no una conclusión legal general ni una autorización obtenida.

La plataforma no se imaginaba como un espacio abierto donde cualquier usuario pudiera ofrecer dinero sin controles.

### 4.2 Integración progresiva de la metodología con los financiadores

La metodología de reconocimiento económico se ofrecería inicialmente como herramienta complementaria a los modelos de riesgo existentes de las instituciones participantes. La intención era:
1. comenzar como fuente adicional de información;
2. permitir que las instituciones contrastaran su utilidad con sus propios criterios;
3. mejorar progresivamente la metodología y construir confianza institucional;
4. procurar que, con evidencia y aceptación, las instituciones pudieran integrarla completamente en sus criterios internos de evaluación crediticia.

La evaluación tradicional podría seguir utilizándose cuando la institución, sus políticas o sus obligaciones lo requirieran. La adopción completa era un objetivo futuro, no una condición inicial.

La decisión final de otorgar o rechazar cada crédito permanecería en el prestamista, aplicando sus propios criterios y responsabilidades. La presencia de una persona en una lista de candidatos sugeridos no equivaldría a aprobación ni garantizaría financiamiento.

### 4.3 Informe de evaluación

La idea era entregar un informe detallado que combinara:
- un indicador propio de capacidad económica;
- evidencias e indicadores que explicaran la evaluación;
- información disponible sobre actividad, ingresos y comportamiento económico.

No se llegó a definir si el indicador sería único para todas las personas o si tendría componentes adaptados a cada actividad. Tampoco se definió una metodología formal, ponderaciones aprobadas, validación estadística ni umbrales de decisión.

El indicador no debe describirse como score predictivo validado. La metodología requeriría validación empírica, revisión de sesgos, explicabilidad, controles de calidad y mecanismos de rectificación.

## 5. Flujo de solicitud y aprobación que se llegó a iterar

La siguiente secuencia reconstruye la idea explicada por el fundador. No representa un flujo funcional probado.

1. El usuario ingresaría al marketplace P2P de BREGPersonal.
2. La plataforma mostraría una lista de prestamistas sugeridos a partir del desempeño registrado del usuario.
3. El solicitante elegiría el prestamista de su preferencia.
4. Completaría un formulario breve de solicitud formal de microcrédito.
5. El prestamista recibiría una notificación y un informe actualizado del solicitante.
6. El prestamista revisaría el informe con sus propios criterios y decidiría si aprobar o rechazar.
7. Si rechazaba, el solicitante recibiría la notificación correspondiente.
8. Si aprobaba, el solicitante recibiría una notificación y un código de activación del protocolo de desembolso, proporcionado por el prestamista.
9. El solicitante debía tener previamente configurada una cuenta bancaria principal para recibir los fondos.
10. Al activar el código, el sistema lo redirigiría al dashboard financiero de BREGPersonal.
11. El dashboard mostraría un mensaje de nuevo crédito, el monto aprobado, el saldo a favor del crédito, el saldo de la cuenta BREG y una opción de retiro.
12. Para retirar fondos a su cuenta bancaria, el usuario debía introducir un código enviado al teléfono registrado y una palabra de seguridad para transferencias.

El código de activación, el segundo factor telefónico y la palabra de seguridad eran elementos de una propuesta de experiencia. No se definieron protocolos criptográficos, recuperación, límites, protección contra fraude, caducidad, revocación ni controles técnicos verificables.

## 6. Bóvedas individuales BREG y partner financiero hipotético

### 6.1 Una bóveda por prestamista

El fundador aclaró que no imaginaba un fondo común de todos los prestamistas. Cada prestamista tendría:
- su propia cuenta dentro de BREGPersonal;
- una cuenta de transferencias BREG, denominada **Bóveda**;
- un saldo y movimientos individualizados en el panel del prestamista.

Las bóvedas serían independientes entre prestamistas. La reconstrucción no permite afirmar que se hubiera definido una estructura contable, jurídica o de custodia completa.

### 6.2 Global66 como proveedor propuesto

La idea inicial era explorar la integración de [Global66](https://global66.com/) como partner financiero para administrar cuentas de dinero real y gestionar/controlar los flujos de efectivo. BREGPersonal mantendría cuentas de registro contable individuales que reflejarían los saldos y movimientos de cada prestamista, mientras los fondos reales serían administrados mediante cuentas y servicios del proveedor.

El fundador aclaró expresamente que:
- Global66 fue una empresa considerada como posible partner;
- nunca hubo conversaciones, negociaciones, acuerdos ni integración con Global66;
- no se verificó la disponibilidad de un producto de Global66 que soportara esta arquitectura;
- no se abrieron cuentas reales ni se implementaron las bóvedas BREG.

La propuesta de partner no debe interpretarse como respaldo, aprobación, relación comercial ni compromiso de Global66.

La participación de un proveedor financiero no habría conferido automáticamente legalidad al conjunto del modelo. Habría sido necesario revisar quién custodia jurídicamente los fondos, quién mantiene cuentas, quién ejecuta pagos, qué entidad contrata con el usuario, cómo se segregan fondos, qué sucede ante insolvencia y qué registros o autorizaciones exige cada actividad.

## 7. Devolución del crédito y distribución de pagos

### 7.1 Micro pagos flexibles

La idea era que el prestatario pudiera programar desde su dashboard pagos diarios, semanales, quincenales o mensuales, según el flujo real y constante de sus ingresos.

La intención declarada era que la persona pudiera devolver el crédito mediante microtransacciones de menor tamaño, sin depender necesariamente de una cuota mensual tradicional. El objetivo era adaptar la devolución a la frecuencia de ingresos del usuario.

No se definieron reglas de monto mínimo, pausas, períodos sin ingresos, mora, pago fallido, reprogramación, prepago, límites de débito ni protección de gastos esenciales. La flexibilidad no debe confundirse con autorización para extraer dinero automáticamente sin límites ni consentimiento válido.

### 7.2 Secuencia de distribución imaginada

El flujo que describió el fundador era:
1. El prestatario realizaría los pagos mediante el protocolo de micro pagos programados desde su dashboard BREG.
2. Global66 recibiría los fondos de devolución a través de la estructura financiera propuesta.
3. Global66 cobraría su parte por los servicios que prestara y transferiría el remanente a BREGPersonal.
4. BREGPersonal cobraría su comisión de emparejamiento.
5. El resto se transferiría a la cuenta/panel BREG del prestamista correspondiente, reflejando capital e intereses recuperados y los movimientos asociados.

La secuencia económica exacta, el orden jurídico de los pagos, el tratamiento tributario, la liquidación, las comisiones, el cálculo de intereses y la conciliación no llegaron a definirse. El orden anterior reproduce la idea explicada por el fundador, no un contrato ni un mecanismo validado con Global66.

### 7.3 Intención de la experiencia para el usuario

El prestatario no tendría que coordinar directamente pagos con el prestamista ni gestionar manualmente cada transferencia. La plataforma procuraría facilitar una devolución adaptada a sus ingresos, mientras el proveedor financiero administraría los flujos y BREGPersonal reflejaría los movimientos en los paneles respectivos.

Esto era una intención de diseño. No se acredita que el flujo se hubiera implementado ni que se hubieran resuelto las obligaciones de cobro, mandato, autorización, protección al consumidor o tratamiento de pagos.

## 8. Artefactos técnicos y diferencias observadas

### 8.1 Repositorio principal de experimentación localizado

[ breg-personal-ziva ](https://github.com/lusdrey523/breg-personal-ziva) contiene una beta experimental con un archivo HTML de gran tamaño y una versión preliminar `app/breg-personal-ziva-v0.1.html`. El README utiliza la denominación “BREG Personal FOS v2.1” y describe una PWA experimental.

La versión revisada incluye, entre otros elementos:
- registro de sesiones/jornadas;
- materiales, cantidades, kg e ingresos por jornada;
- gastos, tiempo, zona e historial;
- gráficos y productividad;
- PIN y bloqueo por inactividad;
- módulo Capital Semilla;
- simulación de préstamos y límites de crédito;
- conceptos de evaluación basados en consistencia, estabilidad, frecuencia, calidad de ingresos y anomalías.

El README describe ponderaciones de 30 % consistencia, 25 % estabilidad, 15 % frecuencia, 20 % calidad de ingresos y 10 % anomalías. Esas ponderaciones pertenecen a una versión experimental descrita en el repositorio; no constituyen una metodología validada estadísticamente ni evidencia de capacidad predictiva.

### 8.2 Arquitectura declarada en la beta

La documentación de esa versión distingue almacenamiento local como fase activa, IndexedDB como fase pendiente, Supabase como fase pendiente y una futura ZIVA Network. El código revisado utilizaba localStorage; no se verificó una arquitectura de backend productiva.

El README afirma que no realiza llamadas externas, pero el código examinado contiene una consulta a un servicio externo de tipos de cambio. Se conserva esta discrepancia para revisión futura.

### 8.3 Seguridad y pruebas

En la versión revisada se observaron controles experimentales que no deben utilizarse como referencia de seguridad de producción, entre ellos PIN predeterminados y salt fijo en código; localStorage por sí solo no cifra los datos. No se ejecutaron pruebas de funcionamiento, seguridad, privacidad, recuperación ni resistencia a manipulación en el marco de esta reconstrucción.

Por tanto:
- no introducir datos financieros sensibles en esa beta;
- no declarar la aplicación segura, funcional, productiva ni verificada;
- no interpretar las pantallas de crédito como un sistema de otorgamiento real.

### 8.4 Otros repositorios con nombres BREGPersonal

- [BREGPersonal](https://github.com/lusdrey523/BREGPersonal): el contenido revisado corresponde a un artefacto ZivaOS Shield, no a la aplicación BREGPersonal buscada.
- [breg-personal](https://github.com/lusdrey523/breg-personal): el contenido revisado incluye documentos e identidad visual de Ruzhex, no la aplicación BREGPersonal.

El PDF histórico aportado por el fundador también utiliza en un pasaje la denominación “RREGPersonal”. El fundador indicó que podría tratarse de un error de escritura y confirmó BREGPersonal como nombre provisional correcto. La variante no debe tratarse como iniciativa distinta sin evidencia adicional.

## 9. Elementos no definidos o no validados

Al cerrar esta reconstrucción, se identifican expresamente como no definidos:
- si el indicador económico sería universal o adaptable por actividad;
- metodología formal, ponderaciones finales y validación estadística;
- tasas de interés, costo total y estructura de precios;
- límites de crédito y cálculo validado de capacidad de pago;
- política de riesgo, mora, provisiones, recuperación y sobreendeudamiento;
- modelo contractual y jurídico entre prestatario, prestamista, plataforma y proveedor;
- categorías de prestamistas y requisitos regulatorios específicos;
- alcance real de la participación de un proveedor como Global66;
- custodia, segregación, conciliación y protección de fondos;
- reglas de débito, pausas, consentimiento, reversas y fallas de pago;
- distribución contractual de comisiones, intereses y gastos;
- pruebas técnicas, auditorías y validación profesional.

No debe inventarse una decisión para completar estos vacíos. Son preguntas abiertas que podrían investigarse si el concepto se retomara, pero no son decisiones vigentes de ZivaLatam.

## 10. Estado histórico y relación con ZivaLatam

BREGPersonal debe conservarse como antecedente conceptual y experimental. Algunas de sus ideas —control del titular sobre sus datos, reconocimiento de actividad económica, evidencias de ingresos y evaluación complementaria— guardan relación temática con intereses posteriores de ZivaLatam.

Sin embargo, no se ha decidido que BREGPersonal sea un producto actual de ZivaLatam, que su código se reutilice, que sus componentes formen parte de ZivaID o ZivaPay, ni que el modelo de microfinanciamiento descrito vaya a desarrollarse. Cualquier reutilización futura requerirá evaluación independiente de viabilidad, seguridad, propiedad intelectual, regulación, arquitectura y estrategia.

## 11. Fuentes y trazabilidad

### Testimonio del fundador
- Reconstrucción progresiva realizada durante noviembre de 2026.
- Aclaraciones sobre el propósito original, el nicho de reciclaje, el modelo P2P, los prestamistas institucionales, el partner hipotético, las bóvedas y los pagos flexibles.

### Artefactos
- [Repositorio breg-personal-ziva](https://github.com/lusdrey523/breg-personal-ziva).
- [Repositorio BREGPersonal](https://github.com/lusdrey523/BREGPersonal).
- [Repositorio breg-personal](https://github.com/lusdrey523/breg-personal).
- [Archivo histórico mi historia.pdf](../../) — referencia descriptiva al archivo aportado en la conversación; su ubicación institucional y versión deberán asignarse si se incorpora al repositorio.

### Precaución sobre fechas
Las fechas de commits reflejan registros de Git. La beta BREGPersonal revisada presenta actividad registrada en 2026; esto no determina cuándo surgió originalmente la idea ni cuándo se elaboró cada requisito.

## 12. Documentos relacionados

- [Historia y evolución de la iniciativa: antecedentes de ZivaLatam](../../foundation/history-and-evolution.md)
- [Portal de conocimiento institucional](../../README.md)
- [Índice maestro](../../master-index.md)
- [Glosario institucional](../../glossary.md)

---

**Control de cambios:** esta versión 0.1 consolida el relato histórico del fundador y los artefactos de repositorio identificados hasta noviembre de 2026. No constituye una especificación vigente, una decisión de negocio aprobada ni una autorización para implementar el modelo.
