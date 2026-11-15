# 00 · Documento de inicio del proyecto

> **Plantilla.** Se rellena **en la sesión de Inicio (6-nov-2026)** y se afina hasta el **12-nov**, donde el tutor aprueba la propuesta. Es breve: una página. Si algo no lo sabes todavía, escribe «pendiente» y por qué. Borra las notas en cursiva al rellenar.
>
> **No escribas datos personales sensibles** (teléfono, dirección, DNI) ni tu correo personal.

## 1. Datos del alumno/a

| | |
|---|---|
| **Nombre y apellidos** | Jhonatan Stiven Albarracin Agudelo |
| **Usuario de GitHub** | jhonatan-albarracin |
| **Repositorio del proyecto** | *[github.com/jhonatan-albarracin/proyectoDWES](https://github.com/jhonatan-albarracin/proyectoDWES)* |
| **Ciclo y curso** | DAW, 2.º · curso 2026-27 |
| **Fecha** | 2026-11-12 |

## 2. Nombre del proyecto

miCita

Plataforma para pequeños empresarios la cual ayuda a gestionar tanto las citas de una empresa como sus reservas para la prestacion de sus servicios.

## 3. Qué quiero hacer

La plataforma será un entorno digital diseñado para otorgar al empresario el control total sobre la gestión de su tiempo y la disponibilidad de sus servicios.

Su principal objetivo será permitir que cada empresario pueda definir, personalizar y establecer los horarios que mejor se adapten a sus necesidades, para posteriormente ponerlos a disposición de sus clientes de una manera organizada y controlada.

El núcleo de la plataforma será un calendario inteligente y personalizable, cuyo funcionamiento se adaptará a las características, preferencias y necesidades particulares de cada negocio. A través de este calendario, los clientes podrán consultar la disponibilidad del empresario e interactuar con ella de forma sencilla, intuitiva y práctica, facilitando así la contratación y reserva de sus servicios.

Más allá de ser una herramienta de gestión de citas, la plataforma busca ofrecer un modelo de organización del tiempo que permita al empresario mantener el control sobre su actividad profesional, establecer límites en su disponibilidad y alcanzar un equilibrio saludable entre su vida laboral y su tiempo personal.

En definitiva, se trata de transformar la gestión del tiempo en una herramienta flexible, personalizada y centrada en las necesidades del empresario, sin dejar de ofrecer una experiencia cómoda y accesible para sus clientes.

## 4. Qué problema o necesidad resuelve

Los trabajadores por cuenta propia y los pequeños empresarios de servicios gestionan sus citas y reservas de forma manual o dispersa (WhatsApp, teléfono, papel). Eso les quita tiempo de su actividad, genera solapamientos y ausencias sin aviso, y dificulta poner límites a su disponibilidad. El resultado es un desbalance entre el tiempo de trabajo y el tiempo personal.

miCita responde a esta necesidad dando al empresario un calendario propio, personalizable y de control total, que pone a disposición de sus clientes solo los horarios que él elige.

Esta necesidad la he visto y vivido de cerca. Mi madre fue autónoma durante una temporada, prestando servicio de manicura mediante citas y reservas. Después de trabajar, tenía que seguir trabajando pegada al teléfono recordando y agendando más citas, sin contar las que cancelan a última hora. Eso le causaba un desgaste mayor y le robaba tiempo de calidad por tener que trabajar de más.

También conozco el caso de mi tía, que hace limpiezas a domicilio en Suiza. Para ella es necesaria la gestión de un calendario adaptado a las regiones geográficas donde presta el servicio, no solo un gestor simple, porque no puede acudir si la distancia entre ubicaciones es elevada y el transporte corre por su cuenta.

Además, he podido observar esta misma situación en muchas otras personas con las que interactúo en el día a día.

Se desarrolla con detalle en [`01-analisis.md`](01-analisis.md), apartado 2 (Necesidades y oportunidades).

## 5. Para quién

**Quién lo usa**

- **Autónomos que trabajan solos** (manicura, limpiezas a domicilio, fisioterapia, clases particulares, consultoría…): gestionan su propia agenda, citas y disponibilidad sin depender de llamadas ni WhatsApp.
- **Pequeños empresarios con poco personal** (unos 2 a 5 trabajadores): el empresario controla los horarios de cada trabajador y decide cómo se reparten las citas entre ellos.

**Contexto de uso**

Es un uso profesional y comercial dentro de su negocio. El empresario define sus horarios de trabajo, bloques, descansos y días de disponibilidad. A partir de ahí:

- El **cliente** consulta la disponibilidad y reserva una cita. Puede elegir a un trabajador concreto o dejar que el sistema asigne uno.
- Si el cliente **no elige trabajador**, el empresario (o el propio trabajador) asigna la cita a quien tenga hueco.
- Si un trabajador ya tiene su cupo lleno ese día u horario, **no se muestra como disponible** para el cliente. Así el trabajo se reparte entre el equipo y no se acumulan todas las citas con una sola persona.

El cliente usa la plataforma como canal de reserva de servicios; el empresario la usa para organizar su tiempo y poner límites a su disponibilidad.

**Campo de mejora a futuro (no parte de la primera versión)**

Más adelante se podría expandir a otros tipos de usuarios, como redes de profesionales independientes, asociaciones de autónomos o pequeños grupos que compartan una marca común sin que nadie sea jefe de nadie. En ese caso cada uno seguiría gestionando su propio calendario y sus citas, pero compartirían la plataforma de reservas y la captación de clientes. Esta expansión queda fuera del alcance inicial y se plantea solo como una posible evolución del proyecto.

## 6. Funcionalidades principales

*Lista de 3 a 6 cosas que debe hacer. Marca cuáles son imprescindibles para una **primera versión mínima** (la que quieres tener funcionando antes del 31-mar).*

| # | Funcionalidad | ¿Imprescindible? (sí / no) |
|---|---|---|
| 1 | Configuración del calendario del empresario: horarios de trabajo, bloques, descansos, días festivos y límite diario de citas | sí |
| 2 | Gestión de citas: crear, editar y cancelar citas desde el panel del empresario | sí |
| 3 | Página pública de disponibilidad: el cliente consulta horarios libres y reserva una cita | sí |
| 4 | Distribución de citas entre trabajadores: si el cliente no elige a alguien específico, el sistema asigna la cita a quien tenga hueco y no muestra como disponible a quien ya está lleno | sí |
| 5 | Historial de clientes y servicios prestados | no |
| 6 | Recordatorios automáticos de cita (por ejemplo, por correo o SMS) | no |

## 7. Tecnologías previstas

*Lenguajes, frameworks, base de datos, despliegue... Y cuáles ya conoces y cuáles tendrás que aprender.*

| Tecnología | Para qué | Nivel actual (nada / media / bien) |
|---|---|---|
| HTML | Estructura de las páginas web | media |
| CSS | Diseño y maquetación de la interfaz | media |
| JavaScript | Interactividad en el cliente (calendario, formularios, reserva) | media |
| Java | Lógica del servidor y backend de la aplicación | media |
| Spring Boot | Framework Java para crear la API y servicios del backend | nada |
| SQL (MySQL / PostgreSQL) | Base de datos para usuarios, citas, trabajadores y disponibilidad | media |
| Git y GitHub | Control de versiones y repositorio del proyecto | media |
| Despliegue (servidor en la nube o similar) | Publicar la aplicación para que esté accesible por internet | nada |

## 8. Dónde se integra con los módulos de 2.º

*Marca los módulos de 2.º cuyos contenidos usarás de forma real en el proyecto (debe haber **al menos tres**).*

- [x] Desarrollo web en entorno cliente (0612): HTML, CSS y JavaScript para la interfaz, el calendario y la reserva desde el navegador.
- [x] Desarrollo web en entorno servidor (0613): Java y Spring Boot para la API, la lógica de citas y la conexión con la base de datos.
- [x] Despliegue de aplicaciones web (0614): publicación de la aplicación en un servidor en la nube para que esté accesible por internet.
- [x] Diseño de interfaces web (0615): maquetación con CSS y diseño de la experiencia de reserva para empresarios y clientes.

## 9. Datos y empresas

- ¿El proyecto parte de una **empresa** (por ejemplo, de tus prácticas)? **No**. Se plantea como un encargo simulado.
- ¿Usará **datos personales reales**? **No**. Se usarán datos de ejemplo.

## 10. Riesgos y dudas iniciales

**Riesgos**

- **Tiempo:** compaginar el desarrollo del proyecto con las asignaturas de 2.º de DAW y las entregas del tutor (H1, H2, H3) puede ajustar mucho los plazos, especialmente si surgen imprevistos en alguna parte del proyecto.
- **Tecnología:** Spring Boot y SQL (MySQL/PostgreSQL) los marcas con nivel "nada", por lo que hay una curva de aprendizaje inicial que puede retrasar el backend y la base de datos.
- **Alcance:** la lógica de distribución automática de citas entre varios trabajadores y el control de disponibilidad (bloques, descansos, límite diario) puede resultar más compleja de lo que parece al principio.
- **Despliegue:** nunca he desplegado una aplicación en un servidor en la nube, por lo que esa parte puede generar imprevistos técnicos cerca de las entregas.

**Dudas iniciales**

- ¿Cómo gestionar que dos clientes no reserven la misma hora con el mismo trabajador al mismo tiempo?
- ¿Qué tan personalizable debe ser el calendario en la primera versión mínima sin que se dispare el tiempo de desarrollo?
- ¿Es suficiente con una base de datos relacional (SQL) para todo, o hará falta algo más adelante para el calendario?

## 11. Qué espero aprender

Espero aprender a desarrollar una aplicación web completa con Java y Spring Boot, desde la base de datos hasta la interfaz, y a desplegarla en un servidor para que sea accesible por internet.

---

## Aprobación del tutor

*Esta parte la rellena el tutor.*

| Criterio mínimo | Cumple |
|---|---|
| Necesidad real y documentada | ☐ |
| Alcance abordable en el tiempo disponible | ☐ |
| Integra contenidos de al menos tres módulos de 2.º | ☐ |
| No usa datos personales reales | ☐ |

**Estado:** ☐ Aprobada · ☐ Aprobada con cambios · ☐ Necesita rehacerse

**Fecha:** 

**Comentarios del tutor:**
