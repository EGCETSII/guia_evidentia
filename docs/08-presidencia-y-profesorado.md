# 8. Guía de presidencia y profesorado

[← Volver al índice](../README.md)

La **presidencia** de las jornadas y el **profesorado** de la asignatura comparten casi todas las herramientas de gestión. El profesorado tiene además tres exclusivas (importar alumnos, borrarlos todos y aleatorizar) y la presidencia tiene su propia cola de revisión.

| Herramienta | Presidente | Profesor |
|---|:-:|:-:|
| Configurar curso | Sí | Sí |
| Alumnos (ver, editar, dar roles, crear) | Sí (no ve al profesorado) | Sí |
| Revisar evidencias (cola de presidencia) | Sí | No |
| Evidencias (todas, mover, aceptar o rechazar) | Sí | Sí |
| Reuniones, Asistencias y Bonos (consulta) | Sí | Sí |
| Comités | Sí | Sí |
| Integridad | Sí | Sí |
| Exportar | Sí | Sí |
| Registro de actividad y Errores | Sí | Sí |
| Importar alumnos desde Excel | No | Sí |
| Borrar todos los usuarios | No | Sí |
| Aleatorizar evidencias | No | Sí |

Las herramientas están en el grupo **Gestión** del menú lateral. Al entrar, tu inicio es el **Panel del curso**: horas acreditadas, participación, evidencias por revisar y aceptación, el estado de cada comité, la actividad reciente, las señales del registro, los accesos, los errores del servidor, la cola de presidencia y los plazos.

## Puesta en marcha de un curso (orden recomendado)

