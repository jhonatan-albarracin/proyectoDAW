# 01b · Estado del arte (SOTA) de mi proyecto

> **Plantilla.** En **H1 (26-nov-2026)** entregas una **versión breve** (2-3 páginas: apartados **1, 2 y 5**), junto al `01-analisis.md`. Los apartados 3, 4, 6, 7 y 8 se completan en **H2 (21-ene-2027)** hasta las **4-6 páginas** del documento final. Aquí estudias qué soluciones, **modelos de negocio** y **herramientas** existen ya para el problema que has elegido, y justificas tus decisiones con ello. Cada apartado indica el criterio de evaluación (CE) que alimenta. Borra los bloques «Guía» al rellenar.

> **Guía.** Calendario de H1: **ciclo 1, hasta el jueves 19-nov:** preguntas de búsqueda y tabla de soluciones (apartados 1 y 2) · **ciclo 2, hasta el jueves 26-nov:** hueco y diferenciación (apartado 5). Los apartados 3, 4, 6, 7 y 8 son de H2.
>
> **Reglas.**
>
> - Solo cuenta lo que tiene **enlace y fecha de acceso**.
> - Si usas IA para buscar, **abre cada fuente** y comprueba que existe y dice lo que te cuenta la IA. Puede inventar productos, precios o referencias. Anótalo en `asistenciaIA/bitacora.md`.
> - Usa **solo información pública** de las soluciones que estudias. **Nada** de la empresa de prácticas ni de clientes reales.
> - Compara herramientas con **los mismos criterios**, no por opinión. Salvo razón argumentada, prefiere lo que has visto en el ciclo (Java 21, Spring Boot, SQL).
> - Si algo no lo has podido comprobar, dilo en el apartado 8.

## 1. Problema y preguntas de búsqueda (CE 1c)

**Problema:** Los trabajadores por cuenta propia y los pequeños empresarios de servicios gestionan sus citas y reservas de forma manual o dispersa (llamadas, WhatsApp, papel), lo que les quita tiempo de su actividad, genera solapamientos y ausencias sin aviso y dificulta poner límites a su disponibilidad.

| # | Pregunta | Dónde busqué | Fecha |
|---|---|---|---|
| P1 | ¿Qué soluciones existen para gestionar citas y reservas online y para qué tipo de negocio? | Webs y catálogos de software de reservas: Setmore, Square Appointments, SimplyBook.me, Eskedula, Booksy y Fresha (apartado 1.1 de `01-analisis.md`) | 2026-11-15 |
| P2 | ¿Qué modelos de precio utilizan esas soluciones y cómo ganan dinero? | Páginas de productos y planes de precios de las seis soluciones anteriores | 2026-11-15 |
| P3 | ¿Qué necesidades son más demandadas por el colectivo y con qué criterio se priorizan? | MITES (Estadística de autónomos, abril 2026), UPTA (informe del primer semestre de 2026 y estudio de racionalización de tiempos del autónomo, 2021) y experiencia directa (punto 4 de `00-documentoInicio.md`) | 2026-11-15 |
| P4 | ¿Qué alternativas no digitales se usan hoy y por qué no resuelven el problema? | Experiencia directa (casos familiares y observación del entorno) recogida en `00-documentoInicio.md` y en el apartado 3 de `01-analisis.md` | 2026-11-15 |
| P5 | ¿Existe mercado suficiente para una herramienta de gestión de citas? | Fortune Business Insights, informe *Appointment Scheduling Software Market* (fuente F4 de `01-analisis.md`) | 2026-11-15 |

## 2. Soluciones existentes (CE 1a, 1c, 2a)

