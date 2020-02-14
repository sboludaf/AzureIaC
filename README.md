# Infraestructura como Código en Azure

## Proyecto que contiene script y plantillas ARM para desplegar recursos en Azure.
>Este proyecto trata sobre el uso de infraestructura programable, también llamada Infraestructura como Código (IaC). Esta práctica trata la configuración de la infraestructura como un software de programación. De este modo, se puede desplegar elementos de infraestructura de forma automática, sin necesidad de desplegar recursos de forma iterativa. 
>
>Este tipo de implementación ha ayudado a la cultura DevOps ya que difumina aún más las líneas que separan desarrollo de operaciones. De esta forma se converge el código que ejecutan las aplicaciones y el código generado por la infraestructura para generar un código capaz de ofrecer una integración continua.
>
>La documentación generada en este repositorio, está desarrollada única y exclusivamente para desplegar recursos en Azure, se trata de una documentación de libre acceso.

---
---

## Indice
1.	Requisitos para los despliegues
2.	Plantillas ARM
3.	Scripts
4.  Despliegue
5.	Licencia y Contacto



## Requisitos para los despliegues
 **[Visual Studio Code:](https://code.visualstudio.com/)** Se trata de un editor de texto de código fuente desarrollado por Microsoft para Windows, Linux y macOS. Que a su vez se han instalado una serie de extensiones para facilitar el desarrollo de las plantillas ARM.
 
 - [Azure Tools:](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-node-azure-pack) Instala todas las herramientas necesarias para conectar VS Code con la plataforma de Azure, además, incluye una herramienta que nos ayudará a auto-completar las plantillas ARM.

 - [Azure ARM Template Helper](https://marketplace.visualstudio.com/items?itemName=ed-elliott.azure-arm-template-helper) Ayuda a identificar los recursos desplegados en la plantilla ARM que serán mostrados de forma gráfica.

 **[Azure CLI](https://docs.microsoft.com/es-es/cli/azure/?view=azure-cli-latest)** Se trata de la interfaz de la linea de comandos (CLI) de Azure 

 **[Suscripción de Azure:](https://portal.azure.com/)** Donde se desplegarán los recursos.



## Plantillas ARM
Una [plantilla ARM](https://docs.microsoft.com/es-es/azure/azure-resource-manager/templates/overview) es un fichero JSON que contiene la infraestructura y la configuración del proyecto. Las plantillas tienen las siguientes ventajas:
 - **Sintaxis declarativa:** Las plantillas ARM permiten crear una infraestructura de Azure completa de forma declarativa.


 - **Resultados repetibles:** La infraestructura de implementa de manera coherente y de forma idempotente, lo que significa que la plantilla se puede implementar múltiples veces y obtener los mismos recursos en el mismo estado.

 - **Orquestación:** Resource Manager se encarga de gestionar la implementación de recursos interdependientes para que se creen en el orden correcto.

- **Integración de CI/CD:** El objetivo de las plantillas ARM es que la infraestructura perteneza al flujo de integración y entrega continua.



## Scripts
Los scripts están desarrollados para ser desplegados mediante la interfaz de líneas de comandos de Azure.

Estos scripts se utilizan para desplegar recursos que no están contemplados con las plantillas ARM, en su mayoría recursos de Azure Active Directory.



## Despliegue
Al igual que todo flujo de CI/CD se establecerá una construciccón del artefacto y se desplegará en el grupo de recursos correspondiente.



# Licencia y Contacto
Todo el código desarrollado en el repositorio es de libre acceso y uso, para más información puede contactar a través de los siguientes métodos.

-GMAIL

LINKEDIN