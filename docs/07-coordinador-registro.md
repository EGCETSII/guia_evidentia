# 7. Guía del coordinador de registro

[← Volver al índice](../README.md)

El coordinador de registro mantiene en Evidentia los **eventos** de las jornadas (charlas, talleres, actividades) y las **asistencias** del alumnado. La fuente principal es **Eventbrite**, la plataforma en la que se publican los eventos y se hace el check-in de los asistentes. Los eventos celebrados antes de usar Eventbrite pueden crearse a mano.

Las horas de los eventos a los que un estudiante ha asistido se suman a su cómputo como horas de **Asistencia**, por lo que este registro afecta directamente a la evaluación.

Todo lo que necesitas está en el grupo **Asistencias y eventos** del menú lateral:

- **Eventbrite** (solo visible mientras el plazo de registro de eventos y asistencias esté abierto)
- **Eventos**
- **Asistencias**
- **Mensajes**

En el móvil, la barra inferior da acceso directo a **Eventos** y **Asistencias**.

## Paso 1: conectar con Eventbrite

Evidentia necesita un **token** de la API de Eventbrite para leer los eventos y las asistencias de la cuenta organizadora de las jornadas.

1. En Evidentia, abre **Eventbrite** y pulsa **Obtener el token**. Se abre la página de claves de la API de Eventbrite ([www.eventbrite.com/platform/api-keys](https://www.eventbrite.com/platform/api-keys)); inicia sesión con la cuenta que organiza los eventos.
2. Copia el **token privado** (*Private token*).
3. Vuelve a Evidentia, pégalo en el campo **Token** de la tarjeta *Token de la API* y pulsa **Validar y guardar**.

Evidentia comprueba el token antes de guardarlo. Si ves «Ups, parece que hay un problema con el token. Comprueba que es válido.», revisa que lo has copiado completo y que la cuenta tiene acceso a los eventos.

> El token da acceso a los datos de la cuenta de Eventbrite. No lo compartas.

## Paso 2: cargar los eventos

1. Abre **Eventos**.
2. Pulsa **Cargar desde Eventbrite**.

Evidentia descarga **todos los eventos** de las organizaciones asociadas al token y guarda su nombre, descripción, inicio y fin, capacidad, estado y enlace. Las **horas** de cada evento se calculan como la duración entre el inicio y el fin.

Puedes repetir la carga cuantas veces quieras: los eventos ya existentes se actualizan y los nuevos se añaden. Hazlo cada vez que se cree o modifique un evento en Eventbrite.

La tabla de eventos muestra las columnas **Evento**, **Fecha**, **Horas**, **Capacidad** y **Estado**. Puedes buscar, ordenar por columna y pasar de página. El estado es el que tiene el evento en Eventbrite:

| Estado | Significado |
|---|---|
| En borrador | El evento aún no está publicado en Eventbrite. |
| Publicado | Publicado y con inscripciones abiertas. |
| En curso | El evento está celebrándose. |
| Finalizado / Completado | El evento ya ha terminado. |
| Cancelado | El evento se canceló. |

### Crear eventos a mano

Para las sesiones que se celebraron antes de usar Eventbrite, pulsa **Nuevo evento** y rellena la tarjeta *Datos del evento*:

| Campo | Regla |
|---|---|
| **Nombre** | Obligatorio, hasta 255 caracteres. |
| **Inicio** y **Fin** | Obligatorios. El fin debe ser posterior al inicio. |
| **Capacidad** | Opcional, un número entero (0 o más). |
| **Descripción** | Opcional, hasta 5000 caracteres. |

Pulsa **Crear evento**. Las horas se calculan con la duración y el estado se pone solo: *Completado* si el fin ya pasó y *Publicado* si no. Estos eventos llevan la etiqueta *Creado a mano* y en su fila tienes:

- **Añadir una asistencia**, que abre el formulario de asistencia con el evento ya elegido.
- **Editar**, para cambiar sus datos (**Guardar evento**).
- **Borrar el evento**, que pide confirmación (**Sí, borrar**). Un evento con asistencias no se puede borrar; borra antes sus asistencias.

### Ocultar eventos

Los eventos aparecen en el panel de inicio de todos los usuarios (tarjeta **Eventos**). Si alguno no debe mostrarse (pruebas, eventos internos, cancelados...), pulsa **Ocultar** en su fila. Los eventos ocultos llevan la etiqueta *Oculto*, siguen en tu lista de *Eventos* y puedes volver a **Mostrarlos** cuando quieras.

## Paso 3: cargar las asistencias

Para cada evento de Eventbrite, cuando ya se haya celebrado (o cuando quieras actualizar las inscripciones):

1. En **Eventos**, pulsa el botón de descarga **Cargar las asistencias** de la fila del evento.
2. Evidentia descarga la lista de asistentes de Eventbrite y la empareja con las cuentas de Evidentia.

Cómo se hace el emparejamiento:

- Primero se busca un usuario con el mismo **correo electrónico** que la inscripción (sin distinguir mayúsculas).
- Si no lo hay, se busca por **nombre y apellidos** (ignorando mayúsculas, tildes y signos), pero solo si coincide exactamente **una** cuenta.
- Si tampoco así hay una única coincidencia, la inscripción **se ignora** (no se crea nada).

Para cada persona emparejada se guarda su **estado de asistencia** tal como figura en Eventbrite. Si ya existía, se actualiza. Los estados posibles son:

| Estado en Evidentia | Estado en Eventbrite | ¿Suma horas? |
|---|---|:-:|
| Pendiente de asistir | Attending | No |
| Pendiente de asistir (invitado) | Guests Attending | No |
| **Asistido** | **Checked In** | **Sí** |
| Asistido (invitado) | Guests Attended | No |
| No asistido | Not Attending | No |
| Asistencia cancelada | Not Attending (Refunded/Canceled) | No |

> Solo el estado **Asistido** (check-in realizado en Eventbrite) suma las horas del evento al estudiante. Asegúrate de que en cada evento se hace el check-in de los asistentes y **vuelve a cargar las asistencias después del evento**.

Repite la carga tantas veces como necesites; es una operación segura.

## Asistencias

**Asistencias** muestra todas las asistencias registradas con las columnas **Estudiante**, **Evento**, **Fecha** y **Asistencia**. Puedes buscar, ordenar y pasar de página. Desde aquí puedes:

- **Exportar** las asistencias a un archivo Excel.
- **Añadir asistencia** a mano: elige el **Estudiante**, el **Evento** y la **Asistencia** (*Asistido* o *No asistido*) y pulsa **Crear asistencia**. Sirve cuando alguien asistió pero no se emparejó con Eventbrite (por ejemplo, se inscribió con otro nombre y otro correo) o para los eventos creados a mano. No puede haber dos asistencias de la misma persona al mismo evento.
- **Editar** una asistencia (pulsando su fila): cambiar el estudiante, el evento o el estado y pulsar **Guardar cambios**.
- **Eliminar** una asistencia desde su página de edición (pide confirmación, **Sí, eliminar**).

No puedes registrar ni editar tu propia asistencia: el intento queda anotado en el registro de actividad.

> Si vuelves a cargar las asistencias de un evento, el estado de las personas emparejadas se sobrescribe con el de Eventbrite. Las asistencias añadidas a mano para personas que no están en Eventbrite no se ven afectadas.

Todo lo que haces aquí (guardar el token, cargar eventos y asistencias, ocultar, crear, editar, borrar y exportar) queda anotado en el registro de actividad.

## Recomendaciones para el alumnado

Recuérdales estas dos cosas antes de los eventos; evitarán la mayoría de incidencias:

1. Inscribirse en Eventbrite con **el mismo correo** que tienen en Evidentia (o, al menos, con el mismo nombre y apellidos).
2. Pasar por el **check-in** al llegar al evento.

## Plazo que te afecta

| Plazo | Efecto |
|---|---|
| **Registro de eventos y asistencias** | Cuando vence, desaparece *Eventbrite* y ya no puedes cargar eventos ni asistencias, ocultar o mostrar eventos, crear o editar eventos ni añadir, editar o eliminar asistencias. Sigues viendo las listas y puedes exportar. |

## Lista de comprobación

- [ ] El token de Eventbrite está validado.
- [ ] Todos los eventos de las jornadas están cargados (o creados a mano) y los que no procede mostrar están ocultos.
- [ ] Tras cada evento he vuelto a cargar sus asistencias.
- [ ] He resuelto a mano las asistencias de quienes no se emparejaron.
- [ ] Todo está registrado antes de que venza el plazo.
