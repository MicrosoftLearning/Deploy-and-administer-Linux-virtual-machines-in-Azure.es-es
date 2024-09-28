---
demo:
  title: 'Demostración 02: Supervisión de una máquina virtual Linux de Azure'
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Demostración 02: Supervisión de una máquina virtual Linux de Azure

## Tareas de credenciales

+ Creación de una máquina virtual (plantilla de inicio rápido).
+ Configure VM Insights.
+ Crear una alerta.  
+ Identifique los problemas de rendimiento. 
+ Cambie de tamaño una máquina virtual. 

## Requisitos de recursos

+ Máquina virtual Linux (creación mediante una plantilla personalizada)

## Diapositivas de referencia 

+ Plantillas del Administrador de recursos de Azure
+ Funcionalidades clave de Azure Monitor
+ Componentes de Azure Monitor
+ Métricas y registros

  
## Pasos de referencia

En estos vínculos se proporcionan pasos detallados.

+ [Deploy a simple Ubuntu Linux VM](https://learn.microsoft.com/azure/virtual-machines/linux/quick-create-template) (Implementar una máquina virtual Ubuntu Linux sencilla)
+ [Habilitación de VM Insights para el agente de Azure Monitor](https://learn.microsoft.com/azure/azure-monitor/vm/vminsights-enable-portal#enable-vm-insights-for-azure-monitor-agent) 
+ [Tutorial: Creación de una alerta de métrica para un recurso de Azure](https://learn.microsoft.com/azure/azure-monitor/alerts/alerts-create-metric-alert-rule)


## Diapositivas de referencia (opcional)

Usa estas diapositivas para proporcionar más contexto.



## Puntos de discusión

1. Usa **Implementación de una plantilla personalizada** para una máquina Linux Ubuntu básica. Así es como los alumnos crearán la VM en el ejercicio. Analiza el uso de plantillas. 

1. Habilita VM Insights. Revisa cómo usar una regla de recopilación de datos y cómo seleccionar un área de trabajo de Log Analytics. 

1. Crea una alerta basada en métricas. Por ejemplo, crea una regla de alertas nueva en función del uso de porcentaje de CPU.

1. Analiza el uso de grupos de acciones y cómo asignar un grupo de acciones a la alerta. 

1. Revisa cómo supervisar una alerta cuando se desencadene.

1. Cierra con cómo exportar la plantilla de recursos. 
