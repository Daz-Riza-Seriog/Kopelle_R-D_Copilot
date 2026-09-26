# Kopelle I+D Copilot — sitio estático

Este paquete contiene una versión estática del dashboard académico.

## Archivos

- `index.html`: punto de entrada del sitio.
- `style.css`: estilos.
- `data.js`: datos documentales y sintéticos usados por el dashboard.
- `app.js`: lógica e interactividad.
- `.nojekyll`: evita que GitHub Pages procese el sitio con Jekyll.

## Probar localmente

La forma más simple es abrir una terminal en esta carpeta y ejecutar:

```bash
python -m http.server 8000
```

Después visita:

```text
http://localhost:8000
```

## Publicar con GitHub Pages

1. Crea un repositorio nuevo en GitHub, por ejemplo `kopelle-id-copilot`.
2. Sube estos archivos a la raíz del repositorio.
3. Ve a `Settings > Pages`.
4. En `Build and deployment`, selecciona `Deploy from a branch`.
5. Selecciona la rama `main` y la carpeta `/(root)`.
6. Guarda y espera a que GitHub publique el sitio.
7. La URL tendrá normalmente la forma:
   `https://TU-USUARIO.github.io/kopelle-id-copilot/`

## Publicar con ChatGPT Sites

En ChatGPT web:
1. Abre `Work`.
2. Pide crear un sitio web y menciona `@Sites`.
3. Adjunta `index.html`, `style.css`, `data.js` y `app.js`.
4. Indica que debe conservar el contenido y la lógica del dashboard, usando los archivos como fuente.
5. Revisa la vista previa.
6. En `Share`, selecciona la audiencia disponible y, si corresponde, `Anyone on the internet`.
7. Publica solo después de revisar que no exista información confidencial.

## Nota de seguridad

Todo contenido publicado con GitHub Pages o con acceso público en ChatGPT Sites puede quedar accesible por Internet. Antes de publicar, revisa especialmente `data.js`.
