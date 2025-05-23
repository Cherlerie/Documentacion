# Base de datos

### Nombre de la base de datos: Factura

La base de datos creada para este sistema lleva por nombre **Factura**. Esta base de datos se encarga de almacenar la información relacionada con las facturas ingresadas desde el formulario, facilitando la gestión de los registros.

&nbsp;

### Tabla principal: Factura

Dentro de esta base de datos se creó una única tabla, también llamada **Factura**, la cual contiene los campos esenciales para el registro de cada factura. Entre los campos se encuentran:

* Un identificador único llamado **ID**, que se genera automáticamente.
* El campo **DESCRIPCION**, donde se indica el nombre del producto o servicio facturado.
* La **CATEGORIA**, que clasifica el tipo de producto.
* La **CANTIDAD**, que representa cuántas unidades se están facturando.
* El **PRECIO\_UNITARIO**, correspondiente al valor por unidad.
* El campo **ITEBIS**, que almacena el valor del impuesto aplicado.
* Y finalmente, el campo **DESCUENTO**, que refleja cualquier rebaja otorgada al total.

![Image](<lib/Nuevo tem 29.png>)

&nbsp;

### Inserción de datos de prueba

Una vez creada la base de datos y la tabla, se procedió a insertar registros de ejemplo para verificar que la estructura funciona correctamente. Estos datos permiten realizar pruebas de lectura, edición y eliminación desde el sistema.

![Image](<lib/Nuevo tem 30.png>)

### Visualización de los datos

Para verificar los datos almacenados, se puede ejecutar una consulta que muestre todos los registros de la tabla. Esto permite comprobar que los datos ingresados desde el formulario se reflejan correctamente en la base de datos

![Image](<lib/Nuevo tem 31.png>)

### Nombre del servidor y conexión

### El nombre del servidor se obtiene al iniciar sesión en SQL Server Management Studio. Es importante usar este nombre exacto en la cadena de conexión del proyecto para garantizar la comunicación entre la aplicación y la base de datos.

![Image](<lib/Nuevo tem 28.png>)


***
_Creado con el Personal Edition de HelpNDoc: [Crear fácilmente EBooks](<https://www.helpndoc.com/es/descubrir-funciones/>)_
