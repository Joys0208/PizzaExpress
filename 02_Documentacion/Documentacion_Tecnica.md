Documentación Técnica – PizzaExpress
1. Introducción
PizzaExpress es una propuesta de sistema de gestión de pedidos e inventario para una pizzería. Su propósito es apoyar la administración de los pedidos, el control de inventario, la gestión de usuarios y roles, la validación de entregas y la consulta de reportes de ventas.
La solución fue planteada aplicando principios de Ingeniería de Software y una metodología de trabajo ágil, buscando organizar las funcionalidades de acuerdo con las necesidades principales del negocio.

2. Objetivo de la solución
El objetivo de PizzaExpress es centralizar y organizar la información relacionada con los procesos operativos de una pizzería, reduciendo la dependencia de registros manuales y facilitando el control de pedidos e inventario.
Entre sus principales objetivos se encuentran:
•	Gestionar pedidos de manera organizada.
•	Controlar las existencias de ingredientes.
•	Actualizar el inventario de acuerdo con los pedidos.
•	Generar alertas cuando existan niveles bajos de inventario.
•	Administrar usuarios y roles.
•	Controlar el acceso a las funcionalidades.
•	Validar las entregas de productos.
•	Consultar reportes de ventas.
•	Facilitar la toma de decisiones administrativas.

3. Alcance técnico
La propuesta contempla las siguientes funcionalidades:
1.	Inicio de sesión.
2.	Gestión de usuarios.
3.	Gestión de roles y permisos.
4.	Registro de pedidos.
5.	Gestión de pedidos en mesa.
6.	Gestión de pedidos para llevar.
7.	Gestión de pedidos a domicilio.
8.	Gestión de inventario.
9.	Descuento automático de ingredientes.
10.	Alertas de inventario.
11.	Validación de entregas.
12.	Consulta de reportes de ventas.
Funcionalidades fuera del alcance del MVP
Para mantener un alcance controlado, no se contemplan inicialmente:
•	Pagos en línea.
•	Aplicación independiente para domiciliarios con GPS.
•	Programa de fidelización de clientes.
Estas funcionalidades podrían considerarse posteriormente como mejoras o nuevas versiones del sistema.

4. Arquitectura propuesta
PizzaExpress se plantea utilizando una arquitectura por capas, con el propósito de separar las responsabilidades del sistema.
Las principales capas son:
4.1 Capa de presentación
Es la parte con la que interactúan los usuarios.
Incluye:
•	Pantallas de inicio de sesión.
•	Formularios de pedidos.
•	Gestión de usuarios.
•	Inventario.
•	Entregas.
•	Reportes.
Su función es recibir las acciones del usuario y presentar la información generada por el sistema.
4.2 Capa de lógica de negocio
Contiene las reglas que permiten procesar las operaciones del sistema.
Por ejemplo:
•	Validación de credenciales.
•	Control de permisos.
•	Cálculo del valor de los pedidos.
•	Descuento de ingredientes.
•	Validación de existencias.
•	Generación de alertas.
•	Procesamiento de reportes.
4.3 Capa de datos
Es responsable del almacenamiento y consulta de la información.
Puede manejar información relacionada con:
•	Usuarios.
•	Roles.
•	Productos.
•	Ingredientes.
•	Pedidos.
•	Detalles de pedidos.
•	Inventario.
•	Entregas.
•	Ventas.
La separación por capas facilita el mantenimiento y permite realizar cambios en una parte del sistema sin afectar directamente las demás.

5. Tecnologías y herramientas
Para el desarrollo y gestión de la propuesta PizzaExpress se consideran las siguientes tecnologías y herramientas.
Tecnología / herramienta	     Uso dentro del proyecto
Python	                       Lenguaje de programación para la lógica de la aplicación
Django	                       Framework para el desarrollo de la aplicación web
HTML	                          Estructura de las interfaces
CSS	                            Presentación y estilos de las interfaces
Base de datos relacional	      Almacenamiento de la información del sistema
Git	                            Control de versiones
GitHub	                        Repositorio y gestión del código/documentación
Trello	                        Organización y seguimiento de tareas
draw.io	                        Elaboración de diagramas
Excel	                          Elaboración del cronograma del proyecto

