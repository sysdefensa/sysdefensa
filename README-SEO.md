# SEO técnico — Sagredo Srdanovic & Cía

Dominio configurado en los archivos: `https://www.sagredosrdanovic.cl/`

Si el dominio final es distinto, reemplazarlo en:
- `index.html`
- `sitemap.xml`
- `robots.txt`
- `site.webmanifest`
- páginas de servicio en la raíz (`*.html`)
- `.htaccess` si se usa Apache

## Archivos incluidos

- `index.html`: landing principal optimizada con title, meta description, canonical, Open Graph, Twitter Card, hreflang, JSON-LD y contenido visible.
- `robots.txt`: permite rastreo general y declara el sitemap.
- `sitemap.xml`: incluye la home y páginas canónicas de servicios.
- `site.webmanifest`: metadatos básicos de instalación y tema.
- `favicon.ico`, `favicon.svg`, `assets/favicon-*`, `assets/apple-touch-icon.png`: favicons e íconos.
- `assets/og-yerko-sagredo-srdanovic.jpg`: imagen social 1200x630 para Open Graph/Twitter.
- `assets/foto-abogado-yerko-sagredo-srdanovic.webp`: versión WebP optimizada de la foto principal.
- `litigacion-civil-responsabilidad-civil.html`, `derecho-familia.html`, `juicios-ejecutivos-defensa-patrimonial.html`, `derecho-administrativo-sector-publico.html`, `asesoria-estrategica-informes-en-derecho.html`, `derecho-laboral.html`, `derecho-penal.html`: páginas SEO friendly para cada área legal ubicadas en la raíz.
- `404.html`: página de error con `noindex, follow`.
- `.htaccess`: reglas para HTTPS, canonical www, caché y headers en Apache.
- `_headers`: headers equivalentes para Netlify/Cloudflare Pages.

## Acciones posteriores al despliegue

1. Subir todo el contenido a la raíz del hosting.
2. Confirmar que la home responda HTTP 200.
3. Configurar SSL y redirección HTTP → HTTPS.
4. Revisar si el dominio final será con `www` o sin `www` y dejar solo una versión.
5. Verificar propiedad en Google Search Console.
6. Pegar el código de verificación en el comentario de `index.html`:
   `<meta name="google-site-verification" content="..." />`
7. Enviar `sitemap.xml` en Search Console.
8. Validar datos estructurados con Rich Results Test o Schema Markup Validator.
9. Medir Core Web Vitals en PageSpeed Insights.
10. Completar la ubicación real si la oficina quiere posicionamiento local por ciudad o comuna.

## Importante

No se agregó dirección física porque no venía en el documento base. Para SEO local fuerte, conviene completar dirección, comuna/ciudad, horario y ficha de Google Business Profile.

## Corrección de estructura de servicios

Las páginas de servicio quedaron en la raíz del proyecto, no dentro de `/servicios/`. Los enlaces internos, canonical, Open Graph, sitemap y JSON-LD apuntan a los archivos raíz `.html`. El `.htaccess` mantiene redirecciones 301 desde las URLs antiguas `/servicios/.../` hacia las nuevas URLs raíz para evitar errores si ya existían enlaces externos.
