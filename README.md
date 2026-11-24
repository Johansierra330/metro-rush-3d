# Metro Rush 3D — Telegram Mini App (prototipo)

Este proyecto es una primera versión jugable de un corredor infinito 3D inspirado en el género endless runner. Usa Three.js desde CDN y el SDK oficial de Telegram Web Apps.

## Probarlo localmente
1. Abre una terminal en esta carpeta.
2. Ejecuta `python -m http.server 8000`.
3. Abre `http://localhost:8000` en un navegador moderno.

Se necesita conexión a internet para cargar Three.js y el SDK de Telegram.

## Publicarlo para Telegram
Telegram Mini Apps necesitan una URL HTTPS pública:
1. Sube `index.html` a un hosting estático con HTTPS (por ejemplo, GitHub Pages, Netlify o Vercel).
2. En Telegram, abre **@BotFather** y crea un bot con `/newbot`.
3. En BotFather configura el menú Mini App con `/setmenubutton` (o configura una Main Mini App desde la configuración del bot) y pega la URL HTTPS publicada.
4. Abre el bot y pulsa el botón de la Mini App.

## Controles
- Deslizar a izquierda/derecha: cambiar de carril.
- Deslizar hacia arriba: saltar.
- Deslizar hacia abajo: deslizarse.
- En escritorio: flechas o WASD; espacio para saltar.

## Próximas mejoras recomendadas
- Modelos 3D y animaciones originales para el personaje.
- Sonidos y música con controles de volumen.
- Misiones, tienda, skins y tabla de clasificación.
- Guardado seguro de récords en un backend.
- Validación del `initData` de Telegram en servidor antes de confiar en datos del usuario.

Este prototipo no incluye todavía backend, cuentas, pagos ni clasificación compartida. No reutiliza personajes, nombres, música ni recursos oficiales de Subway Surfers.
