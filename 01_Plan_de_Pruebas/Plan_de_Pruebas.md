Plan de Pruebas del Sistema – PizzaExpress
1. Introducción

El presente Plan de Pruebas tiene como finalidad establecer las actividades, criterios y casos de prueba necesarios para verificar el correcto funcionamiento del sistema PizzaExpress: Sistema de Gestión de Pedidos e Inventario.

Las pruebas se plantean sobre las funcionalidades definidas para el proyecto, con el propósito de identificar posibles errores, validar el cumplimiento de los requisitos y garantizar que el sistema sea confiable, funcional y fácil de utilizar.

Las evidencias incluidas en este documento corresponden a resultados simulados, de acuerdo con lo solicitado en la actividad académica.

2. Objetivo

Evaluar el funcionamiento de las principales funcionalidades del sistema PizzaExpress mediante diferentes tipos de pruebas, verificando que los procesos de autenticación, gestión de pedidos, inventario, entregas, usuarios, roles y reportes respondan de acuerdo con los requisitos establecidos.

Objetivos específicos
Verificar el inicio de sesión de los usuarios.
Validar el registro y gestión de usuarios y roles.
Comprobar el registro y gestión de pedidos.
Verificar el descuento automático de ingredientes del inventario.
Validar las alertas generadas cuando el inventario alcance niveles bajos.
Comprobar el proceso de validación de entregas.
Verificar la generación y consulta de informes de ventas.
Identificar posibles errores que puedan afectar la calidad del sistema.
3. Alcance

El plan contempla las principales funcionalidades definidas para PizzaExpress:

Autenticación de usuarios.
Gestión de usuarios y roles.
Registro y gestión de pedidos.
Gestión de inventarios.
Descuento automático de ingredientes.
Alertas de inventario.
Validación de entregas.
Consulta de informes de ventas.

No se incluyen en este plan funcionalidades que fueron establecidas fuera del alcance inicial del MVP, como:

Pagos en línea.
Aplicación independiente de domicilios con GPS.
Programa de fidelización.
4. Estrategia de pruebas

La estrategia combina diferentes tipos de pruebas para evaluar el sistema desde distintos niveles.

4.1 Pruebas funcionales

Permiten verificar que cada funcionalidad cumpla con el comportamiento esperado según los requisitos definidos.

4.2 Pruebas unitarias

Se enfocan en comprobar componentes individuales del sistema, como funciones de autenticación, cálculo de pedidos, actualización de inventario y generación de alertas.

4.3 Pruebas de integración

Permiten comprobar la interacción entre diferentes módulos. Por ejemplo, verificar que al registrar un pedido se actualice correctamente el inventario.

4.4 Pruebas de estrés

Buscan evaluar el comportamiento del sistema ante una cantidad elevada de solicitudes o usuarios simultáneos, con el propósito de identificar posibles problemas de rendimiento.

4.5 Pruebas de aceptación

Permiten verificar que las funcionalidades desarrolladas respondan a las necesidades definidas para los usuarios del sistema.

5. Ambiente de pruebas

Para las pruebas se plantea el siguiente ambiente:

Sistema: PizzaExpress.
Tipo de aplicación: Sistema de gestión de pedidos e inventario.
Base de datos: Base de datos definida para el proyecto.
Usuarios de prueba: Administrador, empleado y distribuidor.
Datos: Usuarios, productos, ingredientes, pedidos y ventas ficticias.
Entorno: Ambiente de desarrollo/pruebas.

Los datos utilizados durante las pruebas deben ser ficticios y no contener información personal real.

6. Casos de prueba
CP-01 – Inicio de sesión exitoso

Objetivo:
Verificar que un usuario registrado pueda ingresar al sistema.

Precondición:
El usuario debe encontrarse registrado.

Datos de entrada:
Usuario y contraseña válidos.

Procedimiento:

Abrir el sistema.
Ingresar el usuario.
Ingresar la contraseña.
Seleccionar la opción de iniciar sesión.

Resultado esperado:
El sistema valida las credenciales y permite el acceso según el rol del usuario.

