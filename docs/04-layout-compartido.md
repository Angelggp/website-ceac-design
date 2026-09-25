# 4. Layout compartido

Se diseña **una sola vez** y se reutiliza en todas las páginas listadas en
[03-mapa-del-sitio.md](03-mapa-del-sitio.md).

## Header

- Logo "CEAC" (`font-display`, bloque con gradiente azul) → link a Inicio
- Navegación: Inicio, Nosotros, Proyectos, Servicios, Investigación,
  Noticias, Contacto
- Botón CTA a la derecha: "Escríbenos" → Contacto
- Fondo blanco con sombra suave; sin selector de idioma ni de tema (sitio
  solo en español, un modo por ahora)

## Footer

- "CEAC" + nombre completo: "Centro de Estudios Ambientales de Cienfuegos"
- Dirección: Apartado Postal 5, CP 59350, Ciudad Nuclear, Cienfuegos, Cuba
- Contacto: Tel. 43965146 / 43965187 · Fax 53-43-965146 · ceac@ceac.cu
- Enlaces rápidos: Proyectos, Servicios, Investigación, Docencia, Noticias,
  Sobre Nosotros
- "Síguenos" (redes sociales)
- Copyright: "© 2026 Centro de Estudios Ambientales de Cienfuegos. Todos los
  derechos reservados."

## Notas de implementación

- Header y footer son los únicos elementos que aparecen en **todas** las
  plantillas de página (ver [`paginas/`](paginas/)) — conviene componentizarlos
  desde el día 1 (partial, componente compartido, layout base, etc.) en vez
  de copiarlos por página.
- Usan los tokens de [02-tokens-de-diseno.md](02-tokens-de-diseno.md)
  (`color-primary`, `font-display`, `color-border` para la sombra suave del
  header, `radius-*` en el botón CTA).
