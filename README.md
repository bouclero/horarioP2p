Control Horario P2P con Sincronización en Tiempo Real
Esta es una aplicación web avanzada para el control de horarios laborales que funciona sin necesidad de un servidor o base de datos central. Utiliza tecnologías P2P (Peer-to-Peer) a través de WebRTC para permitir la sincronización de datos en tiempo real entre diferentes usuarios.

✨ Características Principales
Sin Backend: La aplicación es 100% cliente. Todos los datos se guardan localmente en el navegador y se sincronizan directamente entre los usuarios conectados.

Sincronización P2P en Tiempo Real: Un usuario (Host) puede crear una sala y compartir un ID. Otros usuarios (Clientes) pueden unirse a esa sala para ver y recibir actualizaciones del horario en tiempo real.

Gestión de Horarios Mensual: Genera una vista de calendario mensual para asignar y visualizar las horas de entrada y salida de múltiples trabajadores.

Entrada de Datos Intuitiva: Haz clic en cualquier celda para abrir un modal y registrar la hora de entrada, salida y la firma del trabajador.

Firma Digital: Cada registro puede ser validado con una firma digitalizada, dibujada directamente en la aplicación.

Gestión de Trabajadores: Añade o elimina trabajadores de la lista fácilmente.

Informes Mensuales: Calcula y muestra automáticamente el total de horas trabajadas por cada empleado en el mes seleccionado.

Importación y Exportación de Datos:

Exporta el informe mensual a un archivo de texto (.txt) legible.

Exporta todos los datos de la aplicación (trabajadores y horarios) a un archivo JSON como copia de seguridad.

Importa datos desde un archivo JSON para restaurar o consolidar información.

Persistencia Local: Los datos se guardan en el localStorage del navegador, por lo que no se pierden al cerrar la pestaña.

🚀 Cómo Usar
Configuración Inicial
Añadir Trabajadores: En la sección "Gestión de Datos", introduce el nombre de un trabajador y haz clic en "Añadir". Repite el proceso para todos los trabajadores.

Generar Horario: Selecciona el mes y el año deseado y haz clic en "Generar". Se creará la tabla con los trabajadores y los días del mes.

Registrar Horas
Haz clic en la celda del día y trabajador que quieras editar.

En la ventana emergente, introduce la hora de entrada y salida. Puedes usar el botón "Ahora" para registrar la hora actual.

Pide al trabajador que dibuje su firma en el panel correspondiente.

Haz clic en "Guardar Registro". La celda se actualizará y los datos se sincronizarán con los clientes conectados.

Guardar los Datos
Aunque los datos se actualizan en tiempo real, es una buena práctica hacer clic en "Guardar" en la sección "Gestión de Datos" para asegurar que todo se guarde en la memoria local del navegador.

🌐 Sincronización P2P
Esta es la característica más potente de la aplicación.

Para el Host (quien crea la sala):

En la sección "Conexión P2P", selecciona la acción "Crear sala (Host)".

Haz clic en "Conectar". Se generará un ID de Sala único.

Comparte ese ID con los otros usuarios que quieras que se conecten.

Para los Clientes (quienes se unen):

Selecciona la acción "Unirse a sala (Cliente)".

Pega el ID de Sala que te ha proporcionado el Host en el campo "ID de Sala".

Haz clic en "Conectar".

Una vez conectados, los clientes recibirán automáticamente todos los datos del horario del Host. Cualquier cambio que el Host realice se reflejará en tiempo real en las pantallas de los clientes.

💾 Importar y Exportar
Exportar Informe (TXT): Genera un resumen de texto plano del mes actual, ideal para imprimir o enviar.

Exportar Datos (JSON): Crea una copia de seguridad completa de tu estado actual (trabajadores y todos los horarios). Este es el archivo que debes usar para la función de importar.

Importar Datos: Te permite cargar un archivo .json previamente exportado para restaurar todos los datos.

💻 Tecnologías Utilizadas
HTML5

CSS3 (Estilo moderno sin frameworks)

JavaScript (ES6+)

PeerJS: Librería que simplifica la conexión WebRTC para la comunicación P2P.

SignaturePad.js: Librería para capturar la firma digital en un canvas.

FileSaver.js: Librería para facilitar la descarga de archivos generados.

📄 Licencia
Este proyecto está bajo la licencia de JJRAMIREZ.
