# Base de datos

Para que el sistema funcione correctamente, es necesario contar con una base de datos MySQL que almacene la información que se mostrará en el reporte PDF.

### Creación de la Base de Datos

Primero se debe crear una nueva base de datos desde un gestor como **phpMyAdmin**, **MySQL Workbench**, o directamente desde la consola de MySQL. Esta base de datos se utiliza exclusivamente para este sistema, separada del proyecto en C#.

![Image](<lib/Nuevo tem 43.png>)

### Estructura de la Tabla

Dentro de la base de datos se crea una tabla que contiene los datos a exportar. Esta tabla puede incluir campos como ID, Descripción, Categoría, Cantidad, Precio, entre otros, dependiendo de la naturaleza del reporte que se quiere generar.&nbsp;

![Image](<lib/Nuevo tem 41.png>)

### Inserción de Datos

Una vez creada la tabla, se insertan registros de prueba o datos reales que se desean mostrar en el PDF. Esto puede hacerse manualmente o mediante scripts SQL.

&nbsp;

![Image](<lib/Nuevo tem 42.png>)

***
_Creado con el Personal Edition de HelpNDoc: [Producir ayuda online para aplicaciones Qt](<https://www.helpndoc.com/es/descubrir-funciones/crear-archivos-de-ayuda-para-qt-help-framework/>)_
