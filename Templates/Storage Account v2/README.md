# Storage Account v2

## Informacion
Para desplegar el servicio de Azure Storage Account v2 se ha utilizado la plantilla [storageaccount.json](storageaccount.json) y han sido necesarios los parámetros definidos en [storageaccount.parameters.json](storageaccount.parameters.json).


## Despliegue
Un flujo ejemplo de despliegue en VSTS sería el siguiente:


### Release-Pipeline
>Se enlaza el artefacto generado con los ficheros storageaccount.json & storageaccount.parameters.json
>![Imagen de Pipeline](Images/Release-Pipeline.png)

### Release-Task
>Se añade una tarea de despliegue de grupo de recursos y se selecciona los ficheros del artefacto.
>![Imagen de Task](Images/Release-Task.png)

### Release-Variables
>Se sustituyen los parámetros definidos en storageaccount.parameters.json para adaptar el despliegue a nuestro entorno.
>![Imagen de Variables](Images/Release-Variables.png)
