Manual de Usuario – PizzaExpress
1. Introducción
PizzaExpress es un sistema de gestión de pedidos e inventario diseñado para apoyar las actividades operativas de una pizzería.
El sistema permite gestionar pedidos, controlar el inventario de ingredientes, administrar usuarios y roles, validar entregas y consultar reportes de ventas.
Este manual tiene como objetivo orientar a los usuarios en el uso de las principales funcionalidades del sistema.

2. Objetivo del manual
Explicar de manera clara y sencilla el funcionamiento de PizzaExpress y proporcionar una guía para que los diferentes usuarios puedan utilizar correctamente las funcionalidades disponibles de acuerdo con su rol.

3. Usuarios del sistema
PizzaExpress contempla diferentes tipos de usuarios:
3.1 Administrador
Es el usuario encargado de la administración general del sistema.
Puede:
•	Gestionar usuarios.
•	Asignar y modificar roles.
•	Consultar reportes de ventas.
•	Supervisar el inventario.
•	Autorizar determinadas acciones.
•	Consultar el estado general de los pedidos.
3.2 Empleado
Es el usuario encargado de las actividades operativas de la pizzería.
Puede:
•	Iniciar sesión.
•	Registrar pedidos.
•	Consultar y actualizar información relacionada con los pedidos.
•	Gestionar determinadas operaciones del inventario.
•	Validar entregas según los permisos asignados.
3.3 Distribuidor
Es el usuario relacionado con la recepción o entrega de productos e insumos.
Puede:
•	Consultar información relacionada con las entregas.
•	Registrar o validar la entrega de productos.
•	Actualizar la información correspondiente a los productos recibidos.

4. Requisitos para utilizar el sistema
Para utilizar PizzaExpress se requiere:
•	Un computador o dispositivo con acceso al sistema.
•	Usuario y contraseña registrados.
•	Permisos de acuerdo con el rol asignado.
•	Acceso a la aplicación.

5. Inicio de sesión
El inicio de sesión permite controlar el acceso al sistema.
Pasos:
1.	Abrir PizzaExpress.
2.	Ingresar el nombre de usuario.
3.	Ingresar la contraseña.
4.	Seleccionar la opción Iniciar sesión.
5.	El sistema valida las credenciales.
6.	Si los datos son correctos, permite el acceso a las funcionalidades correspondientes al rol del usuario.
En caso de datos incorrectos
Si el usuario introduce credenciales incorrectas, el sistema debe mostrar un mensaje indicando que los datos no son válidos y no permitir el acceso.

6. Gestión de usuarios y roles
Esta funcionalidad está principalmente dirigida al administrador.
Permite controlar los usuarios que tienen acceso al sistema y los permisos asociados a cada uno.
Crear un usuario
1.	Ingresar al sistema como administrador.
2.	Seleccionar la opción Usuarios.
3.	Seleccionar Crear usuario.
4.	Registrar los datos solicitados.
5.	Asignar el rol correspondiente.
6.	Guardar la información.
Modificar un usuario
1.	Ingresar al módulo de usuarios.
2.	Buscar el usuario.
3.	Seleccionar la opción Modificar.
4.	Actualizar la información necesaria.
5.	Guardar los cambios.
Eliminar un usuario
1.	Buscar el usuario que se desea eliminar.
2.	Seleccionar la opción Eliminar.
3.	Confirmar la operación.
El sistema debe solicitar confirmación antes de eliminar un usuario.

7. Registro de pedidos
Esta es una de las funcionalidades principales de PizzaExpress.
Permite registrar pedidos realizados por los clientes.
Pasos:
1.	Ingresar al sistema.
2.	Seleccionar Pedidos.
3.	Seleccionar Nuevo pedido.
4.	Registrar la información del cliente o mesa.
5.	Seleccionar los productos solicitados.
6.	Indicar las cantidades.
7.	Seleccionar el tipo de pedido:
o	En mesa.
o	Para llevar.
o	Domicilio.
8.	Revisar la información.
9.	Confirmar el pedido.
El sistema debe registrar el pedido y calcular el valor correspondiente.

8. Gestión del inventario
El módulo de inventario permite controlar los ingredientes y productos utilizados por la pizzería.
Entre los elementos que pueden ser controlados se encuentran:
•	Harina.
•	Queso.
•	Salsa.
•	Carnes.
•	Vegetales.
•	Otros ingredientes necesarios para la elaboración de las pizzas.
Actualización del inventario
Cuando se reciben nuevos productos o ingredientes:
1.	Ingresar al módulo Inventario.
2.	Seleccionar el producto.
3.	Registrar la cantidad recibida.
4.	Guardar la actualización.
El sistema debe reflejar la nueva cantidad disponible.

