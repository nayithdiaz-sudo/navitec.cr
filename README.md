# NAVITEC · Coming soon

Página temporal de **navitec.cr** mientras se construye el sitio principal.
HTML y CSS estáticos, sin dependencias ni build. Modo claro/oscuro automático según el dispositivo del visitante.

```
index.html          Página completa (estilos y animación incluidos)
assets/             Logos (claro y oscuro), favicon, ícono para iOS
CNAME               Dominio personalizado para GitHub Pages
.nojekyll           Sirve los archivos tal cual, sin procesar con Jekyll
```

## Publicar en GitHub Pages

1. Crear un repositorio (por ejemplo `navitec-web`) y subir el contenido de esta carpeta a la raíz de la rama `main`.
2. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. En **Settings → Pages → Custom domain**, confirmar `navitec.cr` (ya viene en `CNAME`) y activar **Enforce HTTPS** cuando GitHub lo permita.
4. En el DNS del dominio:
   - Registros `A` para `navitec.cr` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - Registro `CNAME` para `www` → `<tu-usuario>.github.io`

Confirma las IPs vigentes en la documentación de GitHub Pages antes de configurar el DNS.

## Probar localmente

Abrir `index.html` en el navegador, o servir la carpeta:

```
python3 -m http.server 8000
```

© 2026 NAVITEC · Soluciones Náuticas. Logos y marca propiedad de NAVITEC; no reutilizar sin autorización.
