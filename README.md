# 🔧 Taller Kalos · Web compartida

Web para gestionar el presupuesto del Daewoo Kalos / Chevrolet Aveo 1.6 8v SOHC
con sincronización en tiempo real entre tú y tu compañero.

## 🚀 Cómo desplegarla en internet (gratis, 3 minutos)

### Paso 1 · Subir la web a Netlify

1. Entra en https://app.netlify.com/drop
2. Arrastra el archivo `index.html` a la zona indicada
3. Netlify te dará una URL del tipo: `https://random-name-12345.netlify.app`
4. ✅ Esa URL ya funciona desde móvil y PC

(Alternativa: https://surge.sh o https://vercel.com también valen)

### Paso 2 · Crear la base de datos compartida (JSONBin.io)

**Solo lo hace UNO de los dos, una vez.**

1. Entra en https://jsonbin.io/login y crea cuenta (gratis, sin tarjeta)
2. En el dashboard pulsa **"Create Bin"**
3. En el editor pega: `{}`
4. Pulsa **"Create"**
5. Copia el **BIN ID** (texto largo en la URL, después de `/b/`)
6. Ve a **API Keys** (menú lateral) y copia tu **MASTER KEY** (X-Master-Key)
7. Pásale ambos códigos a tu compañero por WhatsApp

### Paso 3 · Configurar la web

Cuando abras la URL de Netlify la primera vez:

1. Aparece una ventana pidiendo BIN ID y MASTER KEY
2. Los pegáis ambos (tú y tu compañero) en vuestros respectivos navegadores
3. Pulsáis "Conectar"
4. ✅ Ya estáis sincronizados

A partir de aquí, cualquier cambio que hagas (marcar trabajo hecho, cambiar
precio, añadir material) se ve en el dispositivo del otro en unos segundos.

## 📱 Acceso desde el móvil

Una vez tengáis la URL de Netlify, podéis añadirla a la pantalla de inicio:

- **iPhone:** Safari → botón compartir → "Añadir a pantalla de inicio"
- **Android:** Chrome → menú (⋮) → "Añadir a pantalla principal"

Te queda como si fuera una app.

## 💡 Funciones de la web

- **Materiales:** los 15 items reales del Kalos (factura Gaudí + AUTODOC).
  Marca/desmarca para incluir o excluir del total. Añade nuevos.
- **Presupuesto:** mueve el slider del precio al cliente y mira el beneficio
  y el reparto entre los dos en tiempo real.
- **Trabajos:** checklist de los 11 trabajos. Ambos veis qué está hecho.
- **Técnica:** calado del motor SOHC, procedimiento de distribución,
  útiles necesarios y checklist pre-ITV.

## 🔒 Privacidad

- Los datos viven en TU bin de JSONBin (gratis hasta 10k peticiones/mes)
- Nadie más puede leerlos sin la Master Key
- También se guardan en el localStorage del navegador como respaldo

## 🛠 Si queréis editar después

El archivo es `index.html` solo. Si queréis cambiar algo (añadir trabajos
por defecto, modificar estilos, etc.) abrid el archivo con un editor de texto
y subidlo de nuevo a Netlify arrastrándolo.

Para no tener que meter el BIN ID y MASTER KEY cada vez que cambiéis de PC,
podéis pegarlos directamente en el código en estas dos líneas:

```js
const HARDCODED_BIN_ID = '';      // pega aquí
const HARDCODED_MASTER_KEY = '';  // pega aquí
```

(Pero si haces eso, no subas el archivo a sitios públicos como GitHub porque
quien tenga la Master Key puede leer/escribir en vuestro bin.)
