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

## Publicación con GitHub Pages

El workflow `.github/workflows/deploy-pages.yml` compila y publica al actualizar `main`. Vite configura `/web-alinox/` como base de producción; el desarrollo local conserva `/`.

En GitHub, abre **Settings → Pages → Build and deployment → Source** y selecciona **GitHub Actions**. El workflow intenta activar Pages automáticamente; si los permisos del repositorio no lo permiten, selecciona la opción anterior y vuelve a ejecutar **Actions → Publish website to GitHub Pages → Run workflow**.

Dirección tras un despliegue exitoso: https://joelacuna.github.io/web-alinox/

## Galería panorámica 3D

La experiencia principal ocupa la pantalla completa y representa una sala circular mediante CSS 3D, con paredes, iluminación y pedestales. Arrastra horizontalmente para mirar alrededor o usa las flechas de la interfaz. También puedes enfocar la galería con Tab y usar las flechas del teclado. «Explorar esta pieza» abre el elemento situado al frente. El ascensor cambia entre los seis niveles sin recargar la página. Las piezas son representaciones estilizadas en CSS, no modelos CAD descargables.
