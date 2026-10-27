# Flores Amarillas — Experiencia 💛🌼

Segunda versión experimental de la página para Tifany. Este repositorio es independiente de **Flores-amarilla**: los cambios de aquí no modifican la versión original.

## Estado de esta versión

- Diseño cálido y adaptable a teléfono y computadora.
- Álbum que genera sus tarjetas desde una lista de fotos, en vez de tener solo tres espacios fijos.
- Visor ampliado con botones para foto anterior/siguiente; también admite las flechas del teclado.
- Contador de recuerdos y textos breves debajo de las fotos.
- Carta, música opcional y sorpresa con lluvia de flores.
- Detalle secreto: toca la flor amarilla que aparece encima del título.
- Animaciones respetuosas con la preferencia del sistema para reducir movimiento.

## Ver y publicar

El archivo principal es `index.html`. Para publicar esta versión, abre **Settings → Pages**, selecciona **Deploy from a branch**, elige `main` y `/(root)`, y guarda. Después de que termine la publicación, la dirección normalmente será:

`https://josegarcia6.github.io/Flores-amarillas-experiencia/`

## Cómo añadir fotos al álbum

1. Sube las imágenes a `src/album/` de este repositorio.
2. Usa formatos habituales: JPG, JPEG, PNG, WebP, GIF o AVIF. Es mejor usar nombres sencillos, por ejemplo `recuerdo-04.jpg`.
3. Espera a que los cambios se guarden en la rama `main`. El álbum consulta esa carpeta y añade automáticamente las imágenes que encuentre; **no necesitas editar `index.html` por cada foto**.
4. Las tres fotos originales siguen apareciendo primero. Las nuevas se agregan después y el contador se actualiza automáticamente.

Las descripciones de las nuevas fotos se generan a partir del nombre del archivo. Por ejemplo, `recuerdo-playa.jpg` aparecerá con el texto “recuerdo playa 💛”. Para que el álbum cargue los archivos nuevos, el repositorio debe ser público y las imágenes deben estar confirmadas en `main`. La galería consulta la API pública de GitHub; si esa consulta no está disponible, mantiene las tres fotos originales.

**Importante:** el fondo y la música todavía se cargan desde el repositorio original. Esta versión no modifica esos archivos ni el repositorio original.

## Personalización

- Cambia el mensaje principal y el texto de la carta directamente en `index.html`.
- Para cambiar una foto, edita su `src`, `alt` y `caption` en la lista `photos`.
- La música solo se reproduce cuando la persona toca el botón, como requieren muchos navegadores.

## Privacidad

Si el repositorio es público, el código y las fotos que se suban aquí podrán ser vistos por otras personas. Publica fotografías personales solo si tienes permiso para hacerlo.
