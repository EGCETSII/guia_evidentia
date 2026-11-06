# 3. Roles y permisos

[← Volver al índice](../README.md)

Cada usuario de Evidentia tiene uno o varios **roles**. El rol determina qué bloques del menú ves y qué puedes hacer. Los roles los asigna el profesorado o la presidencia desde **Gestión → Alumnos** (ver [capítulo 8](08-presidencia-y-profesorado.md)).

## Los seis roles

| Rol | Quién lo tiene | Qué hace |
|---|---|---|
| **Estudiante** | Todo el alumnado de la asignatura | Registra sus evidencias, consulta sus reuniones y asistencias, firma hojas de asistencia y escribe su resumen de trabajo. |
| **Coordinador** | La coordinación de cada comité | Revisa las evidencias dirigidas a **su** comité y las acepta o rechaza, y organiza su comité desde *Mi comité*. |
| **Secretario** | La secretaría de cada comité | Convoca reuniones de **su** comité, recoge firmas, levanta actas y registra bonos de horas. |
| **Coordinador de registro** | Una persona para todas las jornadas | Conecta Evidentia con Eventbrite y carga los eventos y las asistencias, o los crea a mano. |
| **Presidente** | La presidencia de las jornadas | Revisa las evidencias de la presidencia, configura los plazos, gestiona alumnos, roles y comités, consulta todas las evidencias, reuniones, asistencias y bonos, comprueba la integridad, revisa los errores y exporta datos. |
| **Profesor** | El profesorado de la asignatura | Todo lo de gestión del presidente, más la importación de alumnos, el borrado masivo de usuarios y la aleatorización de evidencias. |

## Combinar roles

Una persona puede tener **varios roles a la vez**, y es lo habitual: quien coordina un comité o hace de secretario también es estudiante.

- Todos los roles salvo el de Profesor registran sus propias evidencias desde **Mis cosas**. *Mis asistencias* solo aparece con el rol **Estudiante**.
- Los roles **Coordinador** y **Secretario** exigen tener un **comité asociado**. Un coordinador o secretario solo actúa sobre su comité.
- El rol **Profesor** solo puede asignarlo otro profesor. La presidencia no ve las cuentas del profesorado ni puede otorgar ese rol.
- Las cuentas con rol Profesor no registran evidencias ni tienen resumen de trabajo.

## Qué ve cada rol en el menú

| Opción del menú | Estudiante | Coordinador | Secretario | Coord. registro | Presidente | Profesor |
|---|:-:|:-:|:-:|:-:|:-:|:-:|
| Inicio, Mi perfil, Mis mensajes, Mi actividad | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| Nueva evidencia, Mis evidencias, Mis reuniones | ✔ | ✔ | ✔ | ✔ | ✔ | |
| Mis asistencias | ✔ | | | | | |
| Mi comité, Revisar evidencias (de mi comité) | | ✔ | | | | |
| Reuniones, Bonos, Listas (de mi comité) | | | ✔ | | | |
| Mensajes (bandeja de entrada) | | ✔ | ✔ | ✔ | ✔ | ✔ |
| Actividad del comité | | ✔ | ✔ | | | |
| Eventbrite, Eventos, Asistencias | | | | ✔ | | |
| Revisar evidencias (de la presidencia) | | | | | ✔ | |
| Configurar curso, Alumnos, Comités | | | | | ✔ | ✔ |
| Evidencias, Reuniones, Asistencias, Bonos (todos) | | | | | ✔ | ✔ |
| Integridad, Exportar, Registro de actividad, Errores | | | | | ✔ | ✔ |
| Importar | | | | | | ✔ |
| Aleatorizar | | | | | | ✔ |

Una persona con varios roles ve la suma de sus columnas.

## Quién revisa cada evidencia

- El **coordinador** de un comité revisa las evidencias dirigidas a ese comité.
- Las evidencias que un coordinador dirige a **su propio** comité, y las dirigidas al comité **Presidencia**, las revisa la **presidencia** desde *Gestión → Revisar evidencias*.
- Las evidencias de un **presidente** quedan aceptadas en cuanto se publican.
- **Nadie puede revisar su propia evidencia.**
- El profesorado puede revisar cualquier evidencia, aunque no tiene cola de revisión propia.

## Quién ve tus evidencias

| Estado de la evidencia | Tú | Quien la revisa | Presidencia y profesorado |
|---|:-:|:-:|:-:|
| Borrador | ✔ | | |
| Pendiente, Aceptada o Rechazada | ✔ | ✔ | ✔ |

Los archivos adjuntos (pruebas) los pueden descargar las mismas personas que pueden ver la evidencia.

## Firmar asistencia a una reunión

Firmar en una hoja de firmas no requiere ningún rol especial: cualquier persona con cuenta en Evidentia puede firmar con su correo y contraseña desde el enlace que comparte el secretario. Ver [capítulo 4](04-estudiante.md#firmar-la-asistencia-a-una-reunión).
