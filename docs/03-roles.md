# 3. Roles y permisos

[← Volver al índice](../README.md)

Cada usuario de Evidentia tiene uno o varios **roles**. El rol determina qué bloques del menú ves y qué puedes hacer. Los roles los asigna el profesorado o la presidencia desde **Gestionar alumnos** (ver [capítulo 8](08-presidencia-y-profesorado.md#gestionar-alumnos)).

## Los seis roles

| Rol | Quién lo tiene | Qué hace |
|---|---|---|
| **Estudiante** | Todo el alumnado de la asignatura | Registra sus evidencias, consulta sus reuniones y asistencias, firma hojas de asistencia y escribe su resumen de trabajo. |
| **Coordinador** | Una persona por comité | Revisa las evidencias dirigidas a **su** comité y las acepta o rechaza. |
| **Secretario** | Una persona por comité | Convoca reuniones de **su** comité, recoge firmas, levanta actas y registra bonos de horas. |
| **Coordinador de registro** | Una persona para todas las jornadas | Conecta Evidentia con Eventbrite y carga los eventos y las asistencias. |
| **Presidente** | La persona que preside las jornadas | Configura los plazos, gestiona alumnos, roles, comités, consulta todas las evidencias y reuniones, y exporta datos. |
| **Profesor** | El profesorado de la asignatura | Todo lo del presidente, más la importación de alumnos, la aleatorización de evidencias, la comprobación de integridad y el borrado masivo de usuarios. |

## Combinar roles

Una persona puede tener **varios roles a la vez**, y es lo habitual: quien coordina un comité o hace de secretario también es estudiante y necesita registrar sus propias evidencias.

- Para poder **crear evidencias** y ver *Mis evidencias*, *Mis reuniones* y *Mis asistencias* es necesario tener el rol **Estudiante**.
- Los roles **Coordinador** y **Secretario** exigen tener un **comité asociado**. Un coordinador o secretario solo actúa sobre su comité.
- El rol **Profesor** solo puede asignarlo otro profesor. La presidencia no ve las cuentas del profesorado ni puede otorgar ese rol.
- Las cuentas con rol Profesor no registran evidencias ni tienen resumen de trabajo.

## Qué ve cada rol en el menú

| Sección del menú | Estudiante | Coordinador | Secretario | Coord. registro | Presidente | Profesor |
|---|:-:|:-:|:-:|:-:|:-:|:-:|
| Dashboard y Mi perfil | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| Crear evidencia / Mis evidencias | ✔ | | | | | |
| Mis reuniones / Mis asistencias | ✔ | | | | | |
| Gestionar evidencias (de mi comité) | | ✔ | | | | |
| Gestionar reuniones, bonos y listas | | | ✔ | | | |
| Ajustes de Eventbrite, eventos y asistencias | | | | ✔ | | |
| Configurar curso | | | | | ✔ | ✔ |
| Gestionar alumnos / comités | | | | | ✔ | ✔ |
| Gestionar evidencias / reuniones (todas) | | | | | ✔ | ✔ |
| Exportaciones | | | | | ✔ | ✔ |
| Importaciones | | | | | | ✔ |
| Aleatorizar evidencias | | | | | | ✔ |
| Comprobar integridad | | | | | | ✔ |
| Actualizaciones, Buzón de sugerencias | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |

## Quién ve tus evidencias

| Estado de la evidencia | Tú | Coordinador de ese comité | Presidencia y profesorado |
|---|:-:|:-:|:-:|
| En borrador | ✔ | | |
| Pendiente, Aceptada o Rechazada | ✔ | ✔ | ✔ |

Los archivos adjuntos (pruebas) los pueden descargar las mismas personas que pueden ver la evidencia.

## Firmar asistencia a una reunión

Firmar en una hoja de firmas no requiere ningún rol especial: cualquier persona con cuenta en Evidentia puede firmar con su correo y contraseña desde el enlace que comparte el secretario. Ver [capítulo 4](04-estudiante.md#firmar-la-asistencia-a-una-reunión).
