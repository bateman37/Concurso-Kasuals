# Concurso Kasuals — Subir a GitHub Pages

Este paquete contiene TODO lo que necesitas. Son 7 archivos y no hay que tocar nada dentro de ellos.

## Archivos incluidos

- `index.html` → el juego completo (HTML, CSS, JS y las 1200 preguntas van todas dentro de este único archivo)
- `manifest.json` → hace que el juego se pueda "instalar" como app en el móvil
- `sw.js` → hace que funcione sin conexión y que las actualizaciones lleguen solas
- `icon-192.png`, `icon-512.png`, `icon-180.png`, `icon-maskable-512.png` → los iconos de la app

## Opción A — Ya tienes el repositorio de Trasnos e Gardas (o cualquier otro) y quieres subir este juego dentro

1. Entra en tu repositorio en github.com
2. Crea una carpeta nueva para este juego (por ejemplo `concurso`) usando el botón **Add file → Create new file**, escribiendo `concurso/index.html` como nombre (GitHub crea la carpeta sola al escribir la barra `/`)
3. Sube ahí dentro los 7 archivos (ver "Cómo subir los archivos" más abajo)
4. Tu juego quedará accesible en: `https://TU-USUARIO.github.io/TU-REPOSITORIO/concurso/`

## Opción B — Quieres un repositorio nuevo solo para este juego

1. Ve a **github.com** → botón verde **New** (arriba a la izquierda, o el símbolo **+** arriba a la derecha → **New repository**)
2. Ponle un nombre, por ejemplo `concurso-kasuals`
3. Márcalo como **Public** (tiene que ser público para que Pages funcione gratis)
4. Botón **Create repository**
5. Sube ahí los 7 archivos (ver siguiente sección)
6. Ve a **Settings** (pestaña arriba del repositorio) → en el menú de la izquierda, **Pages**
7. En "Branch", selecciona **main** y la carpeta **/ (root)** → **Save**
8. Espera 1-2 minutos. Tu juego quedará en: `https://TU-USUARIO.github.io/concurso-kasuals/`

## Cómo subir los archivos (igual en ambas opciones)

1. Dentro del repositorio en GitHub, botón **Add file → Upload files**
2. Arrastra los 7 archivos de este paquete a la ventana (todos a la vez, directamente, sin meterlos en una carpeta zip)
3. Abajo, en "Commit changes", puedes dejar el mensaje que sale por defecto
4. Botón verde **Commit changes**
5. Espera 1-2 minutos a que GitHub Pages lo publique

## Actualizar el juego más adelante (por ejemplo, si corrijo más preguntas)

Solo hace falta volver a subir el **`index.html`** (es el único archivo que cambia casi siempre, porque las preguntas están dentro de él). Los pasos:

1. Entra en el repositorio → abre el archivo `index.html` (o la carpeta `concurso/index.html` si usaste la Opción A)
2. Icono del lápiz (✏️) arriba a la derecha del visor de archivo, o simplemente vuelve a **Add file → Upload files** y sube el nuevo `index.html` — GitHub te preguntará si quieres sobrescribirlo, di que sí
3. Commit changes
4. Espera 1-2 minutos

Gracias al `sw.js` (service worker), si alguien ya tiene el juego instalado en el móvil, la próxima vez que lo abra con conexión a internet se actualizará solo, sin que tenga que reinstalar nada.

## Instalar el juego en el móvil (para usarlo como app)

1. Abre la URL de tu juego con Chrome (Android) o Safari (iPhone)
2. Android (Chrome): menú (⋮) → **Instalar aplicación** o **Añadir a pantalla de inicio**
3. iPhone (Safari): botón compartir (□↑) → **Añadir a pantalla de inicio**

## Si algo no funciona

- Si la página sale en blanco: espera 2-3 minutos más, GitHub Pages a veces tarda en la primera publicación
- Si las imágenes de animales/monumentos no cargan: no es un problema del repositorio, son URLs externas a Wikimedia Commons — revisa el documento de verificación de imágenes que te pasé antes
- Si quieres comprobar que Pages está activo: **Settings → Pages** te dice arriba "Your site is live at ..." con el enlace
