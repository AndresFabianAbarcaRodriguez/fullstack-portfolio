# Validación local — 8 de octubre de 2026

## Comprobaciones realizadas

- Revisión de los archivos originales: los tres proyectos eran HTML/CSS estáticos, sin scripts, API ni backend.
- Comprobación de etiquetas HTML correctamente anidadas, identificadores únicos, archivos referenciados y destinos de anclas en las cuatro páginas: sin incidencias.
- `node --check js/main.js`: sintaxis correcta.
- Edge mediante Playwright, a 375, 768 y 1440 píxeles de ancho, en las cuatro páginas: sin desbordamiento de documento o elementos, imágenes rotas ni anclas inexistentes.
- Consola del navegador y excepciones JavaScript: sin errores en la última ejecución.
- Menú móvil: apertura, Escape y cierre tras navegación comprobados.
- Revisión visual de capturas completas de la página principal en escritorio y móvil.
- Accesibilidad básica revisada en código: idioma, HTML semántico, un h1 por página, texto alternativo del retrato, enlace para saltar al contenido, foco visible, botón de menú con estado expandido y preferencias de movimiento reducido.
- Enlaces de código contrastados con el remoto configurado y los archivos de `origin/main` disponibles localmente.
- Retrato optimizado de PNG (1.012.481 bytes) a WebP (49.620 bytes), conservando el original.
- `git diff --check`: sin errores de espacios en la revisión final.

El resultado de las pruebas de navegador está en `browser-check.json`; las capturas de portada están en `previews/`.

## Límites y pendientes

No se hizo una auditoría WCAG completa, validación W3C, Lighthouse ni pruebas en dispositivos físicos, Safari o Firefox. La accesibilidad básica revisada no equivale a una certificación de conformidad.

Los enlaces de LinkedIn y Credly conservan exactamente los destinos proporcionados por el autor. No se verificó su disponibilidad pública ni la titularidad de las credenciales en línea.

No existe un PDF de CV: se muestra el pendiente y se documenta cómo incorporar un enlace funcional cuando exista. No se han inventado repositorios para los demás proyectos académicos.

No se publicó en Vercel ni se ejecutaron commits, push o cambios remotos. El sitio es estático y no necesita compilar.
