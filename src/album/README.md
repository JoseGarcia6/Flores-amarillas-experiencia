# Álbum de fotografías 🌻

Esta carpeta está preparada para guardar las fotografías adicionales de la experiencia.

## Cómo agregar fotos

1. Subí las imágenes a esta carpeta (`src/album/`).
2. Usá nombres sencillos, por ejemplo `recuerdo-04.jpg`.
3. En `index.html`, agregá cada imagen al arreglo `photos`, usando una ruta como:

```js
{
  src: "src/album/recuerdo-04.jpg",
  alt: "Descripción de la foto",
  caption: "Una frase bonita 💛"
}
```

Formatos recomendados: JPG, JPEG, PNG o WebP. Para que aparezcan en la galería, la imagen también debe agregarse al arreglo `photos` de `index.html`.
