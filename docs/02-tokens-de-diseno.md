# 2. Tokens de diseño

Definidos **una sola vez** acá; ninguna página crea colores o medidas
propias, todas consumen estos tokens. Ver la regla de oro en el
[índice](00-indice.md).

> **Fuente:** esta tabla ya no es solo la plantilla teórica — está
> verificada contra el boceto real `CEAC Home Modern` dentro de
> `ceac-modern.pen` (el frame que sí respeta la identidad de marca; ver nota
> de diagnóstico en [`00-indice.md`](00-indice.md#nota-de-diseño-actual)).
> Versión ejecutable en código: [`tokens.css`](tokens.css).

## Colores — resumen semántico

> **Actualización (2026-09-25):** la primera pasada de tokens quedó
> fiel al boceto pero demasiado apagada — el texto usaba azules muy
> desaturados (grises azulados) en vez de leerse como marca. Se subió la
> saturación de `ink-500`/`ink-400` manteniendo el mismo hue (~206°) y la
> misma luminosidad (para no romper el contraste/jerarquía ya definido), y
> se agregaron variantes "bright" para elementos interactivos (links,
> CTAs de tarjeta). `color-primary` y `color-accent` no se tocaron: ya
> estaban bien saturados (90% y 70%) y son el ancla de marca — no hay que
> alejarse de esos dos.

| Token | Uso | Claro | Oscuro |
|---|---|---|---|
| `color-primary` | Marca / acciones principales, botones grandes, logo | `#0A6FCC` (azul institucional — sin cambios) | `#4C9EE0` (propuesto, sin validar visualmente) |
| `color-primary-bright` | Links y CTA de texto ("Ver más →", "Leer más") | `#007AEB` (mismo hue, saturación al 100%) | — |
| `color-accent` | Acento ambiental / logos de colaboradores | `#1EA84A` (verde — sin cambios) — variante `#1A9D61` | igual, ajustando luminosidad si hace falta |
| `color-accent-bright` | Hover / highlight sobre elementos verdes | `#11D04E` | — |
| `color-background` | Fondo general | `#FFFFFF` (o `#F4FAFC` para fondos suaves) | `#0A1F33` (propuesto) |
| `color-heading` | Títulos y texto de mayor jerarquía | `#083B66` (navy oscuro — sin cambios) | `#EAF4FF` (propuesto) |
| `color-body` | Cuerpo de texto sobre fondo claro | `#2A6FA6` (antes `#4D6C83`, muy desaturado) | `#B9CBDA` (propuesto) |
| `color-muted` | Texto secundario / descripciones cortas | `#5E9AC9` (antes `#7A97AE`) | `#8CA3B8` (propuesto) |
| `color-border` | Bordes y separadores | `#D2E3EF` (sombras suaves `#0A35520D`) | `#1E4E71` (propuesto) |
| `color-on-brand` | Texto sobre fondos de color/oscuros (Hero, LEA, Investigación) | `#FFFFFF` | — |
| `color-on-brand-muted` | Texto secundario sobre esos mismos fondos | `#D9EEFF` | — |

*(Los valores "oscuro" marcados **propuesto** son un punto de partida
calculado, no vienen del boceto — en el `.pen` el modo oscuro todavía no
está decidido, ver checklist en
[06-principios-de-diseno.md](06-principios-de-diseno.md). No dar por
buenos hasta validarlos visualmente.)*

## Escala de azules (navy) — detalle

`CEAC Home Modern` no usa un solo gris para el texto: usa **variaciones de
azul marca** para dar jerarquía, lo cual es más distintivo que un gris
neutro y es justamente lo que le falta al frame genérico. Escala normalizada
(de más oscuro a más claro):

| Paso | Hex | S / L | Uso observado en el boceto |
|---|---|---|---|
| `ink-900` | `#083B66` | S86% L22% | Wordmark "CEAC", títulos de sección grandes ("Proyectos", "Noticias", "Mapa de Cienfuegos") |
| `ink-800` | `#0B4A73` | S83% L25% | Nav activo, cifras de stats, títulos de tarjeta |
| `ink-700` | `#104E7F` | S78% L28% | Labels de stats ("Proyectos", "Investigadores") |
| `ink-600` | `#185C92` | S72% L33% | Nav inactivo |
| `ink-500` | `#2A6FA6` | S60% L41% | Cuerpo de texto, descripciones, bajadas |
| `ink-400` | `#5E9AC9` | S50% L58% | Texto secundario más liviano |
| `ink-100` | `#D2E3EF` / `#BED7EA` | — | Bordes suaves, paneles |
| `ink-50` | `#F4FAFC` / `#F7FBFF` | — | Fondo general |

*(`ink-700`/`ink-600` son los tonos intermedios del sistema — en los
frames vigentes del `.pen` no se usan todavía, pero quedan definidos acá
para header/nav u otros estados que los necesiten después.)*

**Regla práctica:** si estás por escribir texto y dudás qué azul usar,
elegí por jerarquía (título → `ink-900/800`, cuerpo → `ink-500`, secundario
→ `ink-400`) en vez de inventar un hex nuevo.

## Tipografía

| Token | Fuente | Uso |
|---|---|---|
| `font-display` | Funnel Sans | Wordmark "CEAC", títulos de sección y de tarjeta |
| `font-body` | Geist | Cuerpo de texto general, nav, botones |
| `font-label` | IBM Plex Mono | Eyebrows, fechas, siglas de colaboradores (mayúsculas, tipo dato técnico) |
| `font-accent` *(opcional)* | Staccato222 BT | Frase decorativa tipo firma (tagline "...un puente al desarrollo sostenible") — un solo lugar en el sitio (Hero) |

**Importante:** el boceto `CEAC HomePage` (el genérico) usa **Inter** en
casi todo el texto — no es un token válido, es justamente parte de lo que
lo hace ver genérico. No reusar esa fuente al implementar.

## Escala tipográfica (tamaños)

Basada en los tamaños reales del boceto, prolijada a una progresión
coherente:

| Token | Valor | Uso |
|---|---|---|
| `text-xs` | 12px | Labels, fechas, siglas |
| `text-sm` | 13–14px | Texto secundario pequeño |
| `text-base` | 15px | Cuerpo / nav / botones |
| `text-md` | 18px | Bajadas de sección |
| `text-lg` | 20px | Cifras pequeñas (badges) |
| `text-xl` | 24–28px | Subtítulos |
| `text-2xl` | 30–36px | Títulos de tarjeta, stats grandes |
| `text-3xl` | 50–54px | Títulos de sección |
| `text-4xl` | 62–64px | Títulos de sección hero-like |

## Medidas

| Token | Valor |
|---|---|
| `radius-sm` | 4px |
| `radius-md` | 8px |
| `radius-lg` | 16px |
| `radius-pill` | 9999px (badges / tags de estado, ej. "Activo") |

*(El boceto genérico usa 4/12/16/24 sin patrón claro — al implementar,
usar solo estos 4 tokens, no valores sueltos.)*

## Regla

Si un color o medida nuevo aparece mientras diseñás, se agrega **acá
primero**, después se usa en las páginas — nunca al revés.