6. Justificación de las tecnologías
6.1 Python
Python fue considerado como lenguaje de programación debido a que posee una sintaxis clara y permite desarrollar aplicaciones de manera organizada.
También cuenta con una amplia comunidad y numerosas herramientas que facilitan el desarrollo y mantenimiento de proyectos de software.
6.2 Django
Django fue seleccionado como framework porque permite desarrollar aplicaciones web utilizando Python y proporciona mecanismos para trabajar con funcionalidades comunes como:
•	Gestión de usuarios.
•	Manejo de solicitudes.
•	Modelos de datos.
•	Formularios.
•	Seguridad.
•	Conexión con bases de datos.
Su estructura favorece la organización del proyecto y facilita el desarrollo de aplicaciones mantenibles.
6.3 HTML y CSS
HTML permite estructurar las páginas y formularios de la aplicación, mientras que CSS permite definir la presentación visual de las interfaces.
La combinación de ambas tecnologías permite construir interfaces organizadas y comprensibles para los usuarios.
6.4 Base de datos relacional
Una base de datos relacional permite organizar la información en estructuras relacionadas.
En PizzaExpress resulta útil para mantener relaciones entre entidades como:
•	Usuarios y roles.
•	Pedidos y productos.
•	Productos e ingredientes.
•	Inventario y movimientos.
•	Pedidos y ventas.
Esto contribuye a mantener la integridad y organización de los datos.
6.5 Git y GitHub
Git permite llevar un control de las diferentes versiones del proyecto.
GitHub se utiliza como repositorio remoto para almacenar y organizar los archivos del proyecto, además de facilitar el trabajo colaborativo y el seguimiento de cambios.
El repositorio también funciona como espacio para conservar la documentación técnica, el manual de usuario y el plan de pruebas.
6.6 Trello
Trello fue utilizado para organizar las actividades del proyecto y realizar seguimiento al trabajo pendiente.
El tablero permite visualizar las tareas y facilitar la organización del equipo durante el desarrollo.
6.7 draw.io
draw.io se utiliza para la elaboración de diagramas que permiten representar gráficamente diferentes aspectos del sistema.
Entre ellos se encuentra el diagrama de casos de uso, utilizado para identificar actores y funcionalidades.
6.8 Excel
Excel fue utilizado para elaborar y organizar el cronograma del proyecto.
Permite visualizar las actividades, responsables, tiempos y distribución del trabajo.

7. Modelo de información
La información principal que debe manejar PizzaExpress puede organizarse en las siguientes entidades:
Usuario
Contiene información de los usuarios que tienen acceso al sistema.
Rol
Define los permisos y funcionalidades disponibles para cada tipo de usuario.
Producto
Representa los productos ofrecidos por la pizzería.
Ingrediente
Representa los elementos necesarios para preparar los productos.
Pedido
Almacena la información general de cada pedido realizado.
DetallePedido
Permite registrar los productos y cantidades incluidos en cada pedido.
Inventario
Contiene las existencias disponibles de ingredientes y productos.
Entrega
Registra información relacionada con la entrega o recepción de productos.
Venta
Permite almacenar la información necesaria para la generación de reportes de ventas.

8. Flujo general del sistema
El funcionamiento general propuesto para PizzaExpress es el siguiente:
Usuario → Inicio de sesión → Validación de rol → Funcionalidades autorizadas → Procesamiento de operación → Actualización de información → Resultado
Por ejemplo, para registrar un pedido:
Empleado → Iniciar sesión → Registrar pedido → Seleccionar productos → Confirmar pedido → Calcular valor → Descontar ingredientes → Actualizar inventario → Verificar nivel mínimo → Generar alerta si corresponde
Este flujo permite relacionar el proceso de ventas con el control del inventario.

