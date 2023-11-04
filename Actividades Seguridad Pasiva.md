# Actividades Seguridad Pasiva

## Actividad 1.- Búsqueda de Información
Búsqueda de información con el fin de elaborar un diccionario de herramientas mencionadas en este tema, y de aquellos que resulten de la búsqueda de información, en el que se describen los siguientes elementos: descripción, http de descarga y http de tutorial/manual de uso, http de ejemplo de aplicación/uso, otros aspectos.

<br>

### RAID (Redundant Array of Independent Disks)
Consiste en un conjunto de técnicas hardware o software que utilizando varios discos proporcionan principalmente tolerancia a fallos, mayor capacidad y mayor fiabilidad en el almacenamiento. Se trata de un sistema de almacenamiento que utilizando varios discos y distribuyendo o replicando la información entre ellos

Son técnicas que ya van implementadas en los sistemas operativos, solo hace falta llevarlo a cabo

Manual de uso para Linux: https://docs.aws.amazon.com/es_es/AWSEC2/latest/UserGuide/raid-config.html

Manual de uso para Windows: https://docs.aws.amazon.com/es_es/AWSEC2/latest/WindowsGuide/raid-config.html

<br>

### Backup4all
Nos permite proteger los datos de las posibles pérdidas parciales o totales, automatiza el proceso de realización de copias de seguridad y permite, entre otras funciones, comprimir y cifrar las copias de seguridad.

Descarga: https://www.backup4all.com/download.html

Manual/Tutorial: https://download.backup4all.com/download/pdf/Backup4all-User-Manual.pdf

<br>

### Cobian Backup
Cobian Backup es un programa gratuito, multitarea, capaz de realizar copias de seguridad en un equipo, unidad extraíble, red local o incluso en/desde un servidor FTP. Soporta conexiones seguras mediante SSL. Se ejecuta sobre windows y uno de sus grandes fuertes es que consume muy pocos recursos y puede estar funcionando en segundo plano.

Descarga: https://www.cobiansoft.com/cobianbackup.html

Manual/Tutorial: https://youtu.be/LELZdOcpkU4

<br>

### Amanda
Orientada a crear copias de seguridad en múltiples terminales bajo la dirección del administrador de la red. El proceso se lleva a cabo gracias a un servidor que engloba a los terminales seleccionados y realiza un backup rápido y cómodo, ya que evita andar clonando disco por disco.

Descarga: https://www.amanda.org/download.php

Documentación para usuarios: https://wiki.zmanda.com/index.php/User_documentation

Documentación para desarrolladores: https://wiki.zmanda.com/index.php/Developer_documentation

<br>

### Burt
Burt es un sistema de copias de seguridad de redes creado en la universidad de Wisconsin. Está diseñado para hacer copias de seguridad de grandes redes heterogéneas. Usa el lenguaje de encriptado TCL y herramientas de copia de seguridad estándar como dump y GNUTar para permitir copias de seguridad de una amplia variedad de orígenes de datos, incluyendo estaciones de trabajo UNIX y Windows NT, almacenamientos basados en AFS y otros. 

Descarga: https://pages.cs.wisc.edu/~jmelski/burt/download.html

Pasos de instalación: https://pages.cs.wisc.edu/~jmelski/burt/install.html

Manual/Tutorial: https://pages.cs.wisc.edu/~jmelski/burt/docs.html

<br>

### BRU
BRU Server es una herramienta de copias de seguridad en red diseñada por TOLIS Group que proporciona la posibilidad de hacer y restaurar copias de seguridad de clientes y servidores en redes de cualquier tamaño. Soporta todos los principales sistemas operativos cliente así como sistemas operativos servidor.

Descarga: https://www.tolisgroup.com/demos62051.html

Manual/Tutorial: https://www.tolisgroup.com/assets/argest_backup_user_guide.pdf

<br>

### Arkeia
Arkeia Software es un software de copia de seguridad y almacenamiento en red network para Windows, Macintosh, Linux, AIX, BSD y HP-UX 

Descarga: https://support.wdc.com/arkeia/software.aspx

Manual/Tutorial: https://docplayer.net/11888179-Arkeia-network-backup-user-manual.html

<br>

### Mondo
Mondo Rescue es un software de recuperación en caso de desastre. Soporta Linux (i386, x86-64, IA-64) y FreeBSD (i386). Está empaquetado para múltiples distribuciones (Red Hat, RHEL, Fedora, CentOS, OpenSuSE, SLES, Mandriva, Debian, Ubuntu, Gentoo). También soporta cintas, discos, dispositivos USB, redes y CD/DVD como medios para copia de seguridad, múltiples sistemas de ficheros, LVM, software y RAID por software y hardware.

Descarga: http://www.mondorescue.org/downloads.shtml

Manual/Tutorial: http://www.mondorescue.org/docs/mondorescue-howto.pdf

