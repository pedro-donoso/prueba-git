*NOTA: Hago esta prueba de forma explicativa inicialmente, debido a que mi laptop es de 4 gb y colapsó en varias ocasiones al momento de correr la app, el próximo mes me traerán un equipo con las condiciones adecuadas 32gb 12gen para rehacer la prueba, hago esto para cumplir y subir algo a la plataforma dentro del plazo, luego la realizaré en Android Studio cuando tenga las condiciones.*

#### 1. Crear o utilizar algún proyecto existente con Android Studio, para luego crear repositorio en GitHub. 

#### Crear un nuevo proyecto en Android Studio:
  - Abre Android Studio y selecciona "Nuevo proyecto".
  - Elige "Aplicación vacía" como tipo de proyecto y haz clic en "Siguiente".
  - Configura el nombre, la ubicación y el paquete del proyecto.
  - Haz clic en "Finalizar".

#### Inicializar Git en el proyecto:
- Ve a VCS > Git > Inicializar repositorio local.
- Si te lo pide, configura el nombre y el correo electrónico del autor.
- Agrega un archivo README inicial con una breve descripción del proyecto.
- Haz clic en "Commit" y luego en "Push" para subir los cambios a GitHub.

#### Crear un repositorio en GitHub:
- Haz clic en el icono "+" en la esquina superior derecha y selecciona "Nuevo repositorio".
- Escribe un nombre para tu repositorio y haz clic en "Crear repositorio".

#### Conectar el proyecto de Android Studio con el repositorio de GitHub:
- En Android Studio, ve a VCS > Git > Remoto > Agregar remoto.
- Introduce la URL del repositorio de GitHub que has creado.
- Dale un nombre al control remoto.
Haz clic en "Aceptar".

#### Subir el proyecto a GitHub:
- En Android Studio, ve a VCS > Git > Push.
- Selecciona el control remoto que has creado.
- Selecciona la rama a la que quieres subir los cambios.
- Escribe un Commit y haz clic en "Push".

#### 2. Inicializar el sistema de control de versiones con Git, para después agregar y confirmar los cambios. 

#### Inicializar Git
- Abre tu terminal o símbolo del sistema.
- Navega hasta el directorio del proyecto que deseas versionar.
- Ejecuta el siguiente comando:
  
```
git init
```

*Esto creará un nuevo repositorio Git en tu directorio y configurará los archivos necesarios para el control de versiones.*


#### Agregar archivos al seguimiento de Git
- Utiliza el comando git add para agregar los archivos que deseas versionar al repositorio.

```
git add .
```

#### Confirmar los cambios
- Utiliza el comando git commit para confirmar los cambios agregados.

```
git commit -m "agrego navbar"
```

#### Recomendaciones:

*Cada commit debe tener un mensaje descriptivo que explique los cambios realizados.*

*Puedes usar el comando git status para ver qué archivos se han modificado y cuáles no están siendo rastreados por Git.*

*Puedes usar el comando git log para ver el historial de commits de tu repositorio.*


#### 3. Configurar el remoto y empujar los cambios si IDE ya tiene la configuración de GitHub, en caso contrario, agregar el token necesario. 

#### Abre tu proyecto en Android Studio.
- Ve a VCS > Git > Remoto > Agregar remoto.
- Introduce la URL del repositorio de GitHub que has creado.

#### Dale un nombre al control remoto
- Haz clic en "Aceptar".
- Para subir los cambios a GitHub, ve a VCS > Git > Push.
- Selecciona el control remoto que has creado.
- Selecciona la rama a la que quieres subir los cambios.
- Escribe un Commit y Push.

#### 4. Crear la rama feature1, para luego hacer un cambio en un archivo de la rama feature1, guardar los cambios (commit), y empujar la rama feature1 al remoto. 

#### Crear rama feature1:
- Abre tu proyecto en Android Studio.
- Asegúrate de que estés en la rama correcta .
- Ve a VCS > Git > Branch > New Branch.
- Escribe el nombre de la nueva rama ("feature1") y haz clic en "Aceptar".

#### Realizar un cambio en un archivo:
- Abre el archivo en el que deseas realizar el cambio.
- Haz los cambios deseados.
- Guarda el archivo.

#### Confirmar los cambios (commit):
- Ve a VCS > Git > Cambios sin confirmar.
- Selecciona los archivos que deseas agregar al commit.
- Escribe un mensaje descriptivo y Commit.

#### Subir la rama feature1 al remoto:
- Ve a VCS > Git > Remoto > Push.
- Selecciona la rama "feature1" para subir.
- Introduce el nombre del control remoto.
- Escribe un mensaje de confirmación (opcional) y haz clic en Push.

#### Ventajas:
- Al crear una nueva rama, se crea una nueva línea de desarrollo independiente de la rama principal. Esto te permite trabajar en un cambio sin afectar el código de la rama principal.

- Al realizar un cambio en un archivo y confirmarlo, se crea un snapshot del estado actual del proyecto. Esto te permite volver a este estado si es necesario.

- Al subir la rama al remoto, se hace que los cambios estén disponibles para otros colaboradores que puedan trabajar en el mismo proyecto.

#### 5. Crear PR para mezclar los cambios de feature1 a master (desde Android Studio o desde consola). 

#### Desde Android Studio:
- Abre tu proyecto en Android Studio.
- Ve a VCS > Git > Remoto > Ver en GitHub.
- Se abrirá tu repositorio en GitHub en un navegador web.
- Haz clic en la pestaña "Pull requests".
- Haz clic en el botón "New pull request".
- Selecciona la rama "feature1" como rama base.
- Selecciona la rama "main" como rama de destino.
- Escribe un título y una descripción para tu PR.
- Haz clic en "Create pull request".

#### Ventajas:
- Una PR (Pull Request) es una solicitud para que los cambios de una rama se fusionen en otra rama. Esto permite a los colaboradores revisar los cambios y proporcionar comentarios antes de que se fusionen en la rama principal.
- Al crear una PR, se comparan los cambios de la rama "feature1" con la rama principal. GitHub mostrará una vista de las diferencias entre las dos ramas. Los colaboradores pueden revisar estas diferencias, agregar comentarios y aprobar o rechazar la PR.
- Si se aprueba la PR, los cambios de la rama "feature1" se fusionarán en la rama principal.
