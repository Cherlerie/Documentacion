# Descripcion

#### Entorno de Desarrollo

El desarrollo de este módulo se realizó en **Visual Studio**, utilizando el lenguaje **C#** bajo el enfoque de **aplicación de escritorio** con **Windows Forms**. La base de datos utilizada fue **SQL Server**, gestionada mediante SQL Server Management Studio.

![Image](<lib/Nuevo tem 26.png>)&nbsp; ![Image](<lib/Nuevo tem 27.png>)

#### Arquitectura del Sistema

El sistema se estructura en **tres capas básicas**:

* **Capa de Vista**: formularios que interactúan con el usuario.

![Image](<lib/Nuevo tem 23.png>)

* **Capa de Controlador**: contiene la lógica del programa (clases que procesan datos y validaciones).

&nbsp;

![Image](<lib/Nuevo tem 24.png>)

* **Capa de Modelo**: maneja la conexión con SQL Server y ejecuta consultas.

![Image](<lib/Nuevo tem 25.png>)

Esta arquitectura facilita el mantenimiento y escalabilidad del sistema.

#### Dependencias

El proyecto utiliza las siguientes dependencias:

* **Microsoft.ReportViewer.WinForms**: para la generación de reportes.
* **System.Data.SqlClient**: para la conexión con la base de datos.

***
_Creado con el Personal Edition de HelpNDoc: [Agilice su proceso de documentación con la función de conversión WinHelp HLP a CHM de HelpNDoc](<https://www.helpndoc.com/es/guias-paso-a-paso/c%C3%B3mo-convertir-un-archivo-de-ayuda-hlp-winhelp-en-un-archivo-de-ayuda-chm-html-help/>)_
