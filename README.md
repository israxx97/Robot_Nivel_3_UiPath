<a name="top"></a>

# Robot_Nivel_3_UiPath

En este proyecto se hará un UiPath con plantilla **Robotic Enterprise Framework**.

Esta documentación debe leerse a medida que se lee el PDF del correspondiente proyecto, ya que este documento muestra solo puntos importantes que no se muestran o se muestran confusos en el PDF de UiPath.

1. [Versión 1.0](#1dot0version)
2. [Versión 1.1](#1dot1version)

[Subir](#top)

<a name="1dot0version"></a>

### Versión 1.0

En esta versión encontraremos los archivos generados al crear un nuevo proyecto en UiPath Studio con la plantilla **Robotic Enterprise Framework**.

[Subir](#top)

<a name="1dot1version"></a>

### Versión 1.1

En esta versión se han realizado varios cambios:

- Se cambiaron 2 campos del archivo project.json:
    - name: *UiPath_REFrameWork_UiDemo*.
    - description: *Demostrating the REFramework with UiDemo*.
- Dentro del directorio Data: [info1](#info1)
    - Creada una Sequence llamada Dispatcher.xaml.

<a name="info1"></a>

##### Info 1

En la versión 2019.11 la Activity **Read Range** debe ir dentro de la Activity **Excel Application Scope**.

En la propiedad **SheetName** de la actividad **ReadRange** hay que tener cuidado con el idioma con el que tengamos excel.

En la propiedad **ItemInformation** de la activity **Add Queue Item**, en el campo Value introduciremos el nombre que le pusimos al item del bucle **for each**, pasándole a este como parámetro el nombre de la columna en Excel y pasándolo a String con el método **ToString**.

Completar la propiedad **QueueName** de la activity **Add Queue Item** para eliminar el error, deberemos agregarle argumento que crearemos de **entrada** de tipo **Dictionary<String, Object>** llamado **in_config**, pasándole a este como parámetro el **name** de la key que aparecerá en el archivo **Config.xlsx** como **OrchestratorQueueName** y pásandolo a String con el método **ToString**.