Resultado simulado:
Exitoso.

Estado:
Aprobado.

CP-02 – Inicio de sesión con credenciales incorrectas

Objetivo:
Verificar el comportamiento del sistema cuando se ingresan credenciales incorrectas.

Datos de entrada:
Usuario registrado y contraseña incorrecta.

Procedimiento:

Abrir el formulario de inicio de sesión.
Ingresar el usuario.
Ingresar una contraseña incorrecta.
Intentar iniciar sesión.

Resultado esperado:
El sistema debe rechazar el acceso y mostrar un mensaje indicando que las credenciales no son válidas.

Resultado simulado:
El acceso fue rechazado correctamente.

Estado:
Aprobado.

CP-03 – Gestión de usuarios y roles

Objetivo:
Verificar que el usuario autorizado pueda crear, modificar o eliminar usuarios y asignar roles.

Precondición:
Iniciar sesión con permisos administrativos.

Procedimiento:

Ingresar al módulo de usuarios.
Crear un usuario de prueba.
Asignar un rol.
Guardar la información.
Modificar los datos del usuario.
Verificar los cambios.

Resultado esperado:
El sistema debe permitir gestionar los usuarios de acuerdo con los permisos del administrador.

Resultado simulado:
La gestión de usuarios y roles funcionó correctamente.

Estado:
Aprobado.

CP-04 – Registro de pedido

Objetivo:
Verificar que un empleado pueda registrar un pedido.

Precondición:
El empleado debe haber iniciado sesión.

Procedimiento:

Ingresar al módulo de pedidos.
Seleccionar los productos solicitados.
Registrar la información del pedido.
Confirmar el pedido.

Resultado esperado:
El sistema debe registrar correctamente el pedido y mostrar la información correspondiente.

Resultado simulado:
Pedido registrado correctamente.

Estado:
Aprobado.

CP-05 – Actualización automática del inventario

Objetivo:
Verificar que el inventario se actualice después de registrar un pedido.

Precondición:
Deben existir ingredientes disponibles.

Procedimiento:

Consultar la cantidad disponible de un ingrediente.
Registrar un pedido que utilice dicho ingrediente.
Confirmar el pedido.
Consultar nuevamente el inventario.

Resultado esperado:
La cantidad del ingrediente debe disminuir de acuerdo con los productos incluidos en el pedido.

Resultado simulado:
El inventario fue actualizado correctamente.

Estado:
Aprobado.

CP-06 – Alerta de inventario bajo

Objetivo:
Verificar que el sistema genere una alerta cuando un ingrediente alcance el nivel mínimo establecido.

Procedimiento:

Registrar un pedido que reduzca la cantidad disponible.
Verificar el nivel de inventario.
Compararlo con el nivel mínimo establecido.

Resultado esperado:
El sistema debe generar una alerta indicando que el ingrediente requiere reposición.

Resultado simulado:
Alerta generada correctamente.

Estado:
Aprobado.

CP-07 – Validación de entrega

Objetivo:
Verificar que una entrega pueda ser validada correctamente.

Precondición:
Debe existir un pedido pendiente de entrega.

Procedimiento:

Consultar el pedido pendiente.
Verificar la información de la entrega.
Registrar la validación.
Confirmar el proceso.

Resultado esperado:
El sistema debe actualizar el estado del pedido como entregado o validado.

Resultado simulado:
Entrega validada correctamente.

Estado:
Aprobado.

CP-08 – Consulta de reporte de ventas

Objetivo:
Verificar que un usuario autorizado pueda consultar los reportes de ventas.

Precondición:
Deben existir registros de ventas.

Procedimiento:

Iniciar sesión con un usuario autorizado.
Ingresar al módulo de informes.
Seleccionar el informe de ventas.
Consultar la información.

Resultado esperado:
El sistema debe mostrar la información correspondiente a las ventas registradas.

Resultado simulado:
Reporte generado y consultado correctamente.

Estado:
Aprobado.

CP-09 – Restricción de acceso según rol

