 Explicacion de la Tarea Integradora  Fase 1

En esta primera fase del proyecto desarrolle la propuesta y la planificacion inicial de UniBot, una aplicacion de consola creada con Node.js que busca ayudar a estudiantes de primer ingreso a resolver dudas academicas y tecnicas relacionadas con su carrera. La idea es que la inteligencia artificial responda preguntas basicas, pero sin ofrecer informacion de carreras diferentes a la del estudiante.

 1. Descripcion del sistema

Explique que es UniBot, cual es su proposito y que necesidad busca resolver. El sistema pretende reducir la cantidad de preguntas repetitivas que reciben los asesores humanos y evitar que los estudiantes obtengan informacion que no corresponda a su carrera.

Tambien identifique los dos tipos de usuarios:

- Estudiante: ingresa con su codigo institucional y utiliza el chat para hacer consultas.
- Administrador: accede mediante una contrasena maestra y puede gestionar estudiantes, modificar los temas permitidos para cada carrera, revisar las sesiones y cerrarlas de forma forzada cuando sea necesario.

Ademas, describi como se almacenara la informacion. El sistema no utilizara una base de datos: los estudiantes estaran registrados en un archivo CSV, las carreras y sus temas permitidos estaran en un archivo JSON, y las sesiones y conversaciones se guardaran en archivos para llevar un registro de su actividad.

 2. Entradas, procesos, salidas y subsistemas

Organice el funcionamiento de UniBot mediante sus entradas, procesos y salidas.

- Entradas: incluyen el codigo institucional, la contrasena del administrador, los mensajes del estudiante y la informacion guardada en los archivos.
- Procesos: incluyen validar al estudiante, consultar su carrera, preparar el contexto que se enviara a la inteligencia artificial, registrar los mensajes y calcular el costo de cada sesion.
- Salidas: incluyen las respuestas del chat, los mensajes de bienvenida o error, el historial de la conversacion y los registros actualizados.

Tambien separe el sistema en subsistemas, como autenticacion, gestion de archivos, manejo de sesiones, conexion con la inteligencia artificial y trazabilidad. Esto permite entender que responsabilidad cumple cada parte del programa.

 3. Eleccion del desarrollo incremental

Seleccione el desarrollo incremental porque el proyecto esta organizado en varias fases y sus funcionalidades se pueden construir progresivamente. La idea es comenzar con la definicion de requisitos y una estructura inicial, y luego agregar la autenticacion, la programacion orientada a objetos, TypeScript, la gestion de sesiones y la conexion con una API de inteligencia artificial.

Organice las cuatro fases como sprints. En cada sprint se trabaja un conjunto de funcionalidades que se apoya en lo desarrollado anteriormente.

 4. Product Backlog: requisitos del sistema

Elabore un Product Backlog con los requisitos funcionales y no funcionales de UniBot, identificados mediante codigos y organizados por prioridad.

Los requisitos funcionales describen lo que el sistema debe hacer. Entre ellos estan seleccionar el tipo de usuario, autenticar al administrador, validar estudiantes, registrar usuarios, modificar los temas permitidos, responder consultas, restringir las respuestas segun la carrera, registrar y cerrar sesiones, calcular costos, guardar conversaciones, conectarse a una API externa y manejar errores.

Los requisitos no funcionales establecen condiciones sobre como debe construirse el sistema. Incluyen mantener la contrasena fuera del codigo fuente mediante variables de entorno, utilizar TypeScript con tipado estricto, organizar el codigo en modulos, mantener una nomenclatura consistente, documentar el codigo y utilizar Git.

Asignar prioridades permite identificar que requisitos deben atenderse primero y cuales pueden desarrollarse en etapas posteriores.

 5. Diagrama UML de casos de uso

Inclui una explicacion del diagrama UML de casos de uso para mostrar la relacion entre los dos actores y las funciones de UniBot. El estudiante puede acceder al chat y realizar consultas, mientras que el administrador puede gestionar usuarios y temas, consultar informacion de las sesiones y realizar cierres forzados.

El diagrama ayuda a delimitar las funciones del sistema y a distinguir los permisos de cada tipo de usuario.

 6. Tablero Kanban

Finalmente, organice los requisitos en un tablero Kanban con tres columnas: Por hacer, En progreso y Hecho. Alli enumere los requisitos funcionales y no funcionales que deben desarrollarse.

Este tablero sirve para visualizar el avance del proyecto, identificar las tareas pendientes y llevar un control del trabajo durante las distintas fases.

 Conclusion

En resumen, en esta fase defini que es UniBot, que problema busca resolver, quienes lo utilizaran y como se espera que funcione. Tambien identifique sus entradas, procesos, salidas y subsistemas; escogi un enfoque de desarrollo incremental; organice los requisitos en un Product Backlog; describi las interacciones mediante un diagrama de casos de uso y distribui las tareas en un tablero Kanban. Esta planificacion establece una base para desarrollar el sistema en las siguientes fases.

Importante: este documento describe la propuesta y la planificacion presentadas en la Fase 1; no afirma que todas las funcionalidades ya esten programadas o implementadas.
