# Casa Pioneros 261 — DFS Studio

Presentación web del proyecto Casa Pioneros 261 (Pinamar), de **DFS Studio — Arq & Design**.

La página se recorre solo con el scroll: video exterior, imágenes exteriores, video interior, imágenes interiores, planos y ficha técnica con esquemas de superficies.

## Contenido de la carpeta

```
index.html              la presentación (un solo archivo)
media/
  video-exterior/       337 cuadros del video exterior (001.jpg … 337.jpg)
  video-interior/       145 cuadros del video interior (001.jpg … 145.jpg)
  exteriores/           5 renders exteriores
  interiores/           7 renders interiores
  planos/               3 plantas: subsuelo, baja y alta
  esquemas/             9 esquemas: cubiertos, semicubiertos y envigados por planta
.nojekyll               le indica a GitHub Pages que publique los archivos tal cual
```

Son unos 500 archivos y alrededor de 92 MB. Ningún archivo pasa los 1 MB.

## Publicar con GitHub Pages

### Opción recomendada: GitHub Desktop

La subida desde la web de GitHub acepta hasta 100 archivos por vez, y esta carpeta tiene unos 500. GitHub Desktop sube todo junto.

1. Instalar [GitHub Desktop](https://desktop.github.com/) e iniciar sesión con la cuenta de GitHub.
2. **File → Add local repository…** y elegir esta carpeta. Como todavía no es un repositorio, ofrece **create a repository**: aceptar. Nombre sugerido: `casa-pioneros-261`.
3. Escribir un resumen (por ejemplo "Primera versión") y tocar **Commit to main**.
4. Tocar **Publish repository**. Para usar GitHub Pages gratis, destildar **Keep this code private**.
5. En github.com, abrir el repositorio → **Settings → Pages**. En **Source** elegir **Deploy from a branch**, rama **main** y carpeta **/ (root)**, y guardar.
6. En uno o dos minutos la página queda en `https://USUARIO.github.io/casa-pioneros-261/`, con el nombre de usuario de GitHub en lugar de USUARIO.

### Opción desde la web de GitHub

1. Crear un repositorio nuevo, público, llamado `casa-pioneros-261`.
2. **Add file → Upload files** y arrastrar `index.html`, `.nojekyll` y la carpeta `media`. Si GitHub rechaza la carpeta por tener más de 100 archivos, subir `media/video-exterior` y `media/video-interior` en tandas de menos de 100 archivos, respetando las carpetas.
3. Activar Pages igual que en el paso 5 de arriba.

## Ojo

- **Repositorio público:** con GitHub Pages gratis, cualquiera puede ver y descargar los archivos del repositorio, no solo la página.
- **Modo edición:** en la página publicada no aparece el botón **Editar**. Para verlo, agregar `?editar` al final de la dirección (por ejemplo `…/casa-pioneros-261/?editar`). Los cambios que se hagan ahí no se publican solos: hay que guardarlos (se descarga un `index.html` nuevo) y subir ese archivo al repositorio en lugar del anterior.
- **Primera carga:** los videos son secuencias de cuadros. La primera vez tardan unos segundos en cargarse del todo; después el scroll queda fluido.
- **Nombres de archivo:** GitHub distingue mayúsculas de minúsculas. Si se reemplaza una imagen, conservar exactamente el mismo nombre.