| Solución | Para quién | Qué hace | Modelo de precio | Enlace y fecha de acceso | Estado (`leído` / `sin leer`) |
|---|---|---|---|---|---|
| **Setmore** | Autónomos y pequeñas empresas de servicios en general | Software de programación de citas online con página de reserva pública, recordatorios, pagos y sincronización de calendarios | Suscripción (freemium: plan gratuito y plan de pago) | [setmore.com](https://www.setmore.com/) · 2026-11-15 | `leído` |
| **Square Appointments** | Negocios de servicios que también cobran y gestionan TPV (multinacional) | Sistema de reservas todo en uno: agenda, disponibilidad del personal, pagos, recordatorios y TPV | Suscripción + comisión por transacción | [squareup.com/us/en/appointments](https://squareup.com/us/en/appointments) · 2026-11-15 | `leído` |
| **SimplyBook.me** | Negocios de servicios de todos los tamaños, incluidos servicios profesionales | Software de reservas online con página propia, widgets, notificaciones por WhatsApp/SMS/email e integraciones | Suscripción por niveles | [simplybook.me](https://simplybook.me/) · 2026-11-15 | `leído` |
| **Eskedula** | PYME española de belleza, bienestar, estética y fisioterapia | Gestión de reservas, agenda por profesional, clientes, TPV y facturación; sin marketplace ni comisión por reserva | Suscripción / licencia | [eskedula.es](https://www.eskedula.es/) · 2026-11-15 | `leído` |
| **Booksy** | Profesionales y negocios de belleza, bienestar y salud | Marketplace y software de reservas con perfil público, recordatorios, pagos y herramientas de captación de clientes | Suscripción + comisión por reserva | [booksy.com/biz](https://booksy.com/biz/en-us) · 2026-11-15 | `leído` |
| **Fresha** | Negocios de belleza y bienestar (salones, spas, barberías, masajes) | Software de reservas y pagos con calendario, recordatorios y marketplace para captar clientes | Comisión por transacción + suscripción premium | [fresha.com/for-business](https://www.fresha.com/for-business) · 2026-11-15 | `leído` |
| **Hoja de cálculo / agenda de papel** (alternativa no digital) | Autónomos y pequeños negocios que hoy gestionan las citas a mano | Anotar citas, horarios y reservas en papel o en una hoja de cálculo, sin página pública de reserva | Sin coste de software; el coste es el tiempo invertido | no aplica · 2026-11-15 (sin enlace: experiencia directa documentada en `00-documentoInicio.md`) | `leído` |

## 3. Modelos de negocio (CE 1d, 1e)

> **Pendiente.** Se completa en H2 (21-ene-2027).

*Qué **patrones** se repiten en las soluciones del apartado 2 (suscripción, *freemium*, comisión por operación, licencia, publicidad, servicio gratuito o público) y por qué. Describe con un **Business Model Canvas** (opcional; el profesor te da el material) **2-3 casos**. Termina con el modelo que seguiría **tu** proyecto, o qué ahorra o mejora si no es un negocio.*

| Patrón | Soluciones que lo usan | Ventaja | Riesgo |
|---|---|---|---|
| [RELLENAR] | | | |

## 4. Herramientas y tecnologías (CE 2a, 2b)

> **Pendiente.** Se completa en H2 (21-ene-2027).

*Para cada decisión técnica importante (lenguaje y *framework*, base de datos, despliegue, autenticación…), compara **2-3 opciones con los mismos criterios**. Marca la que eliges.*

| Decisión | Opción | Madurez | Licencia | Coste | Curva de aprendizaje | Encaje con el ciclo | Elegida |
|---|---|---|---|---|---|---|---|
| [RELLENAR: p. ej. base de datos] | | | | | | | |

*Cada decisión importante se convierte en una decisión registrada en `decisiones/` (la plantilla llega con el bloque de H2).*

## 5. Hueco y diferenciación (CE 1e)

Las soluciones del apartado 2 resuelven bien la reserva online, pero son genéricas u operativas: optimizan la agenda, los pagos y la captación de clientes, y no ponen el énfasis en que el empresario **controle su propio tiempo** ni en el equilibrio vida-laboral. Incluso las que más se acercan (Eskedula, con reservas propias sin marketplace) van dirigidas a un negocio con TPV, facturación y equipo completo.

miCita se centra en un segmento más concreto: el autónomo solo o el pequeño negocio con poquito personal que quiere un calendario personalizable (bloques, descansos, días no laborables y límite diario de citas) y publicar **solo** los horarios que él elige. Añade además la asignación automática entre trabajadores que evita concentrar todas las citas en una sola persona y deja de mostrar como disponible a quien ya tiene el cupo lleno.

Hay que ser honesto: para un salón que necesite cobrar en el local, emitir facturas, gestionar bonos o captar clientes mediante un marketplace, soluciones como Fresha, Booksy o Eskedula son más completas y miCita no pretende sustituirlas. El hueco está en el empresario que prioriza la simplicidad y el control de su disponibilidad por encima de esas funciones.

## 6. Decisiones derivadas (CE 1e, 1f, 2b)

> **Pendiente.** Se completa en H2 (21-ene-2027).

*Qué consecuencias tiene este estudio en tu proyecto.*

- **Tipo de proyecto elegido** (enlaza con el apartado 3 de [`01-analisis.md`](01-analisis.md)): [RELLENAR]
- **Requisitos que salen del estudio** (con su ID del apartado 4 de `01-analisis.md`): [RELLENAR]
- **Decisiones técnicas** (enlace a cada archivo de `decisiones/`): [RELLENAR]

## 7. Fuentes y calidad (CE 2a)

> **Pendiente.** Se completa en H2 (21-ene-2027).

*Al menos **2 fuentes independientes** (no dos páginas de la misma empresa). Datos oficiales o primarios antes que blogs.*

| # | Fuente (enlace) | Tipo | Fecha de acceso | Fiabilidad (alta / media / baja) y por qué |
|---|---|---|---|---|
| F1 | [RELLENAR] | | | |

## 8. Límites

> **Pendiente.** Se completa en H2 (21-ene-2027).

*Qué **no pudiste comprobar** y qué datos son estimaciones. Una lista corta y honesta es mejor que fingir certeza.*

- [RELLENAR]

---

## Criterios de evaluación que alimenta este documento (texto literal)

- **1a)** Se han clasificado las empresas del sector por sus características organizativas y el tipo de producto o servicio que ofrecen.
- **1c)** Se han identificado las necesidades más demandadas a las empresas.
- **1d)** Se han valorado las oportunidades de negocio previsibles en el sector.
- **1e)** Se ha identificado el tipo de proyecto requerido para dar respuesta a las demandas previstas.
- **1f)** Se han determinado las características específicas requeridas al proyecto.
- **2a)** Se ha recopilado información relativa a los aspectos que van a ser tratados en el proyecto.
- **2b)** Se ha realizado el estudio de viabilidad técnica del mismo.

> El SOTA **no añade criterios de evaluación**: reúne en un solo sitio lo que 1a-1f y 2a-2b ya piden. La evaluación sigue las listas de cotejo de H1 y H2.
