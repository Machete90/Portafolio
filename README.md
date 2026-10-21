# Portafolio · Fabio M. Terceros Argote

Portafolio web de diseño gráfico: branding, packaging, marketing digital y trabajos de Manaco S.A. (Bata Bolivia).
Es una sola página estática (HTML + CSS + JavaScript simple), sin dependencias ni instalación.

## Estructura

```
index.html        La página completa (estilos y scripts incluidos)
img/              Imágenes del portafolio (WebP) y logo
cv/               CV en PDF (botón "Descargar CV")
firebase.json     Configuración opcional para Firebase Hosting
extras/           Flujo opcional de GitHub Actions para Firebase
.nojekyll         Evita que GitHub Pages procese los archivos
```

## Verlo en tu computadora

Abre `index.html` con doble clic. Debe quedar junto a las carpetas `img` y `cv`.
Con servidor local (opcional): `python3 -m http.server 8000` y entra a http://localhost:8000

## Publicarlo en GitHub Pages

1. Crea un repositorio en GitHub (por ejemplo `portafolio`).
2. Sube los archivos:
   - **Desde la web:** botón *Add file → Upload files* y arrastra el contenido de esta carpeta (incluidas `img` y `cv`).
   - **Con git:**
     ```bash
     git init
     git add .
     git commit -m "Portafolio"
     git branch -M main
     git remote add origin https://github.com/TU-USUARIO/portafolio.git
     git push -u origin main
     ```
3. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)`. Guarda.
4. En 1 o 2 minutos estará en `https://TU-USUARIO.github.io/portafolio/`
   (si el repositorio se llama `TU-USUARIO.github.io`, la dirección es `https://TU-USUARIO.github.io/`).

## Actualizar el portafolio

- **Cambiar el CV:** reemplaza `cv/CV_Fabio_Terceros_Argote.pdf` conservando el nombre.
- **Agregar o cambiar imágenes:** guarda la imagen en `img/` (recomendado WebP o JPG de unos 1200 px de ancho) y referénciala en `index.html`.
- Sube los cambios con `git add . && git commit -m "Actualización" && git push`.

## Firebase (opcional)

Con `firebase.json` ya incluido: `firebase login`, `firebase init hosting` (carpeta pública `.`, sin sobrescribir `index.html`) y `firebase deploy`.
Para publicar automáticamente desde GitHub revisa `extras/firebase-hosting.yml`.

## Derechos

© Fabio M. Terceros Argote. Todos los derechos reservados.
Las marcas y trabajos mostrados pertenecen a sus respectivos clientes y se muestran como muestra de portafolio.
