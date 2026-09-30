# 4. Layout compartido

Elementos que se repiten en todas las páginas de la v7 (ver
[03-mapa-del-sitio.md](03-mapa-del-sitio.md)).

## Header (desktop)

Dos franjas:

1. **Barra superior** (38 px, fondo azul oscuro `deep`):
   - Izquierda: teléfono (43965146 / 43965187) y correo general
     (ceac@ceac.cu).
   - Derecha: redes sociales — Facebook, Instagram, YouTube, X y Telegram.
2. **Barra principal** (84 px, fondo blanco con sombra suave):
   - Izquierda: logo original (ícono azul-verde-celeste) + "CEAC" en negro
     (así lo pide el manual de identidad), a 40 px. **Sin el nombre
     completo debajo:** se quitó en la reunión del 2026-09-30 porque el
     hero ya muestra el nombre del centro como título. Pulsar el logo lleva
     al Inicio.
   - Derecha: menú — Proyectos, Servicios, Laboratorio, Investigación,
     Docencia, Noticias, Sobre Nosotros — y el botón "Escríbenos"
     (→ Contacto).
   - La página actual se marca en el menú con el texto en azul y negrita.

## Header (mobile)

- Barra superior con el correo general y las 5 redes.
- Barra principal con el logo + "CEAC" (32 px, sin nombre completo) y un
  botón de menú hamburguesa.
- **Menú abierto** (frame `CEAC v7 - Mobile menú abierto`): pantalla
  completa con las 7 opciones en lista, el botón "Escríbenos" y, abajo, el
  correo y las redes.

## Encabezado de página

Todas las páginas internas (menos los detalles de proyecto y de noticia)
empiezan igual: foto a todo el ancho con un velo degradado azul → verde,
ruta de navegación ("Inicio › Página"), título grande, una bajada y una ola
blanca en el borde inferior.

## Footer

- Fondo degradado azul oscuro → verde oscuro.
- **Logo transparente** (18 % de opacidad) en la esquina inferior derecha,
  recortado por el borde como los adornos. Reemplaza a la palabra "CEAC"
  gigante y al adorno de hojas, que se quitaron en la reunión del
  2026-09-30: según comunicación, las letras cortadas rompían con la
  identidad del centro.
- Columna institucional: nombre completo y dirección (Apartado Postal 5,
  CP 59350, Ciudad Nuclear, Cienfuegos, Cuba).
- **Enlaces rápidos:** Proyectos, Servicios, Laboratorio, Investigación,
  Docencia, Noticias, Sobre Nosotros.
- **Contacto:** Tel. 43965146 / 43965187 · Fax 53-43-965146 · ceac@ceac.cu.
- **Síguenos:** Facebook, Instagram, YouTube, X y Telegram (mismos íconos
  que la barra superior).
- Copyright: "© 2026 Centro de Estudios Ambientales de Cienfuegos. Todos
  los derechos reservados."
- Una ola separa el footer de la sección anterior.

## Elementos comunes

- **Botones:** siempre con bordes totalmente redondeados, relleno 16×30 px
  y texto de 15 px en seminegrita. Principal azul (`blue`) o azul oscuro
  (`deep`); secundario de contorno (azul, azul oscuro o blanco según el
  fondo) con flecha, usado para los "Ver todos…".
- **Etiquetas:** fondo celeste (`sky`) con texto azul (`blue`), un solo
  estilo para categorías, cargos y tipos.
- **Estado (proyectos, programas):** punto azul si está activo o abierto,
  gris si está concluido o próximamente.
- **Olas divisorias:** solo entre secciones que cambian de color, no en
  todas.
- **Carruseles** (colaboradores, investigadores, proyectos en mobile): la
  siguiente tarjeta asoma por el borde para indicar que se puede deslizar;
  en desktop llevan flechas redondas y puntos de posición.

## Notas de implementación

- Header y footer aparecen en todas las páginas: conviene componentizarlos
  desde el principio en vez de copiarlos.
- Los íconos de X y Telegram se dibujaron con su trazo vectorial oficial;
  en código usar los SVG oficiales.
