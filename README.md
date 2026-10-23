# Portafolio · Eduardo Gama

Sitio estático (HTML + CSS + JS), sin servidor ni compilación. Todas las imágenes viven en `images/` como archivos, nada va incrustado en el código.

## Estructura
```
index.html              Inicio
perfil.html             Perfil (incluye el carrusel de marcas)
casos-de-estudio.html   Casos (pestañas: #plataforma, #bonificaciones, #sell-out)
book.html               Book (galería con carrusel por proyecto)
design-system.html      Sistema de diseño
cv.html                 CV (descarga: assets/Eduardo_Gama_CV.pdf)
contacto.html           Contacto
assets/analytics.js     Google Tag Manager (ver abajo)
assets/Eduardo_Gama_CV.pdf
images/                 plataforma/ bonificaciones/ sell-out/ home/ perfil/ cv/ iconos/ + fondo-textura.svg + favicon.svg
```

## Publicarlo
- **GitHub Pages:** sube el CONTENIDO de esta carpeta a la raíz del repositorio y activa Settings → Pages → Deploy from branch. (`.nojekyll` ya está incluido.)
- **Netlify / Vercel / Cloudflare Pages:** arrastra la carpeta completa.
- Para verlo en local con enlaces y rutas funcionando: `python3 -m http.server` dentro de esta carpeta y abrir http://localhost:8000

## Google Tag Manager
El contenedor `GTM-TDFWC65T` está pegado tal cual en las 7 páginas: el script dentro de `<head>` (lo más arriba posible) y el `<noscript>` justo después de `<body>`. Configura Google Analytics 4 dentro de Tag Manager (etiqueta de configuración GA4 con activador *All Pages*) y publica el contenedor; no pongas el código de GA4 en las páginas, o cada visita se contaría doble. Si usas analítica, agrega aviso de privacidad / cookies según corresponda.

## Cambiar imágenes
Reemplaza el archivo en `images/` conservando el nombre y el formato (WebP). Capturas de escritorio: 2400 px de ancho; teléfonos: 700 px; miniaturas del Inicio: `images/home/`. Cada captura del Book y de Casos tiene tres tamaños: `nombre.webp` (2400 px, visor ampliado), `nombre-m.webp` (1200 px, tarjetas del Book) y `nombre-t.webp` (400 px, tiras de miniaturas). Si cambias una, actualiza las tres versiones.

## Licencia
© 2026 Eduardo Gama. Todos los derechos reservados: el contenido, las imágenes y los textos de este sitio no pueden reutilizarse sin autorización. Los logos de terceros pertenecen a sus respectivos titulares.
