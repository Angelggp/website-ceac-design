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
| [06-principios-de-diseno.md](06-principios-de-diseno.md) | Checklist de diseño moderno + qué evitar |

## Nota de diseño actual (2026-09-25)

`ceac-modern.pen` tiene varios frames históricos y uno activo:

- **`CEAC — Inicio`** ✅ **el activo/canónico ahora.** Es un refacto
  completo de `CEAC Home Modern` (que ya tenía las mejores bases: hero con
  gradiente diagonal azul→verde, panel flotante con badge "+27 años",
  bandas de color alternadas). Se le sumó:
  - Sección nueva **"Qué hacemos"** (grid de 4 tarjetas con ícono —
    Proyectos / Servicios-LEA / Investigación / Docencia) entre el Hero y
    Proyectos, para dar un resumen navegable apenas se entra.
  - Íconos (`lucide`: droplet / mountain / wind) en las 3 tarjetas de
    servicios del LEA.
  - Footer ampliado con **Enlaces rápidos** y **Síguenos**, que antes
    faltaban (los pedía [04-layout-compartido.md](04-layout-compartido.md)).
  - Paleta re-brillada igual que el resto (ver
    [02-tokens-de-diseno.md](02-tokens-de-diseno.md)) — este frame nunca
    había recibido ese ajuste.
- **`CEAC Home Modern`**, **`CEAC Actual`**, **`CEAC HomePage`** —
  deshabilitados, quedan como historial/referencia. `CEAC HomePage` fue el
  que arrancó con paleta genérica de SaaS (Inter, azul `#0066FF`) — ya no
  es el que se usa.
- **`About us seccion`** — sin tocar en este refacto (solo Header+Footer,
  pendiente de contenido real; ver [paginas/nosotros.md](paginas/nosotros.md)).

**Estado:** `CEAC — Inicio` consume los tokens de [tokens.css](tokens.css)
en su totalidad. Falta la revisión visual manual en Pencil/VSCode — esto
se construyó por edición directa del JSON (clonando y editando el árbol de
nodos), no de forma interactiva.

## Páginas (plantilla atómica completada)

| Página | Objetivo |
|---|---|
| [inicio.md](paginas/inicio.md) | Presentar el centro de un vistazo y dirigir a proyectos, servicios y contacto |
| [nosotros.md](paginas/nosotros.md) | Comunicar misión, historia (+26 años) y equipo |
| [proyectos.md](paginas/proyectos.md) | Mostrar proyectos de investigación aplicada, con estado y resultados |
| [servicios-laboratorio.md](paginas/servicios-laboratorio.md) | Detallar los servicios técnicos del LEA (ensayos de agua, suelos, ruido/aire) |
| [investigacion.md](paginas/investigacion.md) | Comunicar líneas de investigación y publicaciones científicas |
| [docencia.md](paginas/docencia.md) *(opcional)* | Programas de formación continua para profesionales del sector |
| [noticias.md](paginas/noticias.md) | Actualizaciones sobre proyectos, foros y colaboraciones |
| [contacto.md](paginas/contacto.md) | Formulario de consulta, datos de contacto y ubicación |

## Regla de oro

Si mientras diseñás aparece un color, fuente o medida nueva: se agrega
**primero** en [02-tokens-de-diseno.md](02-tokens-de-diseno.md) y **después**
se usa en la página. Nunca al revés.

## Próximo paso sugerido

Con estos documentos ya se puede pasar a construir un sistema de diseño
reutilizable (paleta, tipografía y espaciados como base compartida, por
ejemplo en Penpot/`ceac-modern.pen` o en CSS/tokens de código) y de ahí a
maquetar pantallas reales, apoyándose en la skill **frontend-design** para
las decisiones de estética e interfaz.
