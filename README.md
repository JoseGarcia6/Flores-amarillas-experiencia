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

1. Sube la foto nueva a una carpeta `src/album/` de este repositorio. Usa nombres sencillos, por ejemplo `recuerdo-04.jpg`.
2. Abre `index.html` y busca el bloque `const photos = [`.
3. Añade un objeto más dentro de la lista, separándolo con una coma:

```js
{src:"src/album/recuerdo-04.jpg",alt:"Descripción de la foto",caption:"Una frase bonita 💛"}
```

4. Guarda los cambios. El álbum se adapta automáticamente al número de fotos; no hace falta crear botones manualmente.

**Importante:** las tres fotos actuales, el fondo y la música se cargan temporalmente desde los archivos del repositorio original para conservar el aspecto mientras preparamos esta versión. Cuando quieras que este proyecto sea completamente autónomo, copia también esos cinco archivos a su propia carpeta `src/` y cambia sus rutas en `index.html` a rutas locales. El repositorio original no se modifica.

## Personalización

- Cambia el mensaje principal y el texto de la carta directamente en `index.html`.
- Para cambiar una foto, edita su `src`, `alt` y `caption` en la lista `photos`.
- La música solo se reproduce cuando la persona toca el botón, como requieren muchos navegadores.

## Privacidad

Si el repositorio es público, el código y las fotos que se suban aquí podrán ser vistos por otras personas. Publica fotografías personales solo si tienes permiso para hacerlo.
