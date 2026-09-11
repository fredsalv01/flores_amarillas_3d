# 🌷 Una pequeña historia para el 21 de septiembre

Esta es una experiencia web 3D hecha con Three.js.

La historia:
1. Introducción.
2. Una niña comienza a caminar.
3. Encuentra 3 cartas repartidas por el camino.
4. Cada carta contiene un mensaje.
5. Entre las cartas aparece un recuerdo/foto.
6. Finalmente llega al campo de tulipanes.
7. Se revela la foto de ella.
8. Aparece el mensaje final.

## Ejecutar

No necesitas instalar Node.js para esta versión.

Por las políticas de módulos del navegador, es mejor usar un servidor local.

### Opción 1 — Python

Dentro de la carpeta:

```bash
python -m http.server 5500
```

Abre:

http://localhost:5500

### Opción 2 — VS Code

Instala la extensión "Live Server" y abre `index.html` con Live Server.

## Fotos

Dentro de:

```text
assets/photos/
```

coloca:

```text
ella.jpeg
foto1.jpg
foto2.jpg
foto3.jpg
```

La página utiliza `ella.jpeg` como foto principal.

`foto1.jpg` aparece durante el recorrido. Los archivos `foto2.jpg` y `foto3.jpg` quedan preparados para que puedas ampliar la historia.

Si quieres usar otras extensiones, cambia las rutas en `index.html`.

## Música

La música está generada con Web Audio API al pulsar "Comenzar", por lo que no tienes que conseguir un MP3 ni preocuparte por copyright para esta demo.

Es una melodía ambiental sencilla. Puedes sustituirla por una canción propia/licenciada posteriormente.

## Publicar

Puedes subir el proyecto a GitHub Pages, Vercel o Netlify.

Importante: mantén `index.html`, `styles.css`, `app.js` y la carpeta `assets` en la raíz.

## Personalizar las cartas

En `app.js` busca:

```js
const letterTexts=[
 ...
];
```

Ahí puedes cambiar los 3 mensajes.

## Personalizar la firma

En `index.html` busca:

```html
Con amor, <i>tu chico color canelita pasion ♥️</i>
```

## Nota sobre el personaje

La niña está construida proceduralmente con geometría de Three.js para que no dependamos de modelos 3D externos. Es un estilo low-poly/ilustrado y se puede reemplazar posteriormente por un modelo GLB más detallado si quieres una calidad todavía más cinematográfica.
