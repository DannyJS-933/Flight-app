# Flight-app
Se requiere un sistema que permita realizar la reserva de un boleto aéreo. Donde
un cliente puede registrarse, luego escoger el país de origen y destino, para
posteriormente seleccionar el aeropuerto correspondiente a los países
seleccionados, donde por cada aeropuerto se mostrará el itinerario de vuelos
disponibles. El sistema le reservará espacio en el vuelo que el cliente desee.
3. Descripción detallada del proyecto
3.1 Comportamiento esperado de la aplicación
1. Se requiere una función de autenticación de usuarios, donde existirán dos
tipos de roles: administrativos y clientes. Los roles deben estar almacenados
en la base de datos, asociados a su vez a los usuarios.
2. El sistema deberá identificar el rol del usuario una vez autenticado, y así
mostrar las opciones de menú a las que tiene acceso.
3. El sistema consta de dos módulos, uno administrativo y otro dirigido a los
clientes.
4. Módulo cliente:
a. El cliente debe registrarse con la información requerida por el
sistema; además, se debe solicitar un usuario y contraseña para la  
autenticación. Al ser cliente se le asociará el rol “cliente” para que
pueda ingresar al sistema sin problemas.
Información requerida:
i. Nombre
ii. Apellido (s)
iii. Identificación
iv. Nacionalidad
v. Sexo
vi. Fecha de nacimiento
vii. Edad (calculado mediante fecha de nacimiento)
viii. Usuario
ix. Contraseña
b. El cliente se autenticará con las credenciales del sistema y una vez
identificado, se mostrará las reservas qua ha realizado, donde puede
agregar, eliminar o modificar. Se debe validar que no pueda crear
reservas en las fechas que ya tiene comprometidas (en reservas
anteriores).
c. Si el cliente desea realizar una nueva reserva el sistema debe tener
un comportamiento similar al siguiente:
i. Se le debe mostrar la información del País del cual desea
partir y al cual es su destino.
ii. Por cada país el cliente debe escoger los aeropuertos
asociados (disponibles), tanto para origen como destino.
iii. Una vez que se selecciona el aeropuerto y las fechas del viaje,
el sistema muestra los vuelos disponibles (itinerario de
vuelos).
iv. El cliente indica la cantidad de boletos que requiere (cantidad
de pasajeros).
v. El cliente selecciona el vuelo y el sistema valora si hay cupo
disponible en el avión para permitir la reserva.
vi. El sistema valida que no tenga reservas en las fechas
seleccionadas.
vii. La reserva del vuelo es almacenada en la base de datos.
d. Una vez almacenada la reserva, el sistema devuelve al cliente a la
lista de reservas que tiene registradas mediante interfaz de usuario.
e. El sistema le debe permitir al cliente exportar una o todas las
reservas mediante un archivo XML con la información del cliente,
países de origen y destino, aeropuerto de origen y destino,
información del vuelo y la cantidad de boletos adquiridos.
5. Módulo administrativo:
a. Debe ser posible buscar en una lista de clientes ya existentes, donde
cada vez que se registre un nuevo cliente la lista deberá actualizarse.
b. El administrador puede crear, modificar y eliminar clientes.
c. Se permite al administrador crear o eliminar reservas de un cliente
especifico, donde lo puede seleccionar mediante lista anterior y el
sistema realizaría el mismo comportamiento como si fuera el cliente.
d. El administrador puede exportar una reserva de un cliente a un
archivo XML con el mismo formato que se generaría al cliente.
e. Deben existir las interfaces que permitan manipular la información de
los siguientes datos (CRUD):
i. Países
ii. Aeropuertos
iii. Aviones y su capacidad
iv. Itinerarios
3.2 Base de datos:
Se deberá crear una base de datos que permita:
1. Manejo de usuarios.
2. Registrar los datos importantes de los clientes, indicados en el punto 4a.
3. Registrar la información de login de los usuarios del sistema.
4. Crear las estructuras que permitan establecer una reserva de un boleto
aéreo, como mínimo debe tener: países, aeropuertos por país, aviones con
su capacidad, itinerario.
5. Se debe almacenar por cada cliente las reservas que realizan.
6. Así como otra información requerida para el uso correcto del sistema, en
caso de ser necesario.
7. Se requiere el uso de procedimientos almacenados para la obtención
de la información.
3.3 Interfaz
Se debe crear una interfaz en Windows Forms que cumpla con las funcionalidades
indicadas en el punto 3.1. Las cuales quedan a criterio del estudiante.
3.4 Manual de usuario
Crear un video explicativo del sistema y sus funcionalidades.
4. Descripción técnica
El proyecto se debe desarrollar usando:
● Visual Basic .Net en Visual Studio 2019.
● Se debe utilizar .NET Framework (evitar el uso de .NET Core).
● Utilizar Windows Forms para desarrollo de interfaces.
● El diseño de las interfaces queda a criterio de los estudiantes.
● Se debe utilizar una arquitectura N capas.
● Se debe utilizar SQL Server para el desarrollo de la base de datos.
● La estructura de la base de datos queda a criterio del estudiante, así como
la definición de los atributos que requiera para el uso de la aplicación.
● El manejo de datos debe ser mediante base de datos.
● Se permite el uso de ADO.NET o Entity Framework para la conexión de base
de datos. 
● Debe generar 1 único archivo XML válido con la información solicitada.
● Se debe realizar el manejo de errores, tanto en aplicación como en base de
datos.
