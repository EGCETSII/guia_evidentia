# 7. Guía del coordinador de registro

[← Volver al índice](../README.md)

El coordinador de registro es la persona que mantiene sincronizados en Evidentia los **eventos** de las jornadas (charlas, talleres, actividades) y las **asistencias** del alumnado. La fuente de estos datos es **Eventbrite**, la plataforma en la que se publican los eventos y se hace el check-in de los asistentes.

Las horas de los eventos a los que un estudiante ha asistido se suman a su cómputo como *horas en eventos*, por lo que esta sincronización afecta directamente a la evaluación.

Todo lo que necesitas está en el bloque **ASISTENCIAS Y EVENTOS** del menú lateral:

- **Ajustes de Eventbrite** (solo visible mientras el plazo de importación esté abierto)
- **Gestionar eventos**
- **Gestionar asistencias**

## Paso 1: conectar con Eventbrite

Evidentia necesita un **token** de la API de Eventbrite para leer los eventos y las asistencias de la cuenta organizadora de las jornadas.

1. Inicia sesión en Eventbrite con la cuenta que organiza los eventos y ve a [www.eventbrite.com/platform/api-keys](https://www.eventbrite.com/platform/api-keys).
2. Copia el **token privado** (*Private token*) de la API.
3. En Evidentia, abre **Ajustes de Eventbrite**, pega el token y pulsa **Validar y guardar token**.

Evidentia comprueba que el token es válido antes de guardarlo. Si aparece un error, revisa que lo has copiado completo y que la cuenta tiene acceso a los eventos.

> El token da acceso a los datos de la cuenta de Eventbrite. No lo compartas.

## Paso 2: cargar los eventos

1. Abre **Gestionar eventos**.
2. Pulsa **Cargar eventos desde Eventbrite**.

Evidentia descarga **todos los eventos** de las organizaciones asociadas al token y los guarda con su nombre, descripción, fecha de inicio y fin, capacidad, estado y enlace. Las **horas** de cada evento se calculan automáticamente como la duración entre la hora de inicio y la de fin.

Puedes repetir la carga cuantas veces quieras: los eventos ya existentes se actualizan y los nuevos se añaden. Hazlo cada vez que se cree o modifique un evento en Eventbrite.

La tabla de eventos muestra su **estado** en Eventbrite:

| Estado | Significado |
|---|---|
| En borrador | El evento aún no está publicado en Eventbrite. |
| Pendiente | Publicado y con inscripciones abiertas (*live*). |
| En curso | El evento está celebrándose. |
| Finalizado / Completado | El evento ya ha terminado. |
| Cancelado | El evento se canceló. |

### Ocultar eventos

Todos los eventos cargados aparecen en el panel principal de todos los usuarios (bloque **Eventos programados**). Si hay eventos que no deben mostrarse (pruebas, eventos internos, cancelados...), pulsa el botón de **ocultar** en su fila. Los eventos ocultos se marcan con la etiqueta *Oculto*, siguen visibles para ti en *Gestionar eventos* y puedes volver a **mostrarlos** cuando quieras.

## Paso 3: cargar las asistencias

Para cada evento, cuando ya se haya celebrado (o cuando quieras actualizar las inscripciones):

1. En **Gestionar eventos**, pulsa el botón **Cargar asistencia** de la fila del evento.
2. Evidentia descarga la lista de asistentes de Eventbrite y la empareja con las cuentas de Evidentia.

Cómo se hace el emparejamiento:

- Primero se busca un usuario cuyo **nombre y apellidos** coincidan con los de la inscripción en Eventbrite (ignorando mayúsculas, tildes y signos).
- Si no hay coincidencia, se busca por **correo electrónico**.
- Si tampoco coincide, la inscripción **se ignora** (no se crea nada).

Para cada persona emparejada se guarda su **estado de asistencia** tal como figura en Eventbrite. Si ya existía, se actualiza. Los estados posibles son:

| Estado en Evidentia | Estado en Eventbrite | ¿Suma horas? |
|---|---|:-:|
| Pendiente de asistir | Attending | No |
| **Asistido** | **Checked In** | **Sí** |
| Asistido (invitado) | Guests Attended | No |
| Pendiente de asistir (invitado) | Guests Attending | No |
| No asistido | Not Attending | No |
| Asistencia cancelada | Not Attending (Refunded/Canceled) | No |

> Solo el estado **Asistido** (check-in realizado en Eventbrite) suma las horas del evento al estudiante. Asegúrate de que en cada evento se hace el check-in de los asistentes y **vuelve a cargar la asistencia después del evento**.

Repite la carga tantas veces como necesites; es una operación segura.

## Gestionar asistencias

**Gestionar asistencias** muestra todas las asistencias registradas: alumna/o, evento y estado. Desde aquí puedes:

- **Exportar asistencias** a un archivo Excel.
- **Añadir asistencia** manualmente: elige el usuario, el evento y el estado (*Asistido* o *No asistido*) y pulsa **Crear asistencia**. Útil cuando alguien asistió pero no se emparejó con Eventbrite (por ejemplo, se inscribió con otro nombre o correo). No puede haber dos asistencias de la misma persona al mismo evento.
- **Editar** una asistencia: cambiar el usuario, el evento o el estado.
- **Borrar** una asistencia (pide confirmación).

> Si vuelves a **Cargar asistencia** de un evento, el estado de las personas emparejadas se sobrescribirá con el de Eventbrite. Las asistencias añadidas manualmente para personas que no están en Eventbrite no se ven afectadas.

## Recomendaciones para el alumnado

Recuérdales estas dos cosas antes de los eventos; evitarán la mayoría de incidencias:

1. Inscribirse en Eventbrite con **el mismo nombre y apellidos** que tienen en Evidentia (o, al menos, con el mismo correo).
2. Pasar por el **check-in** al llegar al evento.

## Plazo que te afecta

| Plazo | Efecto |
|---|---|
| **Importación de eventos y asistencias** | Cuando vence, desaparece *Ajustes de Eventbrite* y ya no puedes cargar eventos ni asistencias ni ocultar/mostrar eventos. Sigues viendo las listas. |

## Lista de comprobación

- [ ] El token de Eventbrite está validado.
- [ ] Todos los eventos de las jornadas están cargados y los que no procede mostrar están ocultos.
- [ ] Tras cada evento he vuelto a cargar su asistencia.
- [ ] He resuelto manualmente las asistencias de quienes no se emparejaron.
- [ ] Todo está cargado antes de que venza el plazo de importación.
