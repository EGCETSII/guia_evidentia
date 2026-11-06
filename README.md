# Guía de uso de Evidentia

**Evidentia** ([evidentia.us.es](https://evidentia.us.es)) es la plataforma con la que se registra, valida y contabiliza el trabajo realizado por el alumnado en las **Jornadas InnoSoft Days**, organizadas en el marco de la asignatura *Evolución y Gestión de la Configuración* (EGC) de la ETSII, Universidad de Sevilla.

Esta guía está escrita para las personas que **usan** la aplicación: estudiantes, coordinadores y secretarios de comité, coordinador de registro, presidencia y profesorado. No es documentación técnica ni de despliegue.

> Guía correspondiente a la versión **4.0.1** de Evidentia.

## Índice

| Capítulo | Contenido |
|---|---|
| [1. Introducción y conceptos clave](docs/01-introduccion.md) | Qué es Evidentia, comités, evidencias, quién revisa cada una, horas computadas, plazos, integridad y trazabilidad |
| [2. Acceso, página de inicio y perfil](docs/02-acceso-y-perfil.md) | Primer acceso, contraseña, barra superior, menú lateral y móvil, página de inicio, *Mi perfil*, avisos, mensajes, *Mi actividad*, ayuda |
| [3. Roles y permisos](docs/03-roles.md) | Qué puede hacer cada rol y cómo se asignan |
| [4. Guía del estudiante](docs/04-estudiante.md) | Crear, publicar, corregir y cambiar de comité las evidencias; reuniones; asistencias; firmar asistencia; mensajes; resumen de trabajo |
| [5. Guía del coordinador de comité](docs/05-coordinador.md) | Revisar, aceptar, rechazar y mover evidencias; *Mi comité*; mensajes y avisos |
| [6. Guía del secretario de comité](docs/06-secretario.md) | Convocatorias, hojas de firmas, actas, bonos de horas y listas |
| [7. Guía del coordinador de registro](docs/07-coordinador-registro.md) | Eventos y asistencias con Eventbrite y eventos creados a mano |
| [8. Guía de presidencia y profesorado](docs/08-presidencia-y-profesorado.md) | Configurar el curso, alumnos, cola de revisión de presidencia, comités, evidencias, reuniones, registro de actividad, errores, importar y exportar |
| [9. Preguntas frecuentes](docs/09-preguntas-frecuentes.md) | Problemas habituales y cómo resolverlos |
| [10. Glosario](docs/10-glosario.md) | Términos y estados que aparecen en la aplicación |

## ¿Por dónde empiezo?

| Si eres... | Lee primero |
|---|---|
| Estudiante | [2. Acceso](docs/02-acceso-y-perfil.md) y [4. Guía del estudiante](docs/04-estudiante.md) |
| Coordinador/a de un comité | [4. Guía del estudiante](docs/04-estudiante.md) (para tus propias evidencias) y [5. Guía del coordinador](docs/05-coordinador.md) |
| Secretario/a de un comité | [6. Guía del secretario](docs/06-secretario.md) |
| Coordinador/a de registro | [7. Guía del coordinador de registro](docs/07-coordinador-registro.md) |
| Presidente/a de las jornadas | [8. Guía de presidencia y profesorado](docs/08-presidencia-y-profesorado.md) |
| Profesor/a | [1. Introducción](docs/01-introduccion.md) y [8. Guía de presidencia y profesorado](docs/08-presidencia-y-profesorado.md) |

## El flujo de trabajo en siete pasos

```mermaid
flowchart LR
    A[Profesorado<br>importa alumnos,<br>configura plazos<br>y comités] --> B[Presidencia<br>asigna roles<br>y comités]
    B --> C[Estudiantes<br>registran y publican<br>evidencias]
    C --> D[Coordinadores y presidencia<br>aceptan o rechazan<br>evidencias]
    B --> E[Secretarios<br>convocan reuniones,<br>recogen firmas,<br>levantan actas<br>y registran bonos]
    B --> F[Coordinador de registro<br>sincroniza eventos y<br>asistencias de Eventbrite]
    D --> G[Profesorado<br>exporta horas y<br>aleatoriza evidencias<br>para evaluar]
    E --> G
    F --> G
```

1. El **profesorado** importa el listado de alumnos, configura las fechas límite del curso y revisa los comités.
2. La **presidencia** (o el profesorado) asigna a cada persona sus roles y su comité.
3. Cada **estudiante** registra sus evidencias de trabajo, adjunta pruebas y las publica.
4. El **coordinador** de cada comité revisa las evidencias recibidas y las acepta o las rechaza indicando el motivo. Las evidencias de los propios coordinadores las revisa la **presidencia**.
5. El **secretario** de cada comité convoca las reuniones, recoge las firmas de asistencia, levanta acta y registra bonos de horas.
6. El **coordinador de registro** sincroniza los eventos y las asistencias desde Eventbrite.
7. Al cierre, el profesorado exporta las horas computadas de cada estudiante y selecciona al azar una evidencia por persona para su evaluación.

## Soporte

- Grupo de asistencia técnica en Telegram: [t.me/evidentia_sat](https://t.me/evidentia_sat)
- Dentro de la aplicación: enlace **Sugerencias** del pie de página, que abre un mensaje al profesorado (no es anónimo)
- Código fuente de Evidentia: [github.com/drorganvidez/evidentia](https://github.com/drorganvidez/evidentia) (licencia GNU GPL v3)