Objetivo:
Verificar que cada usuario solamente pueda acceder a las funcionalidades autorizadas para su rol.

Procedimiento:

Iniciar sesión con un usuario de prueba.
Intentar acceder a una funcionalidad restringida.
Verificar la respuesta del sistema.

Resultado esperado:
El sistema debe impedir el acceso a funcionalidades no autorizadas.

Resultado simulado:
El acceso fue restringido correctamente.

Estado:
Aprobado.

CP-10 – Prueba de estrés

Objetivo:
Evaluar el comportamiento general del sistema ante una cantidad elevada de solicitudes.

Procedimiento simulado:

Simular múltiples solicitudes de consulta y registro.
Observar el comportamiento del sistema.
Verificar la disponibilidad de los módulos principales.

Resultado esperado:
El sistema debe mantener un comportamiento estable y responder dentro de tiempos aceptables.

Resultado simulado:
El sistema mantuvo su disponibilidad durante la prueba simulada.

Estado:
Aprobado.

7. Resumen de resultados
ID	Prueba	Resultado simulado	Estado
CP-01	Inicio de sesión exitosa	Funcionó correctamente	Aprobado
CP-02	Credenciales incorrectas	Acceso rechazado	Aprobado
CP-03	Usuarios y roles	Gestión correcta	Aprobado
CP-04	Registro de pedido	Pedido registrado	Aprobado
CP-05	Actualización de inventario	Inventario actualizado	Aprobado
CP-06	Alerta de inventario	Alerta generada	Aprobado
CP-07	Validación de entrega	Entrega validada	Aprobado
CP-08	Reporte de ventas	Reporte generado	Aprobado
CP-09	Restricción por roles	Acceso restringido	Aprobado
CP-10	Prueba de estrés	Comportamiento estable	Aprobado
Resultado general
Total de casos de prueba: 10
Casos aprobados: 10
Casos con resultado no aprobado: 0
Porcentaje de aprobación simulado: 100 %
8. Evidencias simuladas

De acuerdo con las instrucciones de la actividad, se presentan resultados simulados de las pruebas realizadas.

Las evidencias pueden representarse mediante capturas simuladas de:

Pantalla de inicio de sesión exitosa.
Mensaje de credenciales incorrectas.
Gestión de usuarios y roles.
Registro de un pedido.
Inventario antes y después de registrar un pedido.
Alerta de inventario bajo.
Validación de una entrega.
Reporte de ventas.
Restricción de acceso por rol.
Resultado de la prueba de estrés.

Nota: Las evidencias son de carácter académico y simulado. No representan datos reales de clientes, empleados o proveedores.

9. Criterios de aceptación

Se considera que una funcionalidad cumple con los criterios de aceptación cuando:

Ejecuta el proceso solicitado correctamente.
Presenta información coherente al usuario.
Controla los errores de entrada.
Respeta los permisos establecidos según el rol.
Mantiene la información registrada correctamente.
No afecta negativamente otras funcionalidades del sistema.

Para considerar el sistema aceptable dentro del escenario académico, se establece como referencia que los casos de prueba críticos deben presentar un resultado satisfactorio.

10. Gestión de errores

Cuando una prueba presente un resultado no esperado, se deberá:

Registrar el error.
Describir los pasos para reproducirlo.
Identificar el módulo afectado.
Clasificar su prioridad.
Asignar un responsable.
Realizar la corrección.
Ejecutar nuevamente la prueba.
Registrar el nuevo resultado.
11. Conclusiones

El Plan de Pruebas permite establecer un procedimiento organizado para evaluar las funcionalidades principales de PizzaExpress.

Los casos definidos abarcan aspectos relacionados con autenticación, permisos, pedidos, inventario, entregas e informes, además de pruebas unitarias, de integración, estrés y aceptación.

Los resultados presentados son simulados, tal como establece la actividad académica, y permiten evidenciar la aplicación de un proceso estructurado de aseguramiento de calidad.

La implementación de este plan contribuye a identificar posibles errores, mejorar la confiabilidad del sistema y facilitar su mantenimiento durante las etapas posteriores del proyecto.
