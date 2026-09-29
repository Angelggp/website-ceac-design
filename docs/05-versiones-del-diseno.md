# 5. Versiones del diseño

Registro de todas las propuestas del diseño, qué contiene cada una y por
qué se pasó a la siguiente. **La versión vigente es la v7.**

**Dónde está cada cosa:**

- **Rama `main`:** `ceac-modern.pen` contiene **solo la v7**, desde la
  esquina superior izquierda del lienzo. Las páginas desktop van en una
  fila, de izquierda a derecha; las mobile de Proyectos, Detalle de
  proyecto y Servicios están debajo de su versión desktop.
- **Rama `historial-versiones`:** conserva el `ceac-modern.pen` completo,
  con los bocetos previos y las versiones v1 a v7, por si hace falta
  consultarlas o recuperar algo. Para verlo: `git checkout
  historial-versiones` (y volver con `git checkout main`).

## Resumen

Los frames de v1 a v6 y los bocetos previos solo existen en la rama
`historial-versiones`.

| Versión | Frames | Concepto | Estado |
|---|---|---|---|
| Históricos | `CEAC Home Modern`, `CEAC Actual`, `CEAC HomePage`, `About us seccion`, `CEAC — Inicio` | Bocetos previos a este registro | Historial |
| v1 | `CEAC Diseño rápido - Desktop / Mobile` | Primera prueba: verdes y beige, tono cálido | Historial |
| v2 | `CEAC v2 - Desktop` | Verde + beige, secciones del home según la documentación | Historial |
| v3 | `CEAC v3 - Desktop` | "Inmersión batimétrica": todo en azul, profundidades | Historial |
| v4 | `CEAC v4 - Desktop`, `CEAC v4 - Menú abierto`, `Ornamentos v4` | "El manglar": azul + verde, formas de pétalo, adornos botánicos | Historial |
| v5 | `CEAC v5 - Desktop`, `Ornamentos v5` | Mezcla de v2 y v3 con el contenido real del centro | Historial |
| v6 | `CEAC v6 - Desktop` | Home resumida en 8 bloques | Descartada |
| **v7** | `CEAC v7 - …` (ver abajo) | Home de 6 secciones de un solo tema + todas las páginas internas | **Vigente** |

## Versiones anteriores

### v1 — Diseño rápido

Primera prueba con Pencil a partir de un brief inspirado en UMCES y
Wholegrain Digital. Paleta de verdes naturales, azul suave y beige;
titulares en Fraunces y texto en Inter. Secciones: hero con foto de
manglar, "Qué hacemos", equipo, proyectos y publicaciones, colaboración y
footer. Tiene versión mobile.

### v2

Toma la estructura de secciones de [paginas/inicio.md](paginas/inicio.md).
Hero con la foto real del edificio del CEAC en un arco, badge del OIEA y
cifras en vidrio. Proyectos en tarjetas escalonadas, laboratorio en azul
marino, posgrado, noticias, investigación con cifra grande, colaboradores,
mapa con formulario y footer. Se descartó porque el verde dominaba sobre
el azul del logo.

### v3 — Inmersión batimétrica

El sitio se lee como un descenso desde la superficie de la bahía: cada
sección lleva su profundidad (0 m, −5 m, −15 m…), con curvas de nivel y
coordenadas como recurso gráfico. Todo en azul, con el verde solo como
acento. Aportó el lenguaje de olas divisorias, cápsulas de fotos y la
palabra CEAC gigante del footer, que llegaron a la v7.

### v4 — El manglar

Mezcla azul y verde con un degradado de malla en el hero, fotos con forma
de pétalo y adornos SVG generados (rama, pez y hojas) en algunas esquinas.
Primera prueba de menú hamburguesa con pantalla de menú abierto. Se
descartó por recargada y por la falta de coherencia del navbar.

### v5

Combina v2 y v3 con el contenido real del centro: proyectos por categoría
(territoriales, nacionales, internacionales), servicios científicos y
estatales, solo diplomados y cursos de posgrado, artículos por año,
colaboradores y clientes separados y fundadores en Nosotros. Adornos de
atmósfera, tierra y aguas. **De aquí sale el menú y el logo que usa la
v7.** Se descartó por demasiado larga (11 secciones en el home).

### v6

Intento de resumir el home en 8 bloques con enlaces "Ver más". Se descartó
porque mezclaba conceptos distintos en una misma sección (proyectos,
servicios, laboratorio y docencia en una sola tarjeta) y seguía
sintiéndose recargada.

