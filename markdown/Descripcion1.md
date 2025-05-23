# Descripcion

Este proyecto consiste en una página web simple desarrollada en PHP que permite **generar y descargar un reporte en formato PDF** con todo el contenido de una tabla de base de datos. La generación del PDF se realiza utilizando la librería **DOMPDF**, una herramienta popular en PHP que convierte código HTML y CSS en documentos PDF.

![Image](<lib/Nuevo tem 39.png>)

La interfaz del sistema está compuesta por una sola página funcional con un botón principal identificado como **“Descargar reporte”** o **“Generar PDF”**, el cual, al ser presionado, ejecuta un script PHP que:

* Realiza la conexión a una base de datos MySQL diferente a la usada en el sistema anterior.
* Recupera todos los registros de una tabla específica (por ejemplo, una tabla de facturas o productos).
* Organiza estos datos en una estructura HTML que actúa como plantilla del reporte.
* Convierte dicha plantilla en un documento PDF utilizando DOMPDF.
* Fuerza la descarga del PDF automáticamente o lo abre en una nueva pestaña del navegador, según la configuración establecida.

Este tipo de implementación es ideal para exportar datos a un formato portátil y visualmente organizado, lo que facilita su impresión, archivado o envío por correo electrónico.

El sistema está compuesto por:

* Un archivo principal que muestra el botón.
* Un script que genera el PDF usando DOMPDF.
* Un archivo de conexión a la base de datos.
* La plantilla HTML que define el formato visual del reporte PDF.

***
_Creado con el Personal Edition de HelpNDoc: [¿Qué es una herramienta de creación de documentación de ayuda?](<https://www.helpauthoringsoftware.com>)_
