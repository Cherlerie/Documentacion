# Reportes

## Generación del Reporte con DOMPDF en PHP

Para generar el reporte en formato PDF se utilizó la biblioteca **DOMPDF**, que permite convertir contenido HTML en archivos PDF desde PHP de forma sencilla.

### Inclusión de DOMPDF

En lugar de usar Composer, la biblioteca DOMPDF fue descargada manualmente desde su sitio oficial. Luego, se descomprimió y se colocó dentro del proyecto PHP. Se incluyó en el archivo mediante require o require\_once, apuntando directamente a la ruta del archivo autoload o del archivo principal de la librería.

### Página Principal

Se creó una página PHP sencilla con un enlace que indica “Descargar reporte” o “Descargar PDF”. Al hacer clic, se redirige a otro archivo que es el encargado de generar el reporte.

![Image](<lib/Nuevo tem 38.png>)

### Generación del Reporte

El archivo que genera el PDF realiza las siguientes tareas:

* Se conecta a la base de datos utilizada (diferente a la del proyecto en C#).
* Se ejecuta una consulta que selecciona todos los registros de una tabla.
* Se construye una estructura HTML con los datos, generalmente en forma de tabla.
* Se configura el tamaño y orientación del PDF.
* Se usa DOMPDF para cargar ese HTML, renderizarlo y generar el PDF.
* Finalmente, se envía el archivo al navegador con encabezados HTTP que fuerzan su descarga.

![Image](<lib/Nuevo tem 37.png>)

### Estilo del PDF

El contenido HTML incluye etiquetas básicas de formato como tablas.

![Image](<lib/Nuevo tem 36.png>)

***
_Creado con el Personal Edition de HelpNDoc: [Actualice sin esfuerzo sus archivos de ayuda WinHelp HLP a CHM con HelpNDoc](<https://www.helpndoc.com/es/guias-paso-a-paso/c%C3%B3mo-convertir-un-archivo-de-ayuda-hlp-winhelp-en-un-archivo-de-ayuda-chm-html-help/>)_
