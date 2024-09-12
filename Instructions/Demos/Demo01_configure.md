---
demo:
  title: "Demostración\_01: Configuración de una máquina virtual Linux de Azure."
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Demostración 01: Configuración de una máquina virtual Linux de Azure.

## Tareas de credenciales

Usa la demostración para revisar estas tareas de credenciales:
+ Creación de una máquina virtual Linux (portal).
+ Configuración de una VM Linux.
+ Conexión a una VM LInux con SSH.  
+ Actualización de sistemas operativos de VM Linux.
+ Instalación y ejecución de una dependencia de carga de trabajo.

## Requisitos de recursos

Este recurso se puede crear antes o durante la demostración. 

+ Grupo de recursos. 

## Diapositivas de referencia (opcional)

+ Plan para las máquinas virtuales
+ Distribuciones de Linux compatibles
+ Tamaño de la máquina virtual
+ Organización de recursos de Azure
+ Herramientas de administrador de Azure

## Pasos de referencia

En estos vínculos se proporcionan pasos detallados.

+ [Aprovisionamiento de una máquina virtual Linux mediante Azure Portal](https://learn.microsoft.com/training/modules/provision-linux-virtual-machine-in-azure/2-provision-linux-virtual-machine-using-the-azure-portal)
+ [Inicio rápido: Creación de una máquina virtual Linux](https://learn.microsoft.com/azure/virtual-machines/linux/quick-create-portal?tabs=ubuntu)

## Puntos de discusión

**Creación y configuración de la máquina virtual**

1. Uso del portal para crear una VM Linux. Analiza cómo, en ejercicios posteriores, se usarán las plantillas de la CLI e inicio rápido para crear VM. 

1. Usa el vínculo del portal para revisar la selección de **imágenes** de Linux.  Identifica la distribución más reciente de Ubuntu.

1. Usa el vínculo del portal para revisar las selecciones de **tamaño**.  Analiza cómo puedes modificar la escala de la configuración de CPU y memoria.

1. Analiza los efectos del cambio de tamaño. El cambio de tamaño se realizará en un laboratorio posterior. 

1. Analiza las distintas formas de conectarse a una máquina virtual Linux (clave pública SSH y contraseña).
   
1. Analiza la importancia de las **reglas de puerto de entrada**. En concreto, el puerto 22 para SSH y el puerto 80 para NGINX. 

1. Usa la pestaña **Discos** para mostrar cómo se agregaría un disco de datos. La adición de un disco de datos se realizará en un ejercicio posterior. 
 
1. Usa la página **Avanzado** para mostrar dónde se puede proporcionar un archivo cloud-init.

1. Asimismo, los ejercicios posteriores usan plantillas y la CLI para instalar máquinas virtuales. 

**Acceso a la máquina virtual e instalación de NGINX**

1. Implementa la máquina virtual. Analiza la fase de validación y cómo supervisar las notificaciones.

1. Abre una ventana de CMD y accede a la máquina virtual con SSH. Analiza el formato del comando SSH y la ubicación del archivo de clave. 

1. Instala NGINX y asegúrate de que se muestra la página principal. 