9. Descuento automático de ingredientes
Una de las funcionalidades propuestas para PizzaExpress es el descuento automático de los ingredientes utilizados en la preparación de los pedidos.
Cuando se confirma un pedido:
1.	El sistema identifica los productos solicitados.
2.	Consulta los ingredientes asociados.
3.	Calcula las cantidades utilizadas.
4.	Descuenta dichas cantidades del inventario.
5.	Actualiza las existencias disponibles.
Esto permite reducir el riesgo de errores en el control manual del inventario.

10. Alertas de inventario
PizzaExpress contempla alertas cuando la cantidad disponible de un ingrediente alcanza un nivel bajo.
Por ejemplo:
Alerta: El inventario de queso se encuentra por debajo del nivel mínimo establecido.
Esta funcionalidad permite que el administrador o el personal encargado pueda identificar oportunamente la necesidad de realizar una reposición.

11. Validación de entregas
La validación de entregas permite registrar y comprobar la recepción o entrega de productos.
Pasos:
1.	Ingresar al módulo de entregas.
2.	Consultar la entrega correspondiente.
3.	Verificar los productos y cantidades.
4.	Confirmar que la información sea correcta.
5.	Seleccionar Validar entrega.
6.	El sistema registra la operación.
En caso de encontrar inconsistencias, la entrega debe quedar pendiente de revisión.

12. Consulta de reportes de ventas
Esta funcionalidad permite al administrador consultar información relacionada con las ventas realizadas.
Los reportes pueden incluir información como:
•	Pedidos realizados.
•	Productos vendidos.
•	Cantidad de ventas.
•	Valores de las ventas.
•	Información por periodo.
Pasos:
1.	Ingresar al sistema como administrador.
2.	Seleccionar Reportes.
3.	Seleccionar Reporte de ventas.
4.	Definir el periodo que se desea consultar.
5.	Generar el reporte.
6.	Revisar la información obtenida.
Los reportes sirven como apoyo para el análisis y la toma de decisiones del negocio.

13. Restricciones según el rol
PizzaExpress utiliza control de acceso basado en roles.
Esto significa que no todos los usuarios tienen acceso a las mismas funcionalidades.
Por ejemplo:
Funcionalidad	          Administrador	Empleado	Distribuidor
Iniciar sesión	            ✓	          ✓	          ✓
Gestionar usuarios	        ✓          	✗	          ✗
Gestionar roles	            ✓          	✗          	✗
Registrar pedidos	          ✓	          ✓          	✗
Gestionar inventario	      ✓          	✓	      Según permisos
Validar entregas	          ✓          	✓	          ✓
Consultar reportes	        ✓          	✗	          ✗
El sistema debe impedir que un usuario acceda a funcionalidades para las cuales no posee permisos.

14. Cierre de sesión
Para finalizar correctamente el uso del sistema:
1.	Seleccionar la opción Cerrar sesión.
2.	El sistema finalizará la sesión actual.
3.	El usuario será dirigido nuevamente a la pantalla de inicio de sesión.
Se recomienda cerrar sesión cuando se termine de utilizar el sistema.

15. Recomendaciones de uso
Para utilizar correctamente PizzaExpress se recomienda:
•	Mantener las credenciales de acceso protegidas.
•	No compartir la contraseña con otros usuarios.
•	Verificar la información antes de confirmar un pedido.
•	Mantener actualizado el inventario.
•	Revisar periódicamente las alertas de existencias.
•	Validar correctamente las entregas.
•	Consultar los reportes de ventas para realizar seguimiento al negocio.
•	Utilizar únicamente las funcionalidades correspondientes al rol asignado

16. Solución de problemas frecuentes
No puedo iniciar sesión
Verificar que el usuario y la contraseña estén escritos correctamente.
Si el problema continúa, solicitar apoyo al administrador.
No puedo acceder a una función
Es posible que la funcionalidad no esté disponible para el rol asignado.
Consultar con el administrador del sistema.
El inventario no coincide
Verificar los últimos movimientos registrados y revisar las cantidades ingresadas.
No aparece un pedido
Verificar que el pedido haya sido guardado y confirmado correctamente.

17. Conclusión
El sistema PizzaExpress busca facilitar la gestión de las operaciones principales de una pizzería mediante el control de pedidos, usuarios, inventario, entregas y reportes de ventas.
El uso adecuado de cada funcionalidad permite mejorar la organización de la información, reducir errores en los procesos y facilitar la toma de decisiones administrativas.
Este manual proporciona una guía básica para que los usuarios puedan comprender y utilizar las principales funcionalidades propuestas para el sistema.

