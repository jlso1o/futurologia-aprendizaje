# Futurología del Aprendizaje — repositorio de materiales

Sitio de consulta de materiales académicos construido con Jekyll, Minimal Mistakes y GitHub Pages.

## Publicar en GitHub Pages

1. Crea un repositorio público llamado `futurologia-aprendizaje`.
2. Sube **el contenido de esta carpeta**, no la carpeta contenedora, a la raíz del repositorio. Incluye los archivos y carpetas que comienzan por `_`.
3. Edita `_config.yml`: sustituye `USUARIO` en `url` y `repository` por tu cuenta de GitHub. Si usas un nombre de repositorio distinto, modifica también `baseurl`.
4. Abre **Settings → Pages → Build and deployment** y selecciona **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
5. Espera a que GitHub Pages publique el sitio y accede a `https://USUARIO.github.io/futurologia-aprendizaje/`.

El tema remoto de Minimal Mistakes y `jekyll-include-cache` están configurados. Requiere que GitHub Pages pueda construir el sitio con Jekyll.

## Incorporar un material

- Agrega una nueva fila en la tabla de la página `_pages/unidad-N.md` (hay un ejemplo comentado) o inserta un enlace debajo de "Materiales de consulta".
- Enlaza el recurso público original o agrega archivos propios/autorizados en `assets/documentos/` y `assets/presentaciones/`.
- Para archivos subidos, usa enlaces Liquid: `[Abrir PDF]({{ '/assets/documentos/archivo.pdf' | relative_url }})`.
- Evita subir archivos protegidos por derechos de autor sin autorización.

## Diseño

- Sin banners, calendarios ni módulos de entrega.
- Navegación superior: Inicio, Unidades, Biblioteca, Recursos y Acerca de.
- Páginas intencionalmente limpias, sin contenidos ficticios.
- Cambia `minimal_mistakes_skin: "air"` en `_config.yml` para probar otra variante de color.

## Probar localmente (opcional)

Con Ruby y Bundler instalados: `bundle install && bundle exec jekyll serve`.
