# spark
Tutorial sobre la instalación y uso de Spark

Apache Spark es un framework (conjunto de herramientas) usadas en el entorno de agrupación computacional para el análisis de big data.

En este tutorial, se mostrará como instalar Spark en una distribución Debian 12. La guia muestra como inicializar un servidor maestro (master) y trabajador (slave), y como cargar las terminales (shells) de Scala y Python. Así como los principales comandos de Spark.

Prerequisitos
Un SO Debian o sus derivadas.
Acceso a la linea de comandos o terminal. En este ejercicio utilizaremos la herramienta MobaXTerm.
Un usuario con permisos sudo o root.
Instalar los paquetes requeridos por Spark
Antes de descargar y configurar Spark, necesitamos instalar dependencias. Estos pasos incluyen la instalación de la siguiente paquetería.

JDK
Scala
Git
Abrimos una terminal y corremos el siguiente comando para la instalación de las tres paqueterías a la vez:

sudo apt install default-jdk scala git -y
Una vez que el proceso este completado, verifica que las dependencias estén instaladas corriendo el siguiente comando:

java -version; javac -version; scala -version; git --version
Se imprimirán las salida con la versiones correspondientes, si la instalación por todos las paqueterías fue exitosa.

Descargar y Configurar Spark en Debian o Ubuntu.
Ahora, necesitamos descargar la versión de Spark que quieras y este disponible desde el sitio web oficial. Al momento de editar este texto la versión más actualizada es Spark 3.5.1 (Junio-09-2024) conjuntamente con la paquetería Hadoop 3.3.
Verificar las últimas versiones en la URL: https://spark.apache.org/downloads.html

Usamos el comando wget junto con la liga del sitio para la descarga de nuestro archivo Spark:

wget https://dlcdn.apache.org/spark/spark-3.5.1/spark-3.5.1-bin-hadoop3.3.tgz
