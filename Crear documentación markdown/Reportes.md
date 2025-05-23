# Reportes

### Instalación de los paquetes necesarios

Para poder generar un reporte en Windows Forms, es necesario instalar el **control de ReportViewer**. Esto se realiza desde el **Administrador de paquetes NuGet**, buscando e instalando el paquete llamado:

* **Microsoft.Reporting.WinForms**

Este paquete permite incorporar el visor de reportes dentro del formulario y vincularlo con los datos provenientes del sistema o base de datos.

### Creación del formulario de reportes

Se debe agregar un nuevo formulario al proyecto, el cual se utilizará exclusivamente para mostrar el reporte.&nbsp;

### Agregar el control ReportViewer

Dentro del nuevo formulario, se debe arrastrar el control **ReportViewer** desde la caja de herramientas (Toolbox) hacia el formulario. Este control se ajusta al tamaño deseado para que ocupe todo el espacio visible.

Posteriormente, es necesario hacer clic en la pequeña flecha de configuración del control y seleccionar la opción **"Elegir un informe"**, lo cual permite vincularlo con un archivo .rdlc.

![Image](<lib/Nuevo tem 9.png>)

### Crear el archivo del reporte (.rdlc)

A continuación, se debe agregar un nuevo archivo de tipo **"Informe"** al proyecto, con extensión .rdlc. Este archivo permitirá diseñar visualmente cómo se mostrará la información del reporte.

Durante su diseño, se agregan los campos deseados a través de una tabla o matriz, arrastrándolos desde el **origen de datos del informe**.

![Image](<lib/Nuevo tem 35.png>)

### Creación del Dataset

Es necesario crear un **Dataset tipado**, que actúe como puente entre la base de datos y el reporte. Este Dataset debe tener un **DataTable** con columnas que coincidan con los nombres y tipos de los campos en la base de datos.

El Dataset también define una **consulta de selección**, que puede traer todos los registros de la tabla **Factura** o aplicar filtros si se desea.

![Image](<lib/Nuevo tem 11.png>)

### Configuración de los orígenes de datos

En el archivo **.rdlc,** se debe configurar el origen de datos del informe para que utilice el Dataset creado. Esto se hace desde la opción **"Orígenes de datos del informe"**, vinculando el reporte con el DataTable definido.

### Botón para mostrar el reporte

En el formulario principal, se debe agregar un botón con una función que abra el formulario del reporte. Este botón simplemente crea una nueva instancia del formulario de reporte y lo muestra con el método .**Show() o .ShowDialog().**

### ![Image](<lib/Nuevo tem 34.png>)

### Visualización del reporte

Al ejecutar la aplicación y hacer clic en el botón correspondiente, se abre el formulario que contiene el ReportViewer, y este muestra todos los datos de la tabla Factura de forma estructurada y profesional, ideal para imprimir o guardar como PDF.

&nbsp;

![Image](<lib/Nuevo tem 33.png>)

***
_Creado con el Personal Edition de HelpNDoc: [Generador de documentación y EBooks gratuito](<https://www.helpndoc.com/es/>)_
