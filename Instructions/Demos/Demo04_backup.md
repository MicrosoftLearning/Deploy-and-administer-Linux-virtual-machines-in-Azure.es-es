---
demo:
  title: "Demostración\_04: Copia de seguridad de máquinas virtuales Linux de Azure"
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Demostración 04: Copia de seguridad de máquinas virtuales Linux de Azure

## Tarea de credenciales

+ Configurar Azure Backup 

## Requisitos de recursos

+ Máquina virtual Linux

## Pasos de referencia

En este vínculo se proporcionan pasos detallados.

+ [Inicio rápido: Copia de seguridad de máquinas virtuales en el portal](https://learn.microsoft.com/azure/backup/quick-backup-vm-portal)
+ [Inicio rápido: Creación e implementación de plantillas de ARM mediante Azure Portal](https://learn.microsoft.com/azure/azure-resource-manager/templates/quickstart-create-templates-use-the-portal)

## Diapositivas de referencia

Usa estas diapositivas para proporcionar más contexto.  

+ ¿Qué es Azure Backup?
+ Opciones de protección de máquinas virtuales

## Puntos de discusión

1. Revisa la importación de una plantilla. Esta es la cuarta forma en que han creado una VM en la clase.
   
1. Analiza la necesidad de un almacén de Recovery Services. El almacén debe estar en la misma región que el origen de datos. 

1. Revisa cómo se puede acceder y habilitar la copia de seguridad de máquinas virtuales en el portal. 

1. Analiza la diferencia entre las directivas de copia de seguridad estándar y mejorada. 

1. Usa la lista desplegable **Tipo de origen de datos** para revisar los recursos que el Centro de copia de seguridad puede proteger.

1. Destaca la directiva de copia de seguridad predeterminada y el hecho de que se pueda crear una personalizada.

1. Analiza cómo se puede usar una sola directiva de copia de seguridad en muchas máquinas virtuales diferentes.

1. Revisa la configuración de la directiva de copia de seguridad (programación y retención).

1. Revisa cómo supervisar trabajos de copia de seguridad.

1. Revisa cómo puedes restaurar máquinas virtuales (no en la credencial). 