1. **Profesor:** importar el listado de alumnos desde Excel (*Importar*).
2. **Profesor o presidente:** revisar los comités (*Comités*).
3. **Profesor o presidente:** configurar los cinco plazos (*Configurar curso*).
4. **Profesor:** dar el rol *Presidente* a la persona que preside las jornadas (*Alumnos*).
5. **Presidente:** asignar los roles de coordinador, secretario y coordinador de registro y su comité (*Alumnos*).
6. Avisar al alumnado de que establezca su contraseña desde la pantalla de acceso ([capítulo 2](02-acceso-y-perfil.md#primer-acceso-establecer-tu-contraseña)).

## Configurar curso

Define los cinco **plazos** del curso, cada uno en su tarjeta con **Día** y **Hora** (obligatorios). Cada tarjeta indica si el plazo está *Abierto*, *Cerrado* o *Sin plazo*.

| Plazo | Qué bloquea al vencer |
|---|---|
| **Subida de evidencias** | Crear, editar, publicar, volver a enviar y borrar evidencias, subir pruebas y que el autor cambie de comité su evidencia. |
| **Validación de evidencias** | Aceptar y rechazar evidencias (coordinación y presidencia) y que la coordinación las mueva de comité. No puede ser anterior a la de subida. |
| **Registro de reuniones** | Crear, editar y borrar actas (secretarios). |
| **Registro de bonos** | Crear, editar y borrar bonos de horas (secretarios). |
| **Registro de eventos y asistencias** | Eventbrite, eventos y asistencias (coordinador de registro). |

La tarjeta **Límites de horas** fija, si quieres, un tope de horas que cuentan para cada alumno, uno para **Evidencias** (horas de evidencias aceptadas) y otro para **Asistencia** (horas de eventos asistidos). Déjalos vacíos para que cuenten todas. El tope se aplica al total del panel, a la ficha de cada alumno y al Excel de **Exportar**; las horas por encima del límite se siguen viendo en el panel del alumno, por ejemplo *«8,00 h de 11,00 (límite)»*.

Pulsa **Guardar configuración**. Puedes guardar una fecha ya pasada: el plazo queda cerrado. El cambio queda anotado en el registro de actividad.

### Cerrar un plazo ahora

Debajo del formulario, la tarjeta **Cerrar un plazo ahora** tiene un botón por cada plazo abierto. Pulsa **Cerrar** en el que quieras y confirma con **Sí, cerrar ahora**: el plazo vence en ese mismo minuto, sin tener que escribir la fecha. Cerrar la **validación** cierra también la **subida**, porque no puede seguir abierta después. El cierre queda anotado en el registro de actividad.

> Deja margen entre el cierre de subida y el de validación: la coordinación necesita tiempo para revisar, y los estudiantes para corregir los rechazos antes de que cierre la subida.

## Gestionar alumnos

**Alumnos** muestra todos los usuarios salvo tu propia cuenta, con las columnas **Apellidos y nombre** (con el correo), **UVUS**, **DNI** y **Roles** (por ejemplo *Coordinador de* un comité, o *Bloqueado*). Puedes filtrar por **Rol** y por **Estado** (*Todos*, *Activos*, *Bloqueados*), buscar, ordenar y pasar de página. La presidencia **no ve** las cuentas con rol Profesor.

Al pulsar una fila se abre el **perfil** del usuario (su expediente): resumen de horas, datos de la cuenta (comités, último acceso, número de accesos, estado) y pestañas **Evidencias**, **Reuniones**, **Firmas**, **Asistencias**, **Bonos**, **Actividad** y **Mensajes**. Desde ahí puedes **Descargar expediente** (CSV) o **Gestionar la cuenta**.

### Editar un usuario

Pulsa el icono **Gestionar** de la fila (o **Gestionar la cuenta** en su perfil). La página tiene tres tarjetas:

| Tarjeta | Contenido |
|---|---|
| **Datos personales** | Nombre, apellidos, UVUS y correo. UVUS y correo deben ser únicos. |
| **Acceso y roles** | Interruptor **Permitir acceso a la aplicación** y casillas de **Roles** (puedes marcar varios). Si marcas *Coordinador* o *Secretario*, debes elegir además el **Comité**. |
| **Cambio de contraseña** | Opcional. Si la rellenas (dos veces), sustituye la del usuario. Mínimo 8 caracteres con mayúscula, minúscula, número y símbolo. |

Al lado verás sus **Horas computadas** (en evidencias, en reuniones, en asistencia y bonificadas). Pulsa **Guardar cambios**.

Notas:

- Al guardar se sustituyen **todos** los roles anteriores por los marcados. Revisa que el rol *Estudiante* sigue marcado en quien deba tenerlo.
- El comité elegido se aplica tanto al rol Coordinador como al rol Secretario si la persona tiene ambos.
- La presidencia no puede asignar el rol *Profesor* ni gestionar cuentas del profesorado.
- Los cambios quedan anotados en el registro de actividad.

### Añadir un usuario a mano

Pulsa **Nuevo usuario** en *Alumnos* y rellena nombre, apellidos, correo y UVUS (los cuatro obligatorios; correo y UVUS únicos). Pulsa **Añadir usuario**. Se crea con rol *Estudiante* y una contraseña aleatoria: deberá establecer la suya desde la pantalla de acceso.

Para altas masivas usa la **importación desde Excel** (solo profesorado, ver más abajo).

### Arreglar los datos de todos (solo profesorado)

El botón **Arreglar datos** de *Alumnos* corrige de una vez todas las cuentas salvo la tuya y las del profesorado. Marca lo que quieras aplicar y pulsa **Arreglar**.

| Opción | Qué hace |
|---|---|
| **Poner el correo oficial** | Pone como correo el UVUS seguido de *@alum.us.es*. Si ese correo ya lo usa otra cuenta, deja esa persona como estaba y te lo indica. |
| **Pasar nombres y apellidos a mayúsculas** | Pasa a mayúsculas el nombre y los apellidos. |
| **Dar acceso a todos** | Permite el acceso a la aplicación a todas las cuentas bloqueadas. |

Al terminar se indica cuántos usuarios han cambiado. Cada cambio queda anotado en el registro de actividad.

### Borrar todos los usuarios (solo profesorado)

El botón **Borrar todos** de *Alumnos* elimina **todos los usuarios excepto el tuyo** junto con sus evidencias, mensajes, avisos, asistencias y las reuniones que registraron. Está pensado para limpiar la instancia al principio del curso o tras hacer pruebas. Pide confirmación (**Sí, borrar todos**) y **no se puede deshacer**.

## Revisar evidencias (presidencia)

La cola de la presidencia tiene pestañas por estado y reúne las evidencias enviadas al **comité de presidencia** y las que un coordinador escribe para el comité que coordina. Se aceptan o rechazan igual que en la cola de un coordinador ([capítulo 5](05-coordinador.md#revisar-una-evidencia)), mientras el plazo de validación esté abierto. Tus propias evidencias no aparecen.

## Evidencias

Tabla con **todas las evidencias enviadas** de todos los comités (los borradores no aparecen), con pestañas **Todas**, **Pendientes**, **Atrasadas** (pendientes desde hace más de 7 días), **Aceptadas** y **Rechazadas**. Puedes filtrar por **Comité** y por fecha de envío (**Enviada desde**, **Enviada hasta**), buscar y ordenar; se muestra el total de horas de la búsqueda. El autor lleva a su perfil y el comité a su página.

Al abrir el **Historial** de una evidencia tienes dos acciones de gestión:

- **Mover a otro comité**: elige el **Comité de destino** y pulsa **Mover**. Conserva las pruebas, la descripción y el estado.
- **Aceptar o rechazar**: elige la **Decisión** y pulsa **Guardar**. Si rechazas, el **Motivo del rechazo** es obligatorio (entre 10 y 1000 caracteres).

Ambas funcionan aunque el plazo esté cerrado, pero entonces la acción **queda señalada en el registro**. No puedes revisar tus propias evidencias.

## Reuniones, Asistencias y Bonos

Son listas de consulta de todo el curso:

- **Reuniones**: reunión, comité, fecha, horas, asistentes y acta (el botón **Acta** la abre). Se filtra por comité y por *Con acta* o *Sin acta*. Desde aquí también llegas a **Convocatorias** (con el PDF de cada una), **Hojas de firmas** y **Listas**.
- **Asistencias**: todas las asistencias con las horas que computan, con pestañas **Todas**, **Asistidas**, **Pendientes** y **No asistidas** y filtro por evento, y los eventos con sus inscritos.
- **Bonos**: bono, comité, personas, horas y fecha de creación.

## Comités

Tabla de comités con su **Equipo** (avisa *Sin coordinación* o *Sin secretaría*), evidencias **Pendientes**, **Horas**, **Reuniones**, **Última actividad** y **Alertas** (*Todo en orden* si no hay ninguna).

- **Crear**: pulsa **Nuevo comité**, escribe el **Nombre** (obligatorio y único) y elige un **Icono**. Pulsa **Crear comité**.
- **Editar**: cambia el nombre o el icono en **Editar el comité** y pulsa **Guardar**. Dos comités no pueden llamarse igual.
- **Eliminar**: el botón **Eliminar el comité** solo aparece si el comité no es el de presidencia, **no tiene coordinador ni secretario, no tiene evidencias (en ningún estado) y no tiene reuniones**.

Al pulsar un comité se abre su página: alertas, equipo (último acceso, última acción y última revisión), horas por origen, envíos por semana, próximas convocatorias y últimas reuniones, evidencias, mensajes y actividad del comité. Las alertas avisan de:

- comités sin coordinación o sin secretaría (*Asignar en Alumnos*);
- evidencias que esperan revisión más de 7 días;
- convocatorias ya celebradas sin acta;
- mensajes sin responder más de 3 días;
- más de 21 días sin reuniones;
- evidencias rechazadas sin corregir más de 7 días.

Muchas alertas incluyen un botón (por ejemplo *Escribir a la coordinación* o *Escribir a la secretaría*) que abre un mensaje ya redactado.

## Mensajes, Registro de actividad y Errores

- **Mensajes**: la presidencia puede leer todas las conversaciones, pero solo participa en las dirigidas a ella o que ha iniciado. El profesorado puede participar en todas.
- **Registro de actividad**: todas las anotaciones del curso, con filtros (quién, acción, señales...) y **Descargar CSV**.
- **Errores**: los errores del servidor con el número de veces y la última vez. Cada uno puede **Marcar como resuelto** o **Reabrir**.

## Exportar

Genera un **archivo Excel** con una fila por usuario (el profesorado no se incluye) con el cómputo de horas. En la tarjeta *Horas del curso*, marca en **Qué incluir** los bloques que quieres y pulsa **Descargar Excel**:

| Columnas siempre presentes | Apellidos, Nombre, Uvus, Correo, Perfil (enlace), Comité, Evidencia aleatoria y Horas de evidencia aleatoria |
|---|---|
| **Evidencias** | Evidencias registradas y Horas de evidencias |
| **Reuniones** | Reuniones asistidas y Horas de reuniones |
| **Asistencia** | Asistencias y Horas de asistencia |
| **Bonos de horas** | Bono de horas |
| Última columna | **Horas en total**, suma de los bloques marcados |

### Copia de las evidencias

La tarjeta **Copia de las evidencias** descarga con **Descargar copia** un archivo ZIP con todas las evidencias enviadas del curso (no incluye borradores ni eliminadas). Dentro va *evidencias.csv*, con una fila por evidencia (alumno, comité, título, descripción, horas, estado, fechas y pruebas), y la carpeta *pruebas*, ordenada por uvus y número de evidencia, con los archivos adjuntos. Sirve como copia de seguridad al cerrar el curso.

## Importar alumnos (solo profesorado)

Da de alta a todo el alumnado de una vez a partir de un archivo **Excel (.xls o .xlsx)**. Llegas desde **Importar** en el menú o en *Alumnos*.

1. Prepara el archivo con estas columnas en la primera fila, **exactamente con estos nombres**:

   | apellidos | nombre | uvus | grupo | email |
   |---|---|---|---|---|
   | Polo Polo | Marco | marpolpol | Grupo 1 | polo@mail.com |

2. Comprueba que **UVUS y correo son únicos** y que no hay celdas combinadas.
3. Arrastra el archivo al cuadro *Hoja de cálculo* (o púlsalo para elegirlo) y pulsa **Importar alumnos**. No cierres la página mientras se procesa.

Todos los usuarios importados reciben el rol **Estudiante** y una contraseña aleatoria. El archivo se borra tras la importación. Después, indica al alumnado que establezca su contraseña desde la pantalla de acceso.

Si algo falla (por ejemplo, un UVUS o correo que ya existe), la importación se cancela entera y no se da de alta a nadie: corrige el archivo y vuelve a intentarlo.

## Aleatorizar evidencias (solo profesorado)

Elige **al azar una evidencia aceptada de cada alumno** para su evaluación. El resultado aparece en la exportación (columnas *Evidencia aleatoria* y *Horas de evidencia aleatoria*) y la página muestra cuántas **Evidencias elegidas** hay.

Pulsa **Aleatorizar** y confirma con **Sí, aleatorizar**. Puedes repetirlo; cada vez se sustituye la elección anterior.

Desde que se aleatoriza, los alumnos **ya no pueden cambiar su resumen del trabajo**, que queda fijo para la evaluación. El diálogo de confirmación lo recuerda.

## Integridad

Muestra dos pestañas, **Evidencias** y **Pruebas**, con todos los registros y una columna **Integridad** (*Íntegra* o *Alterada*). Arriba se cuentan las evidencias y pruebas alteradas. Una alteración significa que la evidencia o el archivo se ha modificado fuera de la aplicación después de su registro.

## Lista de comprobación de cierre del curso

- [ ] Han vencido los plazos de subida y de validación.
- [ ] La cola de presidencia está vacía.
- [ ] Los secretarios han levantado todas las actas y registrado los bonos.
- [ ] El coordinador de registro ha cargado las asistencias de todos los eventos.
- [ ] Se ha ejecutado **Aleatorizar evidencias**.
- [ ] Se ha comprobado la **integridad**.
- [ ] Se ha generado la **exportación** completa (evidencias, reuniones, asistencia y bonos).
