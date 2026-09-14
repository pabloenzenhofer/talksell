# TalkSell Automation Studio

Sitio institucional y comercial de TalkSell, construido con Astro y preparado para desplegar en Vercel.

## Estructura

```text
talksell/
├── public/
│   ├── robots.txt
│   ├── sitemap.xml
│   └── site.webmanifest
├── src/
│   ├── components/
│   │   ├── CTA.astro
│   │   ├── Footer.astro
│   │   └── Header.astro
│   ├── layouts/
│   │   ├── BaseLayout.astro
│   │   └── LegalLayout.astro
│   ├── pages/
│   │   ├── index.astro
│   │   ├── servicios.astro
│   │   ├── casos.astro
│   │   ├── nosotros.astro
│   │   ├── contacto.astro
│   │   ├── privacidad.astro
│   │   ├── terminos.astro
│   │   ├── cookies.astro
│   │   ├── eliminacion-de-datos.astro
│   │   └── 404.astro
│   └── styles/global.css
├── astro.config.mjs
├── package.json
└── vercel.json
```

## Desarrollo local

Requiere Node.js 20 o superior.

```bash
npm install
npm run dev
```

Para validar la versión de producción:

```bash
npm run build
npm run preview
```

## Despliegue en Vercel

1. Importar este repositorio desde Vercel.
2. Framework preset: Astro.
3. Build command: `npm run build`.
4. Output directory: `dist`.
5. Asociar el dominio `talksellstudio.com`.
6. Configurar el DNS siguiendo las instrucciones de Vercel.

## Datos que deben revisarse antes de publicar

- Confirmar que `info@talksellstudio.com` esté creado y reciba correos.
- Reemplazar el enlace de WhatsApp si TalkSell obtiene una línea propia.
- Reemplazar el CTA por Calendly cuando exista la agenda.
- Confirmar que el domicilio comercial y la identificación del responsable coincidan con la documentación presentada a Meta.
- Agregar CUIT a los textos legales si se decide publicarlo.
- Actualizar la URL canónica si se utiliza otro dominio.

## Meta

URLs preparadas:

- Política de privacidad: `/privacidad`
- Términos: `/terminos`
- Eliminación de datos: `/eliminacion-de-datos`
- Contacto: `/contacto`

Para revisión de permisos también será necesario mostrar en un video el flujo completo, explicar cada permiso solicitado, proporcionar credenciales de prueba si existe login y mantener accesibles las páginas legales mediante HTTPS.

## Recursos visuales

Durante esta primera versión se consumen los recursos públicos del repositorio `pabloenzenhofer/imagenes`. Para máxima independencia se recomienda copiarlos luego a `public/assets` manteniendo las mismas variantes de logo, isotipo y foto.
