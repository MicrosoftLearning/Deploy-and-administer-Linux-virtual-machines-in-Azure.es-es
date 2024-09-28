---
demo:
  title: 'Demostración 03: Acceso al almacenamiento para una máquina virtual Linux de Azure'
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Demostración 03: Acceso al almacenamiento para una máquina virtual Linux de Azure

## Tareas de credenciales

+ Creación de una máquina virtual (CLI).
+ Agrega discos de datos de la máquina virtual y configura particiones. 
+ Montaje de un recurso compartido de archivos de Azure de SMB en una VM Linux.
+ Asignación de una identidad administrada en una VM Linux. 
+ Asigne roles de Azure. 
+ Transferencia de datos desde y hacia una VM Linux mediante AzCopy. 

## Requisitos de recursos

Estos recursos se pueden crear antes o durante la demostración. 
+ Resource group
+ Máquina virtual Linux
+ Cuentas de almacenamiento con recurso compartido de archivos y contenedor de blobs.
+ Archivos cargados que se van a usar para realizar pruebas.
+ Identidad administrada. 

## Pasos de referencia

En estos vínculos se proporcionan pasos detallados.

+ [Inicio rápido: Creación de una máquina virtual Linux con la CLI de Azure en Azure](https://learn.microsoft.com/en-us/azure/virtual-machines/linux/quick-create-cli)
+ [Conexión de un disco de datos a una VM Linux](https://learn.microsoft.com/azure/virtual-machines/linux/attach-disk-portal)
+ [Creación de un recurso compartido de archivos SMB](https://learn.microsoft.com/azure/storage/files/storage-how-to-create-file-share?tabs=azure-portal)
+ [Introducción a AzCopy](https://learn.microsoft.com/azure/storage/common/storage-use-azcopy-v10)


## Diapositivas de referencia

Usa estas diapositivas para proporcionar más contexto. 
+ Cuentas de almacenamiento
+ Archivos y contenedores blob
+ Archivos frente a blobs
+ Identidades administradas
+ Control de acceso basado en rol

## Puntos de discusión

**Creación de una máquina virtual mediante la CLI**: referencia n.º 1

>Puedes usar una VM existente, en lugar de crear otra.

1. Acceder a Cloud Shell.

1. Crea la máquina virtual con la CLI. Señala que esta es la tercera forma de crear VM que se ha mostrado a los alumnos.
   
**Adición de un disco de datos a una máquina virtual Linux**: referencia n.º 2

1. Revisa cómo usar el portal para agregar un disco de datos a una máquina virtual. Los alumnos usarán la CLI en el ejercicio.

1. Conéctate a la máquina virtual y usa `lsblk` para enumerar los discos. Fíjate en el tamaño del disco y que no está montado.

1. Prepara el disco con `parted` y `partprobe`. Usa el código del vínculo de referencia.

1. Monta el disco y usa `df` para enumerar el punto de montaje. 

**Acceso a un recurso compartido de archivos SMB desde la máquina virtual**: referencia n.º 3 e instrucciones del laboratorio para estudiantes

1. Busca la cuenta de almacenamiento y analiza los recursos compartidos de archivos.

1. Asigna una identidad administrada a una máquina virtual. La identidad debería tener acceso a la cuenta de almacenamiento.

1. Copia el script del portal para acceder al recurso compartido de archivos desde una máquina virtual Linux.

1. Conéctate a la máquina virtual y crea un archivo con el script. Puedes usar el editor vi.

1. Ejecuta el script y monta el recurso compartido de archivos. 

**Uso de AzCopy para copiar un archivo de blob a la unidad de datos**: referencia n.º 4 e instrucciones del laboratorio para estudiantes.

1. Agrega el rol Colaborador de almacenamiento de datos de blob a la máquina virtual. Revisa los otros roles de blob. 

1. Conéctate a la máquina virtual e instala AzCopy. Revisa otras herramientas que se pueden usar para transferir archivos. 

1. Usa AzCopy para transferir un archivo de Blob Storage a la unidad de datos. También puedes transferir un archivo de vuelta a Blob Storage.  