<br>

### dump
La herramienta se encarga de examinar los archivos y sistemas de ficheros ext2 y ext3 y determina qué archivos deben copiarse. Estos se pueden almacenar en el propio disco del sistema o bien en otro medio externo, ya sea un recurso compartido en red o bien una unidad de cinta. Un volcado que es más grande que el medio de salida, se divide en varios volúmenes. Se puede indicar el tamaño de cada volumen también de manera manual mediante parámetros.

Herramienta básica que ya trae instalado el sistema operativo

Manual/Tutorial: https://help.highbond.com/helpdocs/analytics/13/scripting-guide/es/Content/lang_ref/commands/r_dump.htm

<br>

### restore
Recupera un archivo de copia de seguridad y lo restaura en una CIU o en un appliance virtual o físico independiente.

Herramienta básica que ya trae instalado el sistema operativo

Manual/Tutorial: https://techdocs.broadcom.com/es/es/symantec-security-software/endpoint-security-and-management/endpoint-detection-and-response/4-8/using-the-command-line-interface-v109281349-d38e71236/restore-command-v117597616-d38e72430.html

<br>

### tar
Tar es una herramienta básica de Linux más usada para comprimir archivos. Tar significa Tape Archive (archivo de cinta) y se utiliza para comprimir una colección de archivos y carpetas.

Herramienta básica que ya trae instalado el sistema operativo

Manual/Tutorial: https://www.hostinger.es/tutoriales/como-usar-comando-tar-linux

<br>

### cpio
Es una utilidad que permite copiar archivos a o desde un contenedor cpio, que no es más que un fichero que almacena otros archivos e información sobre ellos (permisos, nombres, propietario...). Este contenedor puede ser un disco, otro archivo, una cinta o incluso una tubería, mientras que los ficheros a copiar pueden ser archivos normales, pero también dispositivos o sistemas de ficheros completos.

Herramienta básica que ya trae instalado el sistema operativo

Manual/Tutorial: https://www.ibiblio.org/pub/linux/docs/LuCaS/Manuales-LuCAS/doc-unixsec/unixsec-html/node106.html

<br>

### dd
El comando dd (Dataset Definition), es una herramienta sencilla, útil, y sorprendentemente fácil de usar; con esta herramienta se puede hacer lo mismo, sobre dispositivos: discos y particiones, que con programas comerciales con solo una pequeña línea de comandos.

Herramienta básica que ya trae instalado el sistema operativo

Manual/Tutorial: https://blog.desdelinux.net/uso-del-comando-dd/

<br>

### rsync
rsync es la herramienta de copiado y sincronización de archivos más potente que existe en el mundo de Linux/Unix. Es una utilería, que de acuerdo a su página, es rápida, versátil para el copiado local y remoto de archivos. Ofrece una larga lista de opciones que controlan todos los posibles aspectos de su comportamiento.

Herramienta básica que ya trae instalado el sistema operativo

Manual/Tutorial: https://www.linuxtotal.com.mx/index.php?cont=rsync-manual-de-uso

<br>

### duplicity
Descripción:Duplicity es un programa de copias de seguridad en red. Puede guardar instantáneas de directorios y archivos en un archivo tar remoto encriptado con GnuPG, que actúa como repositorio de copias de seguridad. La conexión con el repositorio remoto puede realizarse a través de cualquiera de los siguientes protocolos: rsync, ftp, HSI, WebDAV, Tahoe-LAFS, o Amazon S3.

Descarga: apt-get install duplicity

Manual/Tutorial: https://duplicity.nongnu.org/vers7/duplicity.1.html

<br>

### cron
Cron es un administrador de tareas de Linux que permite ejecutar comandos en un momento determinado, por ejemplo, cada minuto, día, semana o mes. Si queremos trabajar con cron, podemos hacerlo a través del comando crontab.
Herramienta básica que ya trae instalado el sistema operativo

Manual/Tutorial: https://www.linuxtotal.com.mx/index.php?cont=info_admon_006

<br>

### Recuva
Recuva es un programa que te permite recuperar información desde tu PC o dispositivos de almacenamiento externos como tarjetas SD o discos duros en caso de que hayas perdido tus archivos al eliminarlos por error, al recibir un ataque de un virus o al dañarse tu información.

Descarga: https://www.ccleaner.com/es-es/recuva/download

Manual/Tutorial: https://4ddig.tenorshare.com/es/computer-data-recovery/how-to-use-recuva.html

<br>

### TestDisk
TestDisk es un software gratuito de recuperación de datos. Fue principalmente diseñado para ayudar a recuperar particiones perdidas y/o volver discos no booteables a booteables nuevamente cuando estos síntomas son causados por software con fallas, ciertos tipos de virus o error humano.

Descarga:https://www.cgsecurity.org/wiki/TestDisk_Download

Manual/Tutorial: https://www.cgsecurity.org/testdisk_doc/