## v7 — Versión vigente

### Decisiones que la definen

- **Home de 6 secciones, una idea por sección:** Hero, Proyectos,
  Servicios, Laboratorio, Noticias y Contacto (más Colaboradores
  internacionales). El resto del contenido vive solo en su página.
- **Azul y verde, como el logo:** azul institucional para texto, botones y
  etiquetas; el verde queda en los degradados del hero y del footer.
- **Navbar de dos franjas:** barra superior azul con teléfono, correo y
  redes; barra principal blanca con el logo original y el menú.
- **Olas divisorias** entre secciones que cambian de color, no en todas.
- **Botones estandarizados:** todos con bordes totalmente redondeados,
  mismo relleno y texto de 15 px en seminegrita.
- **Sin correos a la vista:** el contacto con investigadores pasa por el
  formulario de Contacto.
- **Sin estadísticas** en el home (se quitaron a pedido).

### Frames de la v7

Son los únicos frames del `ceac-modern.pen` en `main`. Desktop en la fila
principal; las mobile de Proyectos, Detalle de proyecto y Servicios están
debajo de su versión desktop.

| Página | Desktop | Mobile |
|---|---|---|
| Inicio | `CEAC v7 - Desktop` | `CEAC v7 - Mobile` + `CEAC v7 - Mobile menú abierto` |
| Proyectos | `CEAC v7 - Proyectos (Desktop)` (por bloques) y `CEAC v7 - Proyectos con filtro (Desktop)` | `CEAC v7 - Proyectos (Mobile)` (por bloques) |
| Detalle de proyecto | `CEAC v7 - Detalle de proyecto (Desktop)` | `CEAC v7 - Detalle de proyecto (Mobile)` |
| Servicios | `CEAC v7 - Servicios (Desktop)` | `CEAC v7 - Servicios (Mobile)` |
| Laboratorio | `CEAC v7 - Laboratorio (Desktop)` | `CEAC v7 - Laboratorio (Mobile)` |
| Investigación | `CEAC v7 - Investigación (Desktop)` | `CEAC v7 - Investigación (Mobile)` |
| Sobre nosotros | `CEAC v7 - Sobre nosotros (Desktop)` | `CEAC v7 - Sobre nosotros (Mobile)` |
| Docencia | `CEAC v7 - Docencia (Desktop)` | `CEAC v7 - Docencia (Mobile)` |
| Noticias | `CEAC v7 - Noticias (Desktop)` | `CEAC v7 - Noticias (Mobile)` |
| Detalle de noticia | `CEAC v7 - Detalle de noticia (Desktop)` | `CEAC v7 - Detalle de noticia (Mobile)` |
| Contacto | `CEAC v7 - Contacto (Desktop)` | `CEAC v7 - Contacto (Mobile)` |

El detalle de cada página está en [`paginas/`](paginas/).

### Pendientes de la v7

- **Proyectos:** elegir entre la versión por bloques y la versión con
  filtro. La mobile hecha corresponde a la de bloques.
- **Contenido real** (hoy es de relleno): lista de proyectos con su ficha,
  investigadores (nombre, cargo, foto), artículos con sus enlaces,
  noticias, fundadores, servicios, parámetros acreditados del laboratorio,
  oferta de programas de docencia, horario de atención y preguntas
  frecuentes.
- **Confirmar:** que el laboratorio está acreditado bajo NC-ISO/IEC 17025
  y la lista de colaboradores internacionales (USAC se identificó solo por
  su logo).
- **Recursos gráficos:** logos de los colaboradores y fotos reales del
  centro (hoy son de stock, salvo el edificio y las insignias de
  reconocimientos).
- **Opcional:** convertir header, footer, botones y tarjetas en componentes
  reutilizables de Pencil.

## Notas para desarrollo

- **Íconos de X y Telegram:** la librería de íconos de Pencil no los trae;
  están dibujados como trazo vectorial con el logo oficial. En código,
  usar los SVG oficiales.
- **Contactar a un investigador:** no usar enlaces `mailto:` con la
  dirección en el HTML. El botón debe abrir el formulario de Contacto con
  el motivo "Contactar a un investigador", y el envío debe hacerse desde el
  servidor.
- **Botones que llevan a Contacto:** "Escríbenos", "Solicitar un servicio",
  "Solicitar un ensayo", "Solicitar información" y "Contactar" abren la
  página de Contacto con el motivo correspondiente ya marcado.
