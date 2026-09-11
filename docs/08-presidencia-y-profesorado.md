# 8. Guía de presidencia y profesorado

[← Volver al índice](../README.md)

La **presidencia** de las jornadas y el **profesorado** de la asignatura comparten la mayor parte de las herramientas de gestión. El profesorado dispone además de algunas herramientas exclusivas (importación de alumnos, aleatorización, integridad y borrado masivo).

| Herramienta | Presidente | Profesor |
|---|:-:|:-:|
| Configurar curso | ✔ | ✔ |
| Gestionar alumnos (ver, editar roles, crear) | ✔ (no ve al profesorado) | ✔ |
| Gestionar evidencias (todas) | ✔ | ✔ |
| Gestionar reuniones (todas) | ✔ | ✔ |
| Gestionar comités | ✔ | ✔ |
| Exportaciones | ✔ | ✔ |
| Importaciones (alumnos desde Excel) | | ✔ |
| Aleatorizar evidencias | | ✔ |
| Comprobar integridad | | ✔ |
| Borrar todos los usuarios | | ✔ |

Las herramientas están en los bloques **PRESIDENCIA** o **HERRAMIENTAS DEL PROFESOR** del menú lateral, según el rol.

## Puesta en marcha de un curso (orden recomendado)

1. **Profesor:** importar el listado de alumnos desde Excel (*Importaciones*).
2. **Profesor:** revisar los comités (*Gestionar comités*).
3. **Profesor o presidente:** configurar las cinco fechas límite (*Configurar curso*).
4. **Profesor:** dar el rol *Presidente* a la persona que preside las jornadas (*Gestionar alumnos*).
5. **Presidente:** asignar los roles de coordinador, secretario y coordinador de registro y su comité (*Gestionar alumnos*).
6. Avisar al alumnado de que establezca su contraseña con **«He olvidado mi contraseña o soy nuev@ en Evidentia»** ([capítulo 2](02-acceso-y-perfil.md#primer-acceso-establecer-tu-contraseña)).

## Configurar curso

Define las cinco **fechas límite** del curso, cada una con día y hora:

| Plazo | Qué bloquea al vencer |
|---|---|
| **Subida de nuevas evidencias** | Crear, editar, volver a publicar y borrar evidencias (estudiantes). |
| **Validación de evidencias** | Aceptar y rechazar evidencias (coordinadores). Debe ser **posterior** a la de subida. |
| **Registro de reuniones** | Fecha de referencia para las actas de los secretarios; se muestra a los estudiantes. |
| **Registro de bonos** | Crear, editar y borrar bonos de horas (secretarios). |
| **Registro de eventos y asistencias** | Ajustes de Eventbrite y carga de eventos y asistencias (coordinador de registro). |

Pulsa **Guardar configuración**. Para poder guardar, **las cinco fechas deben ser posteriores al día de hoy**; si necesitas modificar una fecha una vez que otra ya ha vencido, tendrás que adelantar también la vencida a una fecha futura.

Las fechas se muestran a todos los usuarios en el panel principal y, con cuenta atrás, en las secciones correspondientes.

> Deja margen entre el cierre de subida y el de validación: los coordinadores necesitan tiempo para revisar, y los estudiantes para corregir los rechazos antes de que cierre la subida.

## Gestionar alumnos

Muestra el listado de usuarios (apellidos, nombre, UVUS y roles). Al pulsar sobre un nombre se abre su **perfil**, con todas sus evidencias publicadas; desde ahí puedes abrir cada evidencia, comprobar su integridad y descargar sus pruebas.

La presidencia **no ve** las cuentas con rol Profesor.

### Editar un usuario

Pulsa el icono de edición de la fila. El formulario tiene cuatro apartados:

| Apartado | Contenido |
|---|---|
| **Datos personales** | UVUS, nombre, apellidos y correo. UVUS y correo deben ser únicos. |
| **Configuración** | Interruptor **Permitir acceso a la aplicación** y selector de **roles** (puedes marcar varios). Si asignas *Coordinador* o *Secretario*, debes elegir además el **comité asociado**. |
| **Cambio de contraseña** | Opcional. Si la rellenas (mínimo 6 caracteres, dos veces), sustituye la del usuario. |

Pulsa **Actualizar usuario**.

Notas:

- Al guardar se sustituyen **todos** los roles anteriores por los marcados. Revisa que el rol *Estudiante* sigue marcado en quien deba tenerlo.
- El comité elegido se aplica tanto al rol Coordinador como al rol Secretario si la persona tiene ambos.
- La presidencia no puede asignar el rol *Profesor*.

### Añadir un usuario manualmente

Al pie de *Gestionar alumnos* hay un formulario **Añadir nuevo usuario** con nombre, apellidos, correo y UVUS. El usuario se crea con rol *Estudiante* y una contraseña aleatoria: deberá establecer la suya con **«He olvidado mi contraseña o soy nuev@ en Evidentia»**.

Para altas masivas usa la **importación desde Excel** (solo profesorado, ver más abajo).

### Borrar todos los usuarios (solo profesorado)

En el menú **Acciones** de *Gestionar alumnos*, la opción **Borrar todos los usuarios** elimina **todos los usuarios excepto el tuyo** junto con sus evidencias, asistencias y reuniones. Está pensada para limpiar la instancia al principio del curso o tras hacer pruebas. Pide confirmación explícita y **no se puede deshacer**.

## Gestionar comités

Muestra la tabla de comités con su icono, su nombre y una previsualización.

- **Editar**: cambia el icono o el nombre directamente en la tabla y pulsa **Guardar comités**. El icono es el código HTML de un icono de [Font Awesome](https://fontawesome.com/icons?d=gallery), por ejemplo `<i class="fas fa-warehouse"></i>`.
- **Crear**: rellena el formulario **Crear nuevo comité** (icono opcional, nombre obligatorio y único) y pulsa **Crear comité**.
- **Eliminar**: pulsa **Eliminar** en la fila. Un comité solo puede eliminarse si **no tiene coordinador ni secretario, no tiene evidencias (en ningún estado) y no tiene reuniones**. Si no se cumple, la ventana te indica cuántos elementos lo impiden.

## Gestionar evidencias

Tabla con **todas las evidencias publicadas** de todos los comités (las que están en borrador no aparecen): ID, título, autor, horas, comité, fecha y estado. Puedes buscar y ordenar. Pulsa el título para abrir la evidencia (con su comprobación de integridad y sus pruebas) o el nombre del autor para ver su perfil.

Desde aquí no se aceptan ni rechazan evidencias: esa decisión corresponde al coordinador de cada comité.

## Gestionar reuniones

Tabla con **todas las reuniones** registradas por los secretarios: título, lugar, horas, comité, número de asistentes y fecha. En la columna **Acta** puedes descargar el PDF de cada acta.

## Exportaciones

Genera un **archivo Excel** con una fila por estudiante (el profesorado no se incluye) con el cómputo de horas. Marca qué bloques quieres incluir y pulsa **Exportar**:

| Columnas siempre presentes | Apellidos, Nombre, UVUS, Correo, Perfil (enlace), Participación (nivel de implicación), Comité, Evidencia aleatoria (enlace) y Horas de evidencia aleatoria |
|---|---|
| **Evidencias** | Evidencias registradas (aceptadas) y Horas de evidencias |
| **Reuniones** | Reuniones asistidas y Horas de reuniones |
| **Eventos** | Eventos asistidos y Horas de asistencia |
| **Bono de horas** | Bono de horas |
| Última columna | **Horas en total**, suma de los bloques marcados |

La columna *Comité* refleja los comités a los que el estudiante ha enviado evidencias aceptadas y, si es coordinador o secretario, el suyo.

## Importaciones (solo profesorado)

Permite dar de alta a todo el alumnado de una vez a partir de un archivo **Excel (XLS/XLSX)**.

1. Prepara el archivo con estas columnas en la primera fila, **exactamente con estos nombres**:

   | apellidos | nombre | uvus | grupo | email |
   |---|---|---|---|---|
   | Polo Polo | Marco | marpolpol | Grupo 1 | polo@mail.com |

2. Comprueba que **UVUS y email son únicos** y que no hay celdas combinadas.
3. En **Importaciones**, arrastra el archivo al cuadro de subida y pulsa **Importar alumnos**. No cierres la página mientras se procesa.

Todos los usuarios importados reciben el rol **Estudiante** y una contraseña aleatoria. El archivo se borra del sistema tras la importación. Después, indica al alumnado que establezca su contraseña desde la pantalla de acceso.

Si el archivo contiene un UVUS o correo que ya existe, la importación se interrumpe con un error (las filas anteriores a la errónea pueden haberse importado ya): corrige el archivo, quita de él los alumnos ya dados de alta y vuelve a intentarlo.

## Aleatorizar evidencias (solo profesorado)

Selecciona **al azar una evidencia aceptada de cada estudiante** para su evaluación. El resultado se refleja en la exportación (columnas *Evidencia aleatoria* y *Horas de evidencia aleatoria*).

Pulsa **Aleatorizar evidencias**. Puedes ejecutarlo varias veces; cada ejecución descarta la selección anterior y puede cambiar la evidencia elegida. Los estudiantes sin evidencias aceptadas quedan sin selección.

## Comprobar integridad (solo profesorado)

Muestra dos pestañas, **Evidencias** y **Pruebas**, con todos los registros del sistema y una columna **Integridad** que indica si el sello de cada evidencia o archivo coincide con su contenido actual. Un fallo de integridad significa que la evidencia o el archivo se ha modificado fuera de la aplicación después de su registro.

## Lista de comprobación de cierre del curso

- [ ] Han vencido los plazos de subida y de validación.
- [ ] Los secretarios han levantado todas las actas y registrado los bonos.
- [ ] El coordinador de registro ha cargado las asistencias de todos los eventos.
- [ ] He ejecutado **Aleatorizar evidencias**.
- [ ] He comprobado la **integridad**.
- [ ] He generado la **exportación** completa (evidencias, reuniones, eventos y bonos).