<br>

### Foremost
Foremost es una herramienta forense para la recuperación de ficheros basado en sus cabeceras, footer y estructuras de datos internas. Foremost puede trabajar con imágenes, como las generadas por dd, Safeback, Encase, etc, o directamente sobre un disco.

Descarga: https://foremost.sourceforge.net/

Manual/Tutorial: https://foremost.sourceforge.net/foremost.html

<br>

### PhotoRec
PhotoRec es un software diseñado para recuperar archivos perdidos incluyendo videos, documentos y archivos de los discos duros y CDRoms así como imágenes perdidas (por eso el nombre PhotoRecovery) de las memorias de las cámaras fotográficas, MP3 players, PenDrives, etc. PhotoRec ignora el sistema de archivos y hace una búsqueda profunda de los datos.

Descarga: https://photorec.programas-gratis.net/

Manual/Tutorial: https://www.cgsecurity.org/testdisk_doc/

<br>

### Scalpel
Scalpel es un fork actualizado de foremost, aunque más rápida y más eficiente en el rastreo y búsqueda de patrones de archivos que utiliza una base de datos que almacena patrones de bytes conocidos de archivos e identifica los archivos borrados y recuperar los recupera de manera instantánea.

Descarga: https://pkgs.org/download/scalpel

Manual/Tutorial: https://www.redhat.com/sysadmin/find-lost-files-scalpel

<br>

### Symantec Ghost
Symantec Ghost Solution Suite es una solución de software galardonada que crea imágenes y se implementa en computadoras de escritorio, computadoras portátiles, tabletas y servidores.

Descarga: https://knowledge.broadcom.com/external/article/175846/download-the-latest-version-of-symantec.html

Manual/Tutorial: https://techdocs.broadcom.com/content/dam/broadcom/techdocs/symantec-security-software/endpoint-security-and-management/ghost-solutions-suite/generated-pdfs/GSS_3_3_User_Guide.pdf

<br>

### Acronis True Image
Acronis True Image es un programa que sirve para la clonación de equipos informáticos tanto del disco duro al completo (imágenes de disco) como de una o varias particiones. Además, permite crear copias de seguridad de carpetas y ficheros.

Descarga: https://kb.acronis.com/content/65523#

Manual/Tutorial: https://www.acronis.com/en-us/support/documentation/ATI2021/#35899.html

<br>

## Actividad 2.
Analiza y describe los sistemas biométricos que actualmente se están utilizando, así como los estudios de implantación de nuevas tecnologías respecto a este campo.

La biometría es el método de reconocer a las personas basado en sus características físicas, lógicas o de comportamiento. En la actualidad, la tecnología ha permitido perfeccionar los procesos de reconocimiento biométricos, de forma que tienen uso en multitud de aplicaciones y finalidades.

Hoy en día las tecnologías de biometría más usadas son la huella dactilar y el reconocimiento facial debido a que en los dispositivos móviles son las más comunes.

- Huella dactilar: 
Es la más antigua y sigue en uso debido a su alta tasa de precisión y su facilidad de uso. Funciona de dos formas:

  - Basadas en minucias: 
Esta técnica se basa en identificar las partes más fácilmente detectables existentes en la huella dactilar. Se guarda la forma y la posición dentro de la huella y tras una serie de cálculos permite el acceso. Sin embargo existen algunas dificultades asociadas a este método, porque si la calidad no es muy buena, es difícil extraerlas de forma precisa.

  - Basadas en correlación: 
Mediante este método se analiza el patrón entero y se genera un esquema. Esta técnica requiere un registro preciso. pero su principal problema es que se ve afectada por la rotación de la imagen

- Reconocimiento facial: 
El reconocimiento facial es la técnica por la cual se reconoce a una persona a partir de una imagen de la cara. Entre los aspectos claves se encuentra la simetría facial, la longitud de la nariz o el ángulo de la mandíbula. A diferencia de otros sistemas biométricos este sistema se puede usar para la vigilancia en general, habitualmente es usado en cámaras de vídeo.


- Reconocimiento de iris: 
Esta técnica está aún en desarrollo y que poco a poco está tomando más importancia además es más difícil de vulnerar debido a que tiene más de 200 propiedades únicas. El escaneado del iris se lleva a cabo con una máquina infrarrojos especializada y muy cerca de la persona, ilumina el ojo y le hace una fotografía de alta resolución

## Actividad 3
Analiza el asistente/herramienta de copias de seguridad con el programador de tareas, restauración de las copias de seguridad, puntos de restauración, disco de reparación y reinicio del sistema en reparación/restauración en un entorno Windows 10 o windows server. Realiza el ejemplo pertinente que demuestre la utilización de herramienta.

Las copias de seguridad en un Windows Server 19 son una característica, no un rol, que hay que implementar al servidor porque de base no están implementadas.

!
























