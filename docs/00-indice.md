# Diseño Web CEAC — Índice de documentación

> Este set de documentos reemplaza a la plantilla monolítica original
> (`Estructura-de-Diseno-Web-CEAC.pdf`, conservada como referencia histórica)
> desestructurándola en piezas independientes, más fáciles de consultar y de
> ir marcando como "listas" durante la implementación.

## Cómo usar esto

1. Leé **una sola vez** los documentos base (01 a 04): definen la identidad,
   los tokens de diseño, el mapa del sitio y el layout compartido. Todo el
   resto del sitio consume estas definiciones — ninguna página inventa un
   color, una fuente o una medida propia.
2. Entrá a [`paginas/`](paginas/) y trabajá **una página a la vez**. Cada
   archivo es autocontenido: objetivo, secciones, CTA principal y notas de
   diseño puntuales.
3. Antes de maquetar o picar código, repasá el checklist de
   [06-principios-de-diseno.md](06-principios-de-diseno.md) — evita
   sobre-diseñar cosas que todavía no hacen falta.

## Documentos base

| Doc | Contenido |
|---|---|
| [01-identidad-de-marca.md](01-identidad-de-marca.md) | Quién es CEAC, tono de marca, referencias de estilo |
| [02-tokens-de-diseno.md](02-tokens-de-diseno.md) | Colores, tipografía y medidas (fuente única de verdad) |
| [tokens.css](tokens.css) | Los mismos tokens, en CSS listo para usar en código |
| [03-mapa-del-sitio.md](03-mapa-del-sitio.md) | Páginas del sitio y objetivo de cada una |
| [04-layout-compartido.md](04-layout-compartido.md) | Header y footer, iguales en todas las páginas |
| [05-versiones-del-diseno.md](05-versiones-del-diseno.md) | Registro de las versiones v1 a v7 del `.pen` y qué contiene cada una |
| [06-principios-de-diseno.md](06-principios-de-diseno.md) | Checklist de diseño moderno + qué evitar |

## Estado actual del diseño (2026-09-29)

**La versión vigente es la v7.** En la rama `main`, `ceac-modern.pen`
contiene solo sus páginas (nombres `CEAC v7 - …`), en desktop y mobile.
Las versiones v1 a v6 y los bocetos anteriores (`CEAC Home Modern`, `CEAC
Actual`, `CEAC HomePage`, `About us seccion`, `CEAC — Inicio`) se
conservan en la rama `historial-versiones`.

Qué hay en cada versión, qué se decidió y qué falta:
[05-versiones-del-diseno.md](05-versiones-del-diseno.md).

## Páginas de la v7

| Página | Objetivo |
|---|---|
| [inicio.md](paginas/inicio.md) | Presentar el centro de un vistazo y dirigir a proyectos, servicios, laboratorio y contacto |
| [proyectos.md](paginas/proyectos.md) | Mostrar los proyectos por categoría, con su estado y su ficha |
| [servicios.md](paginas/servicios.md) | Presentar los servicios científicos y estatales y cómo solicitarlos |
| [laboratorio.md](paginas/laboratorio.md) | Presentar los ensayos acreditados del laboratorio y cómo solicitarlos |
| [investigacion.md](paginas/investigacion.md) | Líneas de investigación, investigadores y artículos científicos |
| [docencia.md](paginas/docencia.md) | Diplomados y cursos de posgrado |
| [noticias.md](paginas/noticias.md) | Resultados, eventos y actividades del centro |
| [nosotros.md](paginas/nosotros.md) | Historia, misión, dirección, fundadores y reconocimientos |
| [contacto.md](paginas/contacto.md) | Formulario de consulta, datos de contacto y ubicación |

## Regla de oro

Si mientras diseñás aparece un color, fuente o medida nueva: se agrega
**primero** en [02-tokens-de-diseno.md](02-tokens-de-diseno.md) y **después**
se usa en la página. Nunca al revés.

## Próximo paso sugerido

Cargar el contenido real que falta (ver pendientes en
[05-versiones-del-diseno.md](05-versiones-del-diseno.md)) y, antes de
pasar a código, convertir header, footer, botones y tarjetas en
componentes reutilizables de Pencil.
