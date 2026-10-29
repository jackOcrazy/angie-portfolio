# angie—f. · Portfolio 2026

Sitio web multipágina y responsive construido a partir de la propuesta editorial de Figma.

## Cómo abrirlo

Abre `index.html` con Chrome o Safari para recorrer el sitio. Todos los recursos visuales están en la carpeta `assets/` y el sitio **no necesita redirigir a Figma**. Las fuentes Syne, DM Sans e IBM Plex Mono se cargan desde Google Fonts cuando hay conexión; sin conexión se utiliza una fuente de respaldo.

Para previsualizarlo con un servidor local (recomendado):

```bash
cd angie-portfolio-web
python3 -m http.server 8000
```

Luego visita `http://localhost:8000/`.

## Publicarlo en Netlify

1. Descomprime el ZIP.
2. Accede a https://app.netlify.com/drop y arrastra **la carpeta** `angie-portfolio-web`.
3. Netlify asigna una URL temporal. Puedes configurar después un dominio propio.

Para Vercel también puedes importar el directorio como un proyecto estático (sin comandos de build). **No he publicado ni vinculado el sitio a un dominio real.**

## Contenido

- `index.html`: portada con Burger King, DolFinTech, MasterBase y Creative Lab.
- `work.html`: directorio de los siete proyectos, filtrable por tipo.
- `burger-king.html`, `dolfintech.html`, `masterbase.html`, `shell-chile.html`, `scholas.html`, `telecom-argentina.html`, `creative-lab.html`: casos de estudio con galerías originales y visor ampliable.
- `about.html` y `contact.html`: perfil profesional y contacto por email.
- `css/styles.css`: sistema visual y estilos responsive.
- `js/data.js`: contenido, textos y referencias de cada proyecto. Edita aquí los textos de las páginas y las piezas.
- `js/app.js`: interacciones, menú móvil, filtros y visor de imágenes.
- `assets/*.webp`: 30 imágenes de las piezas de Figma. Son copias locales; no son enlaces temporales.

Los HTML ya incluyen el contenido para que sea indexable y legible incluso si falla JavaScript. JavaScript añade las interacciones.

## Antes de ponerlo público

Revisa los permisos de publicación de piezas de clientes, el detalle de tu participación y los textos de cada caso. No se incluyen cifras de rendimiento ni resultados no verificados. Se ha utilizado una cuenta de correo facilitada en el CV.

## Cómo editar

Para cambiar texto o la selección de piezas, modifica `js/data.js`: JavaScript reflejará esos cambios al cargar la web. Los HTML también contienen una copia precargada del contenido para buscadores y navegación sin JavaScript; actualízala si haces cambios definitivos importantes. Para cambios visuales, edita `css/styles.css`. Las imágenes se sustituyen en `assets/` conservando el nombre de archivo `.webp`.