9. Seguridad y control de acceso
PizzaExpress contempla mecanismos básicos de seguridad para controlar el acceso a la información.
Entre ellos:
•	Autenticación mediante usuario y contraseña.
•	Control de acceso según el rol.
•	Restricción de funcionalidades no autorizadas.
•	Validación de información ingresada.
•	Protección de las operaciones administrativas.
El control basado en roles permite reducir el riesgo de que un usuario realice operaciones que no corresponden a sus responsabilidades.

10. Gestión de inventario
El inventario constituye uno de los componentes principales del sistema.
Cuando se registra un pedido confirmado, el sistema debe identificar los ingredientes necesarios para elaborar los productos solicitados y actualizar las cantidades disponibles.
Ejemplo:
Si un pedido requiere:
•	2 unidades de harina.
•	1 unidad de queso.
•	1 unidad de salsa.
El sistema debe descontar esas cantidades de las existencias correspondientes.
Cuando una existencia llega al nivel mínimo establecido, el sistema puede generar una alerta para facilitar la reposición.

11. Gestión de errores
La aplicación debe validar las operaciones antes de almacenar información.
Algunos posibles errores son:
•	Usuario o contraseña incorrectos.
•	Campos obligatorios sin completar.
•	Cantidades inválidas.
•	Producto inexistente.
•	Inventario insuficiente.
•	Usuario sin permisos.
•	Información de entrega incompleta.
Cuando se presente un error, el sistema debe mostrar un mensaje claro para que el usuario pueda identificar la situación y corregirla.

12. Control de versiones
Git se utiliza como sistema de control de versiones.
El repositorio de GitHub permite mantener organizada la evolución del proyecto.
Se recomienda:
1.	Crear cambios relacionados con una funcionalidad específica.
2.	Utilizar mensajes de commit claros.
3.	Evitar eliminar información importante sin autorización.
4.	Mantener organizada la estructura del repositorio.
5.	Revisar los cambios antes de confirmarlos.
6.	Conservar la documentación junto con el proyecto.

13. Documentación del proyecto
La documentación de PizzaExpress se organiza dentro del repositorio de GitHub.
La estructura propuesta es:
PizzaExpress/
│
├── LEAME.md
│
├── 01_Plan_de_Pruebas/
│   ├── Plan_de_Pruebas.md
│   └── Evidencias/
│
├── 02_Documentacion/
│   ├── Manual_de_Usuario.md
│   └── Documentacion_Tecnica.md
│
├── 03_Gestion_Post_Proyecto/
│   └── Estrategia_Seguimiento_Soporte.md
│
└── 04_Anexos/
    └── Diagramas/
Esta organización permite encontrar fácilmente cada documento relacionado con el proyecto.

14. Integración con herramientas de gestión
El proyecto también utiliza herramientas de apoyo para organizar el trabajo.
GitHub
Se utiliza para almacenar y controlar los archivos y documentación del proyecto.
Trello
Se utiliza para gestionar las actividades y tareas del equipo.
draw.io
Se utiliza para representar gráficamente los componentes y procesos del sistema.
Excel
Se utiliza para la planificación temporal del proyecto.
La combinación de estas herramientas permite mejorar la organización y trazabilidad del trabajo.

15. Mantenimiento técnico
Después de la entrega del sistema se recomienda realizar actividades periódicas de mantenimiento.
Estas actividades pueden incluir:
•	Corrección de errores.
•	Actualización de dependencias.
•	Revisión de seguridad.
•	Optimización del sistema.
•	Copias de seguridad.
•	Revisión de la base de datos.
•	Incorporación de nuevas funcionalidades.
Todo cambio importante debe registrarse en el sistema de control de versiones.

16. Conclusión
La arquitectura y las tecnologías propuestas para PizzaExpress buscan proporcionar una solución organizada, mantenible y escalable para la gestión de pedidos e inventario de una pizzería.
La utilización de Python y Django permite estructurar el desarrollo de la aplicación, mientras que GitHub, Trello, draw.io y Excel facilitan la gestión, documentación y seguimiento del proyecto.
La separación de responsabilidades, el control de acceso por roles y la integración entre pedidos e inventario permiten establecer una base técnica adecuada para futuras mejoras y ampliaciones del sistema.

