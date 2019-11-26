<a name="top"></a>

# Robot_Nivel_3_UiPath

En este proyecto se hará un UiPath con plantilla **Robotic Enterprise Framework**.

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
    - name: ~~UiPath_REFrameWork_UiDemo~~.
    - description: ~~Demostrating the REFramework with UiDemo~~.
- Dentro del directorio Data:
    - Creada una Sequence llamada Dispatcher.xaml.
    - <span style="color: red">En la propiedad SheetName de la actividad ReadRange hay que tener cuidado con el idioma con el que tengamos excel</span>.
