---
name: AEDA
description: Landing institucional de la Asociación de Economía para el Desarrollo de la Argentina
colors:
  brand: "#007FBB"
  brand-dark: "#005C89"
  brand-light: "#7FC4E3"
  navy: "#0A3D5C"
  navy-ink: "#CFE3EE"
  hero-bg: "#071019"
  ink: "#17222A"
  ink-strong: "#0F1B22"
  ink-soft: "#4A5459"
  ink-faint: "#667079"
  muted: "#8C9599"
  border: "#E7E6E1"
  input-border: "#D8DCDD"
  bg: "#FAFAF8"
  bg-alt: "#F1F0EA"
  white: "#FFFFFF"
  success: "#1E8E5A"
  error: "#C4402B"
  footer-muted: "#92A3AB"
typography:
  display:
    fontFamily: "Libre Baskerville, Georgia, 'Times New Roman', serif"
    fontWeight: 700
    lineHeight: 1.2
  body:
    fontFamily: "Lato, system-ui, -apple-system, 'Segoe UI', sans-serif"
    fontWeight: 400
    lineHeight: 1.65
rounded:
  sm: "3px"
  full: "50%"
spacing:
  section-y-desktop: "96px"
  section-y-mobile: "24px"
  card-gap: "28px"
components:
  button-primary:
    backgroundColor: "{colors.brand}"
    textColor: "{colors.white}"
    rounded: "{rounded.sm}"
    padding: "11px 22px"
  button-primary-hover:
    backgroundColor: "{colors.brand-dark}"
  button-outline-on-navy:
    backgroundColor: "{colors.bg}"
    textColor: "{colors.navy}"
    rounded: "{rounded.sm}"
    padding: "14px 26px"
---

# Design System: AEDA

## Overview

**Creative North Star: "El Sello Institucional"**

AEDA es una asociación civil de política económica, no una startup — el sistema visual tiene que leerse como una institución acreditada, no como un producto SaaS. Todo el diseño gira alrededor de una idea central: el isologo de AEDA (la bandera azul recortada detrás de la "e") funciona como un **sello**, y ese mismo gesto —una marca circular con peso— se repite deliberadamente en cada foto de persona, cada ícono de pilar, y el badge de la sección de contacto. No es decoración: es la firma visual del sitio.

La paleta es contenida a propósito: un fondo papel casi blanco, un azul de marca que aparece con moderación, y un navy oscuro reservado para un único quiebre visual (la sección SURi). La tipografía combina un serif editorial (Libre Baskerville) para títulos con un sans-serif neutro (Lato) para el cuerpo — la misma combinación que ya usaba el sitio anterior de AEDA, mantenida a propósito por continuidad de marca, no por default.

Rechazos confirmados: sin gradientes, sin sombras decorativas fuera de los dos casos ya establecidos (el sello circular de contacto y el hover-lift de las tarjetas), sin más de un acento de color por pantalla.

**Key Characteristics:**
- Paleta contenida: un azul de marca, un navy de quiebre, neutros papel/tinta
- El círculo como firma visual recurrente (logos, fotos, sellos)
- Serif editorial + sans neutro, sin una tercera familia tipográfica
- Radios chicos y consistentes (3px) en todo lo rectangular
- Plano por defecto; la sombra aparece solo como respuesta a estado

## Colors

Paleta contenida y con propósito: un acento, un quiebre navy, y neutros papel/tinta que hacen todo el trabajo pesado de jerarquía.

