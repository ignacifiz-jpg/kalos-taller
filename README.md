# 🔧 Taller Kalos · Web compartida

Web para gestionar el presupuesto del Daewoo Kalos / Chevrolet Aveo 1.6 8v SOHC
con sincronización en tiempo real entre tú y tu compañero.

🌐 **URL pública:** https://ignacifiz-jpg.github.io/kalos-taller/

## 🚀 Configuración inicial (solo una vez, 1 minuto)

### Paso 1 · Crear el "bin" de npoint.io (lo hace UNO de los dos)

1. Abre https://www.npoint.io/
2. Pulsa el botón **"Create"** (azul, arriba a la derecha)
3. Te lleva a un editor con un JSON de ejemplo
4. **Borra todo y deja solo:** `{}`
5. Pulsa **"Save"** (arriba a la derecha)
6. Mira la URL del navegador: será algo como
   `https://www.npoint.io/docs/abc123def456789`
7. **Copia el código final** (lo que va después de `/docs/`)
8. Pásaselo a tu compañero por WhatsApp

### Paso 2 · Conectar la web

Tú y tu compañero hacéis lo mismo:

1. Abrid https://ignacifiz-jpg.github.io/kalos-taller/
2. Aparece una ventana pidiendo el "Bin ID"
3. Pegáis el código que habéis creado en el paso anterior
4. Pulsáis **"Conectar"**
5. ✅ Ya estáis sincronizados

A partir de aquí, cualquier cambio que hagas (marcar trabajo hecho, cambiar
precio, añadir material) se ve en el dispositivo del otro en unos 15 segundos.

## 📱 Acceso desde el móvil

Una vez tengáis la web abierta, podéis añadirla a la pantalla de inicio:

- **iPhone (Safari):** botón compartir → "Añadir a pantalla de inicio"
- **Android (Chrome):** menú (⋮) → "Añadir a pantalla principal"

Te queda como si fuera una app.

## 💡 Funciones de la web

- **Materiales:** los 15 items reales del Kalos (factura Gaudí + AUTODOC).
  Marca/desmarca el check para incluir o excluir del total. Añade nuevos.
- **Presupuesto:** slider del precio al cliente (400-900 €), beneficio total,
  reparto entre los dos en tiempo real, comparativa con taller normal.
- **Trabajos:** checklist de los 11 trabajos con barra de progreso.
  Ambos veis qué está hecho.
- **Técnica:** calado del motor SOHC, procedimiento de distribución,
  útiles necesarios y checklist pre-ITV.

## 🔒 Privacidad

- Los datos viven en npoint.io en un bin público con código aleatorio
- Solo quien tenga el código puede acceder a vuestros datos
- También se guardan en el localStorage del navegador como respaldo
- No metáis datos personales sensibles (DNI, teléfonos del cliente, etc.)

## 🛠 Si queréis editar el código después

El archivo es `index.html` solo. Para modificarlo, lo editas y haces commit
en este repo. GitHub Pages publica los cambios automáticamente en 1-2 minutos.
