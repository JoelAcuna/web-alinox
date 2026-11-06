# Alinox · Fundición de aluminio

SPA en español con seis niveles, ascensor animado, catálogo CSS 3D, fichas de producto, estaciones del equipo y taller interactivo. JavaScript ES modules y CSS; Vite para desarrollo y compilación.

## Desarrollo

Requiere Node.js 22 o superior y npm.

```sh
npm ci
npm run dev -- --port 5173
```

```sh
npm run build
npm run preview -- --port 4173
```

## Contacto comercial

Copia `.env.example` a `.env.local` y establece `VITE_WHATSAPP_NUMBER` con el número comercial real, incluido el código de país. Reinicia Vite después de modificarlo. El mensaje incluye el piso o producto seleccionado. Sin número, la aplicación permite copiar la solicitud y explica que falta configurar el contacto. No se usa un número ficticio.

Las fichas y representaciones de productos son ilustrativas; confirmar especificaciones y catálogo antes de publicar comercialmente. Las fotografías de ambientación se cargan desde Unsplash y las fuentes desde Google Fonts; sin conexión se mantienen las fuentes de respaldo y los fondos sólidos.

## Interacción

Botones 0–5: cambiar de nivel. En móvil: abrir «Pisos». Catálogos: arrastrar horizontalmente o usar las flechas para girar 60 grados. Seleccionar un producto abre su ficha. Los diálogos se cierran con Escape, el botón de cierre o el fondo. El sonido mecánico es opcional. Se respeta la preferencia de movimiento reducido.
