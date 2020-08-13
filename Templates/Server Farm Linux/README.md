# Server Farm

## Informacion
Para desplegar el servicio de Server Farm o Service Plan  se ha utilizado la plantilla [ServerFarmLinux.json](ServerFarmLinux.json) y han sido necesarios los parámetros definidos en [ServerFarmLinux.parameters.json](ServerFarmLinux.parameters.json).


## Despliegue
Un flujo ejemplo de despliegue en VSTS sería el siguiente:


### Release-Pipeline
>Se enlaza el artefacto generado con los ficheros ServerFarmLinux.json & ServerFarmLinux.parameters.json
>![Imagen de Pipeline](Images/Release-Pipeline.png)

### Release-Task
>Se añade una tarea de despliegue de grupo de recursos y se selecciona los ficheros del artefacto.
>![Imagen de Task](Images/Release-Task.png)

### Release-Variables
>Se sustituyen los parámetros definidos en ServerFarmLinux.parameters.json para adaptar el despliegue a nuestro entorno.
>![Imagen de Variables](Images/Release-Variables.png)