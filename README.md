# Abiertly · sitio web
Sitio estático (HTML, CSS y JavaScript). No necesita instalar nada.

- `index.html`: la página. `privacidad.html` y `terminos.html`: borradores legales. `404.html`: página de error.
- `css/sitio.css`, `js/sitio.js`: estilos y comportamiento.
- `assets/`: foto, íconos e imagen para compartir.
- `_headers`: reglas de seguridad y caché para Cloudflare Pages.

## Ver en el computador
Desde esta carpeta: `python3 -m http.server 5173` y abrir http://127.0.0.1:5173

## Antes de lanzar con dominio propio
1. Quitar `<meta name="robots" content="noindex,nofollow">` de `index.html`, `privacidad.html`, `terminos.html` y `404.html`.
2. Cambiar `og:image` por la dirección completa con el dominio.
3. Revisar los textos que están entre [corchetes] en privacidad y términos con un abogado.
4. Confirmar precios, días y las respuestas marcadas [confirmar] (están en copy.md del proyecto privado).

## Publicar
Cloudflare Pages: conectar este repositorio, sin comando de build, carpeta de salida: `/` (raíz).
