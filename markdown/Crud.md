# Crud

### Paso 1: Crear el formulario&nbsp;

Abre Visual Studio y crea un proyecto de tipo **Windows Forms App (.NET Framework)**.

Diseña un formulario con los siguientes controles:

* **TextBox** para cada campo: ID, DESCRIPCION, CATEGORIA, CANTIDAD, PRECIO\_UNITARIO, ITEBIS, DESCUENTO .
* **Botones**: Crear, Buscar, Editar, Limpiar.

**DataGridView** para mostrar los datos de la tabla.

![Image](<lib/Nuevo tem 14.png>)

### Paso 2: Conectar con la base de datos

1. Usa la siguiente cadena de conexión para SQL Server local:

csharp

![Image](<lib/Nuevo tem 13.svg>)

string connectionString = "Server=localhost;Database=Factura;Integrated Security=True;";

&nbsp;

2. Esta cadena debe usarse con cada conexión SqlConnection.

&nbsp;

### Paso 3: Insertar datos en la tabla

### En el evento del botón **Crear**, implementa el código para validar y luego insertar datos usando INSERT INTO. Verifica que los campos numéricos como CANTIDAD, PRECIO\_UNITARIO, ITEBIS, DESCUENTO sean válidos antes de ejecutar la consulta.

![Image](<lib/Nuevo tem 15.png>)

![Image](<lib/Nuevo tem 16.png>)

&nbsp;

### Paso 4: Buscar una factura existente

### En el evento del botón **Buscar**, se usa el ID como clave para buscar en la tabla con SELECT \* FROM Factura WHERE ID = @id.Si se encuentra, se llenan los campos del formulario con los datos.

![Image](<lib/Nuevo tem 18.png>)

&nbsp;

![Image](<lib/Nuevo tem 19.png>)

### Paso 5: Editar una factura

### El botón **Editar** permite actualizar los datos de una factura existente, usando el ID como referencia con UPDATE.

![Image](<lib/Nuevo tem 20.png>)

![Image](<lib/Nuevo tem 21.png>)

### Paso 6: Mostrar los datos

### La función CargarDatos() ejecuta una consulta SELECT y carga el resultado en el DataGridView para visualizar todas las facturas registradas.

![Image](<lib/Nuevo tem 22.png>)


***
_Creado con el Personal Edition de HelpNDoc: [Crea sin esfuerzo un sitio web de documentación de calidad profesional con HelpNDoc](<https://www.helpndoc.com/es/descubrir-funciones/producir-paginas-web-html/>)_
