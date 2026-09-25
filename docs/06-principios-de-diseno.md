# 6. Principios de diseño (checklist rápido)

Marcá lo que aplica al proyecto; no diseñes más de lo que hace falta para
arrancar.

- [ ] Responsivo: mobile / tablet / desktop
- [ ] Modo claro y oscuro (¿o solo uno de los dos por ahora?)
- [ ] Accesibilidad básica: contraste suficiente, foco visible en links y
      botones
- [ ] Animación: nivel mínimo viable — fade/scroll-reveal simple en
      secciones y tarjetas, hover sutil en botones. Nada más hasta tener el
      diseño base aprobado.
- [ ] Jerarquía visual clara: un solo elemento "protagonista" por sección,
      no todo compitiendo por atención
- [ ] Whitespace generoso, tipografía legible

## A evitar (salvo que sea parte de la identidad)

- Fondos animados o formas flotando de fondo
- Efectos 3D pesados / WebGL
- Estética que no coincida con el tono definido en
  [01-identidad-de-marca.md](01-identidad-de-marca.md)

## Para mejorar el diseño

Este espacio ya tiene disponible la skill **frontend-design**, pensada
justo para esto: dirección estética, tipografía y decisiones que no se
sientan "genéricas" al construir la interfaz. Se activa sola cuando pasemos
de esta documentación a construir pantallas o componentes reales (mockups,
HTML/React, o directamente en `ceac-modern.pen`) — no hace falta instalar
nada.

## Siguiente paso opcional

Si además se quiere un sistema de diseño reutilizable (paleta, tipografía y
espaciados como base compartida para todas las páginas antes de maquetar),
se arma como próximo paso apoyándose directamente en
[01-identidad-de-marca.md](01-identidad-de-marca.md) y
[02-tokens-de-diseno.md](02-tokens-de-diseno.md).
