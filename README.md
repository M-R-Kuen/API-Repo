# Pasos para desplegar la API/servidor

### 1. Archivos JSON

Se proporcionará un archivo `.zip` que contiene los archivos `.json` tanto en español como en inglés.

### 2. Despliegue de los archivos JSON

Si desean desplegar los archivos JSON desde GitHub, continúen con el paso 3. De lo contrario, pasen directamente al siguiente paso (despliegue del servidor N°7).

### 3. Crear repositorio en GitHub

- Crear un repositorio **público** en GitHub.
- Subir los dos archivos `.json` dentro de una carpeta con el nombre de su elección (por ejemplo, `api`).

### 4. Configurar GitHub Pages

- Una vez creado el repositorio y subida la carpeta con los archivos, ir a la sección **Settings** del repositorio.
- En el menú lateral izquierdo, hacer clic en **Pages**.
- En la opción **Source**, seleccionar **Deploy from a branch** y configurar la rama `main`.
- Guardar los cambios haciendo clic en el botón **Save**.

### 5. Publicación del sitio

- Esperar unos minutos hasta que GitHub indique que el sitio está disponible con el mensaje: **Your site is live at [URL-del-repositorio]**.
- Hacer clic en el botón **Visit site** para abrir el sitio.

### 6. Acceder a los archivos JSON

- En la URL del sitio, acceder a los archivos JSON añadiendo la ruta de la carpeta y el nombre del archivo. Ejemplo:

```
https://[usuario].github.io/[nombre-del-repositorio]/api/es-generated.json
```

### 7. Despliegue del servidor

- Utilizar una plataforma de hosting para desplegar el servidor. Algunas plataformas recomendadas son: **Vercel**, **Render**, **Netlify**, o **Heroku**.

### 8. Configurar variables de entorno

- Según la plataforma de hosting elegida, agregar las siguientes variables de entorno:

```
API_URL_ES = "tu_ruta_de_jsonES"
API_URL_EN = "tu_ruta_de_jsonEN"
```

- **Nota:** Es importante utilizar exactamente los nombres `API_URL_ES` y `API_URL_EN`, ya que el servidor está configurado para reconocer solo esos nombres. De lo contrario, no funcionará correctamente.