### Primary
- **Azul Confianza Institucional** (#007FBB): el acento de marca — CTA "Contacto", links, la bandera del isologo, el borde de foco. Aparece con moderación; nunca cubre una sección entera.
- **Azul Confianza (hover)** (#005C89): estado hover/activo del acento — siempre más oscuro, nunca un color distinto.
- **Celeste sobre Navy** (#7FC4E3): la misma familia de azul, aclarada para funcionar como eyebrow/etiqueta sobre el fondo navy oscuro (hero, sección SURi).

### Secondary
- **Navy SURi** (#0A3D5C): el único quiebre de fondo oscuro del sitio, reservado para la sección del programa SURi — marca ese bloque como el punto emocional más alto de la página.
- **Celeste Pálido sobre Navy** (#CFE3EE): cuerpo de texto legible sobre el navy, sin llegar al blanco puro.
- **Negro Azulado del Hero** (#071019): fondo de respaldo del hero detrás del video/poster.

### Neutral
- **Papel Institucional** (#FAFAF8): fondo base de toda la página.
- **Beige Contacto** (#F1F0EA): el único fondo alternativo, reservado para la sección de contacto — la separa visualmente sin romper la paleta.
- **Tinta Institucional** (#17222A): texto de cuerpo por defecto.
- **Tinta Fuerte** (#0F1B22): títulos y superficies oscuras (footer).
- **Tinta Suave** (#4A5459): texto secundario (descripciones de pilares, intro de contacto).
- **Tinta Tenue** (#667079): etiquetas terciarias (rol de autoridades — "Presidente"/"Tesorero").
- **Gris Placeholder** (#8C9599): placeholders de formulario.
- **Borde Papel** (#E7E6E1) / **Borde de Formulario** (#D8DCDD): divisores y bordes de input.
- **Gris Footer** (#92A3AB): copyright sobre el footer oscuro — deliberadamente más claro que el body text del footer para pasar AA sobre `#0F1B22`.
- **Verde Confirmación** (#1E8E5A) / **Rojo Error** (#C4402B): estados del formulario de contacto únicamente.

### Named Rules
**La Regla del Acento Único.** El azul de marca aparece en un solo elemento interactivo por vista (el CTA activo, o el link que se está mirando). Nunca dos acentos compitiendo en la misma sección.

## Typography

**Display Font:** Libre Baskerville (con Georgia, "Times New Roman", serif de respaldo)
**Body Font:** Lato (con system-ui, sans-serif de respaldo)

**Character:** un serif editorial de peso institucional para todo lo que sea título, contra un sans-serif neutro y muy legible para el cuerpo — la misma combinación heredada del sitio anterior de AEDA, mantenida por continuidad de marca.

### Hierarchy
- **Display** (700, 52px hero / 30-32px de sección, 1.18–1.25 line-height): headline del hero y títulos "AEDA impulsa SURi…" — el único lugar donde el serif se usa a gran escala.
- **Headline** (700, 30px, Libre Baskerville): títulos de sección ("Nuestras acciones…", "Autoridades AEDA", "Contacto con AEDA").
- **Title** (700, 18-19px): nombre de autoridad, título de pilar — serif también, más chico.
- **Body** (400, 15-16px, Lato, 1.65-1.7 line-height): todo el texto corrido.
- **Label** (600-700, 12.5-13px, uppercase, letter-spacing 0.06-0.12em, Lato): eyebrows, roles de autoridades, etiquetas de registros.

### Named Rules
**La Regla Serif-Solo-En-Títulos.** Libre Baskerville nunca aparece en párrafos de cuerpo ni en controles de formulario — el serif es exclusivamente para jerarquía, el sans-serif hace todo el trabajo de lectura.

## Layout

**(2026-08-27 — pivot a lenguaje orgánico, ver nota al final de esta sección).** Página de una sola sección larga (sin routing), contenida en un `.wrap` de `max-width: 1440px` centrado. Padding vertical de sección generoso en desktop (88-150px) que se comprime a 24px horizontal en mobile (`≤900px`, único breakpoint del sitio). El header es sticky (`top: 0`) en todo momento, incluido el panel de navegación mobile que vive dentro del mismo elemento sticky.

Las secciones ya no se cortan en ángulo recto entre sí: cada transición de sección usa un `.wave-divider` (SVG de curva orgánica, `fill` igual al color de la sección siguiente) en vez de un borde de 90°. Acciones, SURi, Autoridades y Registros viven dentro de un `.organic-flow` (contenedor `position: relative`) con 2-3 `.blob` (círculos `filter: blur()`, opacidad baja, tonos de marca/navy, animación de flotación lenta gateada por `prefers-reduced-motion`) que conectan visualmente esas secciones. Las grillas dejaron de ser simétricas a propósito: pilares usa 3 columnas de ancho desigual con stagger vertical (`margin-top` alternado), autoridades escalona su segunda tarjeta, y registros pasó de grid+`border-top` a chips en `flex-wrap`.

## Elevation & Depth

**(Actualizado — ya no aplica "Plano por defecto").** El pivot a glassmorphism introdujo sombra y profundidad como recurso estructural, no solo de estado. Las superficies "flotantes" (tarjetas de pilares/autoridades, panel de SURi, panel de contacto) usan `--shadow-glass` / `--shadow-glass-lift` en reposo — ya no es una excepción rara, es el lenguaje del sitio. El hover-lift de autoridades y el sello de contacto se mantienen sin cambios.

### Shadow Vocabulary
- **Sello flotante** (`var(--shadow-seal)`): el badge circular de "Contacto con AEDA" y los avatares que rompen el borde de sus tarjetas.
- **Glass** (`var(--shadow-glass)` / `var(--shadow-glass-lift)`): todas las superficies de vidrio (tarjetas, paneles) en reposo.
- **Hover-lift** (`box-shadow: 0 16px 32px -14px rgba(15, 23, 42, 0.28)`): sin cambios, se mantiene sobre el hover-lift existente.

### Named Rules
**La Regla Plano-Por-Defecto queda derogada por el pivot orgánico (2026-08-27).** La sombra ahora es parte del lenguaje de superficie (glass), no solo respuesta a interacción. Se mantiene, eso sí, la disciplina de no usar sombras puramente decorativas sin una superficie de vidrio real detrás.

## Shapes

**(Actualizado)** Tres escalas de radio conviviendo con una regla documentada (no es un radio único, pero cada uno tiene un rol fijo):
- **Círculo** (`border-radius: 50%`): reservado para fotos y marcas, sin cambios respecto al criterio original.
- **`--radius-lg` (24px):** tarjetas y paneles de vidrio (pilares, autoridades, SURi, contacto).
- **`--radius-md` (14px):** inputs de formulario.
- **`--radius-pill` (999px):** botones y CTA (antes 3px) — el pill ahora es el default de botón, no la excepción del nav.

## Components

### Buttons
- **Shape:** `--radius-pill` (999px) en todos los botones (primary, outline-on-navy, submit, nav CTA) — ya no hay radio chico de 3px en botones.
- **Primary (sobre fondo claro):** fondo `--color-brand`, texto blanco, hover a `--color-brand-dark`.
- **Outline sobre navy:** fondo `--color-bg` (papel), texto navy, hover invierte a fondo transparente + texto papel — usado para "Conocé más sobre SURi" sobre el navy.
- **Hover / Focus:** el ícono de flecha del botón se desplaza `translateX(3px)` en 0.2s, gateado detrás de `prefers-reduced-motion: no-preference`.

### Cards / Containers (glassmorphism)
- **Corner Style:** `--radius-lg` (24px) en todas las tarjetas y paneles.
- **Background:** `--glass-light-bg` (blanco 66% + `backdrop-filter: blur(20px)`) sobre fondo claro, `--glass-navy-bg` sobre el navy de SURi.
- **Shadow Strategy:** `--shadow-glass` en reposo (ver Elevation).
- **Overlap:** las fotos/avatares y el sello de contacto rompen deliberadamente el borde superior de su tarjeta (`position: absolute` + offset negativo) — es el gesto de "objeto que se posa sobre la superficie", ahora extendido de "solo el sello" a todo retrato en tarjeta.
- **Fallback:** bajo `prefers-reduced-transparency: reduce`, el vidrio cae a fondo sólido sin blur (ver `:root` y cada bloque `.pilar-card`/`.autoridad`/`.contacto-panel`/`.suri-panel`).
- **Internal Padding:** 26-44px según componente.

### Inputs / Fields
- **Style:** fondo blanco, borde 1px `--color-input-border`, radio `--radius-md` (14px, antes 3px), padding 13-16px.
- **Focus:** contorno de 2px en `--color-brand` con 2px de offset (mismo tratamiento que los links).
- **Error / Disabled:** no hay estado de error por campo individual; el formulario reporta éxito/error a nivel de envío completo (`.form-status`, verde `--color-success` / rojo `--color-error`).

### Navigation
- Header sticky con fondo de vidrio (`--glass-light-bg` + `backdrop-filter: blur(20px)`), sin borde inferior duro (reemplazado por una sombra suave). Links en Lato 600, 14.5px. El CTA "Contacto" es un pill de color (antes radio 3px). En mobile (`≤900px`) el nav de texto desaparece y un botón hamburguesa (44×44px, dentro del mismo header sticky) despliega un panel vertical con los mismos 5 links a ancho completo, con las esquinas inferiores redondeadas — nunca un menú separado ni un overlay aparte.

### Section Dividers (`.wave-divider`)
Curva SVG de ancho completo entre secciones de distinto color de fondo (hero→acciones, acciones→SURi, SURi→autoridades, registros→contacto, contacto→footer). El `fill` del path siempre coincide con el color de la sección que sigue. Reemplaza el corte recto de 90° que tenía el sitio original.

### Organic Blobs (`.blob`, `.suri::before/::after`, `.contacto::before`)
Círculos `filter: blur(60-80px)`, opacidad 0.16-0.32, en tonos de la rampa de marca/navy ya definida en `.impeccable/design.json`. Animación `blob-float` (traslación + escala sutil, 22-32s, `ease-in-out infinite alternate`) gateada por `prefers-reduced-motion: no-preference`; ocultos bajo `prefers-reduced-transparency: reduce`. Sirven para conectar visualmente secciones del mismo tono (acciones/autoridades/registros) y para dar profundidad a los bloques navy (SURi) y beige (contacto).

### El Sello Circular (componente de firma)
El mismo patrón —un círculo con foto o logo dentro— se repite en cinco lugares del sitio: el isologo del header (46px), el isologo blanco del hero (56px de alto), las fotos de pilares (96px, ahora rompiendo el borde superior de su tarjeta) y autoridades (108px, ídem — ver "Grilla de equipo" abajo), y el sello blanco con sombra de la sección de contacto (108px, ahora también rompiendo el borde del panel de vidrio). Con el pivot orgánico este gesto de "romper el borde" pasó de ser exclusivo del sello de contacto a ser el tratamiento estándar de todo retrato/marca en tarjeta.

### Grilla de equipo (Autoridades)
`.autoridades-grid` usa `repeat(auto-fit, minmax(220px, 260px))` en vez de un grid fijo de 2 columnas — con los 2 integrantes actuales deja espacio asimétrico a la derecha a propósito; si se suma un tercer o cuarto integrante, la grilla reflowea sola sin tocar CSS. Cada tarjeta es vertical y centrada: foto circular de 108px rompiendo el borde superior, nombre, rol, y el link de LinkedIn como pill (antes texto plano) para que se lea como tarjeta de equipo, no como fila de datos.

### Hero blobs y sección "Colabora"
El hero ahora tiene 2 `.hero-blob` (mismo lenguaje que `.blob`, z-index entre el video y el degradado oscuro) para que la apertura del sitio ya sea orgánica y no dependa solo del wave-divider de cierre. Se agregó una sección nueva, `#colabora`, entre Registros y Contacto: un panel de vidrio alineado a la derecha (asimetría deliberada, en espejo con el panel de SURi que va a la izquierda) sobre dos blobs propios, con un único CTA ("Quiero colaborar" → `#contacto`) — sin eyebrow, porque ya se llegó al máximo de 3 eyebrows permitidos en el resto del sitio.

### Corrección de contraste (2026-08-27)
Los botones de texto blanco sobre `--color-brand` (nav CTA, submit del formulario, y por herencia el nuevo botón de "Colabora") medían 4.42:1 — por debajo del mínimo AA de 4.5:1 para texto normal. Se corrigieron a `--color-brand-dark` en reposo y `--color-navy` en hover (7.26:1), sin agregar ningún color nuevo al sistema.

## Do's and Don'ts

### Do:
- **Do** usar `var(--color-*)` para cualquier color nuevo — nunca un hex literal nuevo sin agregarlo primero al `:root`.
- **Do** mantener el círculo (`border-radius: 50%`) reservado para fotos y marcas; `--radius-lg` para tarjetas/paneles, `--radius-md` para inputs, `--radius-pill` para botones.
- **Do** gatear cualquier animación/transición nueva (incluidos los `.blob`) detrás de `@media (prefers-reduced-motion: no-preference)`, siguiendo el patrón ya establecido.
- **Do** proveer fallback sólido sin blur bajo `prefers-reduced-transparency: reduce` para cualquier superficie de vidrio nueva.
- **Do** mantener Libre Baskerville exclusivamente en títulos; el cuerpo siempre en Lato.

### Don't:
- **Don't** introducir una tercera familia tipográfica (ni siquiera para un detalle chico como un label o un mono de datos).
- **Don't** usar el azul de marca en más de un elemento interactivo por vista — diluye la Regla del Acento Único.
- **Don't** cargar el video del hero fuera de la condición actual (desktop + sin `prefers-reduced-motion`) — es una decisión de accesibilidad y performance, no un descuido.
- **Don't** volver a un corte recto de 90° entre secciones de distinto fondo — usar `.wave-divider`.
- **Don't** mezclar radios fuera de la escala documentada (círculo / 24px / 14px / pill).
