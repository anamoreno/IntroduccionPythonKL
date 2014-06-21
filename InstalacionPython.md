#Software para Instalar

Cualquier inconveniente o error, por favor detalladamente escriba un correo a:

alejandro.cardenasa@konradlorenz.edu.co

Esta lista de Software está basada en la proporcionada para el SciCoder (<http://scicoder.org>), 
se escribió y se probó para:

- Mac OS 10.9 Mavericks 
- Ubuntu 14.04 LTS

Nota personal: Muchas veces las personas piensan que su computador personal es muy viejo o lento. La verdad, sí puede ser viejo pero la lentitud es un asunto diferente. Los computadores en general funcionan bien cuando tienen instalado el Sistema Operativo para el cual fueron diseñados. Windows y Mac OS tienen la particularidad de actualizar el sistema para hacerlo más robusto y mejor, aplica más para Mac, y por lo tanto más pesado. El nuevo sistema operativo está diseñado para otra máquina, no para la que usted compró con otro OS. Por eso no recomiendo los Upgrades de sistema. Su computador, no importa de qué año sea servirá perfectamente si instala una versión adecuada de Ubuntu. 

Ahora bien, si usted tiene pensado hacer grandes simulaciones, correr video, imágenes o procesar grandes volúmenes de datos un computador, el mejor del mercado, no le sirve para eso. Para empezar, el mejor computador que se vende en una tienda Mac no tiene ni siquiera el espacio en disco para por ejemplo, almacenar (¡sólo almacenar!) las imagenes de una sola noche de observación de todo el cielo con un telescopio como el Subaru en Hawai (tenga en cuenta que con una sola noche de observación no se hace estadística). 

Escribo esto para que se haga la idea de que la ciencia, la de  frontera en análisis de datos y simulaciones, no se hace en un computador personal. Se corre en centros de cómputo. Sin embargo, el código sí se escribe en computadores personales.  
______________________
#Linux:
Antes de iniciar: Entre a una terminal y digite sudo apt-get update

#Mac:
- Instale Xcode (lo puede hacer desde el App Store).
- Ingrese a Xcode y entre a las preferencias. Desde la pestaña de "Downloads" instale la línea de comandos (Command Line Developer Tools).
	Nota: Para Mavericks es necesario realizar la instalación desde la terminal con el comando xcode-select --install
- Instale Xquartz (http://xquartz.macosforge.org/landing/)

Nota: MacPorts (http://www.macports.org/install.php) solía ser la forma de instalar Python y sus complementos.
Yo no uso Linux. Sin embargo, he leído que en algunas ocasiones, no sé cuáles específicamente, pero sé que no son comunes,
Anaconda no funciona bien. Para el curso no habrá problemas, espero que esas situaciones (exóticas) no ocurran. 
______________________

A continuación describiré el software que se debe traer instalado para el curso.

Software:

______________________
Los usuarios de Linux deben utilizar el comando apt-get o el instalador GUI cuando esté disponible para
el software de esta lista.

# Python
Se necesitará la versión de Python 2.7 o superior. Los sistemas operativos Mac y Linux incluyen la versión requerida.
Sin embargo, se utilizarán paquetes adicionales que no vienen por defecto con el sistema operativo (i.e. numpy, scipy, iPython, etc.)
Instalar los complementos puede ser tedioso, por esa razón recomiendo instalar una distribución independiente de Python en su sistema. 
La ventaja añadida es que, si la instalación de Python se rompe de alguna manera, su sistema no será afectado. 

La distribución recomendada es Anaconda:

https://store.continuum.io/cshop/anaconda/

Es gratis para uso académico, NO hay que pagar por la versión. 

Al descargar Anaconda, la organización solicita un correo electrónico que no será valido. Sin embargo, sugiero utilizar datos correctos para mantenerse al día en las actualizaciones. Así que mejor descargar la versión académica (opcional):

https://store.continuum.io/cshop/academicanaconda

En el formato digite su institución educativa. Me he puesto en contacto con Continuum Analytics y han incluido el dominio @konradlorenz.edu.co

A vuelta de correo le enviarán un archivo que debe ubicar en el directorio de la instalación ~/.continuum válido por un año. 

Descargue el instalador desde el siguiente enlace (Verifique que descarga el instalador adecuado):

64 versus 32 bit
Para muchas instalaciones binarias debe decidir correctamente: ¿32-bit o 64-bit? Realmente el problema está
si su computador es de 32 bit, puesto que debe instalar el de 32 bit obligatoriamente. Sin embargo, el 
recíproco no es válido, puede instalar 32 bit o 64 bit en un máquina de 64 bit. Si su computador es 64 bit, recomiendo 
descargas la de 64 bit. 

----------------------------------------------------------------
Para saber qué arquitectura de software tiene haga lo siguiente:

# MacOSX: 

Vaya a la manzana de la esquina superior izquierda y escoja la opción "Acerca de este Mac"
y luego "Más información", busque el nombre del Procesador:

Nombre del Procesador 		32- or 64-bit
Intel Core Solo				32 bit
Intel Core Duo				32 bit
Intel Core 2 Duo			64 bit
Intel Quad-Core Xeon		64 bit
Dual-Core Intel Xeon		64 bit
Quad-Core Intel Xeon		64 bit	
Core i3						64 bit
Core i5						64 bit
Core i7						64 bit	

Fuente:
http://support.apple.com/kb/HT3696?viewlocale=en_US&locale=en_US


# Linux: 

En una terminal digite uname -mpi Si usted ve x86_64 x86_64 x86_64 su computador es de 64-bit. 

Si ve uno o más i686 o i386 está utilizando una máquina de 32-bit
______________________________________________

Ahora sí descargue Anaconda

http://continuum.io/downloads.html


Una vez descargado, utilice la terminal para ir al directorio de la descarga y, asumiendo que tiene el mismo nombre el archivo descargado digite
en la línea de comando (una terminal):

Nota: El instalador le preguntará dónde desea instalar el software. Por defecto está predeterminado el directorio home. Sin embargo, recomiendo crear una carpeta para este fin. Cualquier forma funciona bien. 

#Mac:
El archivo descargado es un ejecutable. Siga las instrucciones. 

#Linux:
Desde la terminal digite:

% bash Anaconda-2.0.0-Linux-x86_64.sh

- Presione ENTER para continuar
- Si desea lea las instrucciones. Presionando la tecla q, llega al final del documento. Digite "yes" y presione ENTER. 
- ENTER para confirmar la ubicación.
- La instalación puede tardar varios minutos. 
- Digite "yes" para agregar la instalación al PATH
- Si todo sale bien debe aparecer: "Thank you for installing Anaconda!"

Abra una nueva terminal y digite: python
Si todo ha salido bien, deberá aparecer

# Mac:
Python 2.7.6 |Anaconda 2.0.0 (x86_64)| (default, May 27 2014, 14:58:54) 
[GCC 4.0.1 (Apple Inc. build 5493)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
Anaconda is brought to you by Continuum Analytics.
Please check out: http://continuum.io and https://binstar.org

#Linux:
Python 2.7.6 |Anaconda 2.0.0 (64 -bit)| (default, May 27 2014, 14:58:54) 
[GCC 4.1.2 20080704 (Red Hat 4.1.2 -54)] on linux2
Type "help", "copyright", "credits" or "license" for more information.
Anaconda is brought to you by Continuum Analytics.
Please check out: http://continuum.io and https://binstar.org

Presione Ctrl d para salir. 

Una descripción alternativa que resulta útil para la instalación está en:

<http://python4astronomers.github.io/installation/python_install.html>

______________________

- Paquetes adicionales de Python. Para instalarlos abra una nueva terminal y digite:

pip install <nombre del paquete>

para actualizar un paquete digite:

pip install --upgrade <nombre del paquete>

Paquetes adicionales:

emcee
sqlalchemy
scikit-image
scikit-learn
______________________

- Git. 

Primero, cree una cuenta en GitHub si no tiene una <http://github.com>

Segundo, instale GitHub en su computador. Las instrucciones están en el documento GitHub.pdf
______________________

- R

Utilice el instalador de : <http://cran.r-project.org/mirrors.html> 
Recomiendo el Servidor de la Universidad Nacional: <http://www.laqee.unal.edu.co/CRAN/>

- Paquetes adicionales para R.

FITSio, MASS, scatterplot3d, Hmisc, MASS, scatterplot3d

Linux: Para instarlos abra R y utilice la consola de R para ejecutar el siguiente comando para cada paquete:
Por ejemplo, para instalar Hmisc:

install.packages(repos="http://cran.r-project.org", "Hmisc")

Mac: Para instalar paquetes adicionales de R abra la aplicación y selecciones el menu "Packages & Data/Package Installer" menu.
Con "CRAN (binaries)" seleccionado (por defecto) haga click en "Get List". Use el campo de búsqueda para encontrar los paquetes anteriores y haga click en el boton "instalar".

______________________
- Software específico para Mac.

- Xcode. Es gratis y se obtiene directamente desde el App Store. Siga las siguientes instrucciones para realizar 
la instalación correctamente. http://www.scicoder.org/2012/03/developer-tools-on-os-x-10-7-lion/

- TextWranger, http://www.barebones.com/products/textwrangler/

- iTerm: <http://iterm.sourceforge.net/downloads.shtml>

- TeXShop: <http://pages.uoregon.edu/koch/texshop/obtaining.html>

- XQuartz (descargue la última versión): <http://xquartz.macosforge.org/landing/>

* Software específico para Linux.

- Kate: <http://kate-editor.org/get-it/> (Se puede obtener desde ek Centro de Software de Ubuntu)

______________________

OPCIONAL:

Intalar el procesador de textos LyX desde (<http://www.lyx.org>). Es muy útil y su uso está creciendo en la comunidad
científica. 

Curioso:
import this
______________________


Esta información puede distribuirse libremente