Proyecto de Reserva de Espacios de Coworking

Este proyecto es una aplicación web basada en Java Servlets para gestionar reservas. Permite que los uauarios hagan reservas, listar las reservas que existen y eliminarlas.

1. Estructura del Proyecto

ProyectoReservaCoworking/
│── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── servlets/
│   │   │   │   ├── EliminarReservaServlet.java
│   │   │   │   ├── ListaReservasServlet.java
│   │   │   │   ├── ReservaServlet.java
│── webapp/
│   ├── META-INF/
│   ├── WEB-INF/
│   ├── index.html
│   ├── reservas.jsp
│   ├── styles.css

El código está completamente documentado con comentarios en cada clase y método para mayor claridad.

#2. Despliegue en NetBean

Este proyecto lo vamos a despleguar en **NetBeans** con un servidor **Apache Tomcat** :

-Versiones:
Antes de comenzar, asegúrate de tener instalado:

- *Java JDK 8 o superior
- Apache Tomcat 9 o superior
- NetBeans IDE preferiblemente el 19, con soporte para Java EE
- Git (opcional, para clonar el repositorio directamente)

#3Pasos para el despliegue

1. **Clonar el repositorio:
   Si tienes Git instalado, abre la terminal y ejecuta:
   git clone https://github.com/nikev222/ProyectoReservaCoworking.git
   O bien, descarga el proyecto en formato ZIP desde GitHub y extráelo en tu equipo.

2. **Abrir el proyecto en NetBeans:
   - Abre NetBeans y selecciona `Archivo` -> `Abrir Proyecto`.
   - Busca la carpeta `ProyectoReservaCoworking` y ábrela.

3. **Configurar Apache Tomcat en NetBeans:
   - Ve a `Herramientas` -> `Servidores`.
   - Agrega un nuevo servidor Apache Tomcat y selecciona la ruta donde está instalado.

4. **Compilar y ejecutar el proyecto:
   - En la pestaña `Proyectos`, haz clic derecho sobre `ProyectoReservaCoworking` y selecciona `Limpiar y Construir`.
   - Luego, dale clic en ejecutar para iniciar el proyecto

5. **Acceder a la aplicación:**
   Una vez que el servidor esté en ejecución se abrira un navegador al index.html o accede directamnente con:
   http://localhost:8080/ProyectoReservaCoworking/index.html


4.Funcionalidades Principales
- Realizar reservas:el usuario llena el formulario con los datos para realizar un reserva.
- Listar reservas:Visualizar los datos de todas las reservas en una tabla.
- Eliminar reservas:Opción para eliminar reservas seleccionadas.

5.Desafio encontrado
 -Al eliminar una reserva, la lista no se actualizaba correctamente y seguia mostrando las reservas eliminadas. 
 -Para solucionar esto, se aseguro que la lista se recargara despues de cada operacion, actualizando la informacion en la interfaz de usuario.



