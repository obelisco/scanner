scanner
=======

Analizador Léxico de Código XHTML

TAREA PROGRAMADA I  

Introducción
El objetivo de esta tarea es familiarizarse con los conceptos relativos a la fase de análisis léxico de un compilador, mediante el desarrollo de un scanner para XHTML
Para efectos de esta tarea, se podrá usar Flex o JFlex para generar el analizador léxico. El programa deberá transformar el código XHTML a una serie de tokens que tengan información que será usada en las siguientes fases del procesamiento.

Descripción del programa
Deberán escribir una especificación de Flex o JFlex para construir un scanner para XHTML. Los estudiantes deberán investigar la especificación estándar de XHTML, definir la lista de tokens que van a manejar, y generar las ER, y las acciones asociadas a esas ER, para procesar los tokens.
Deben tomar en cuenta que la información recopilada por el scanner en el análisis léxico va a ser usada por el analizador sintáctico, por lo que deben guardar toda la información relevante en las variables de Flex/JFlex, para que posteriormente puedan ser usadas por el parser (yylen, etc.)
El programa no deberá usar argumentos de línea de comandos, solamente deberá ser un ejecutable que reciba la entrada del stdin, escriba los tokens resultantes al stdout, y reporte errores al stderr.
Como parte de la entrega, deberán tener un archivo MAKEFILE (en el caso de java podrían usar ANT o MAVEN, de forma alternativa) que tenga todas las instrucciones necesarias para compilar/ configurar el programa, de manera que con solo los archivos entregados, se pueda ejecutar el comando MAKE, y se generen automáticamente los ejecutables de la tarea.
Para invocar el programa, se deberá ejecutar el siguiente comando (asumiendo que el MAKEFILE construye el archivo scanner):
./scanner <  archivoFuente

