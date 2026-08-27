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
    backgroundColor: "{colors.brand-dark}"
    textColor: "{colors.white}"
    rounded: "{rounded.sm}"
    padding: "11px 22px"
  button-primary-hover:
    backgroundColor: "{colors.navy}"
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

Rechazos confirmados: sin gradientes, sin glassmorphism, sin sombras decorativas fuera de los dos casos ya establecidos (el sello circular de contacto y el hover-lift de las tarjetas), sin más de un acento de color por pantalla.

**Key Characteristics:**
- Paleta contenida: un azul de marca, un navy de quiebre, neutros papel/tinta
- El círculo como firma visual recurrente (logos, fotos, sellos, y ahora también como acento de fondo entre secciones)
- Serif editorial + sans neutro, sin una tercera familia tipográfica
- Radios chicos y consistentes (3px botones/inputs, 4px tarjetas) en todo lo rectangular
- Plano por defecto; la sombra aparece solo como respuesta a estado

### Nota de reversión (2026-08-27)
El sitio pasó brevemente por un pivot "orgánico" (glassmorphism, blobs difuminados animados, curvas SVG entre secciones, radios grandes tipo pill) que se revirtió el mismo día tras recibir un handoff de diseño de alta fidelidad (`design_handoff_landing_aeda/`) que confirmaba la dirección sobria/institucional original como la vigente. Este documento y `index.html` reflejan esa reversión: **el lenguaje "plano" descrito abajo es el estado real del sitio**, no un borrador histórico. La única herencia que sí se conservó del pivot orgánico fue la corrección de contraste de los botones (ver Components → Buttons) y la incorporación de acentos circulares de fondo entre secciones (ver Layout), ambos compatibles con el lenguaje plano.

## Colors

Paleta contenida y con propósito: un acento, un quiebre navy, y neutros papel/tinta que hacen todo el trabajo pesado de jerarquía.

### Primary
- **Azul Confianza Institucional** (#007FBB): el acento de marca — links, la bandera del isologo, el borde de foco, las etiquetas de registros. Aparece con moderación; nunca cubre una sección entera.
- **Azul Confianza (hover)** (#005C89): estado de reposo de los botones de texto blanco (ver Corrección de contraste) y estado hover/activo del acento en general — siempre más oscuro, nunca un color distinto.
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

Página de una sola sección larga (sin routing), contenida en un `.wrap` de `max-width: 1440px` centrado, con `overflow: hidden` (necesario para recortar los acentos circulares de fondo que asoman por los bordes — ver abajo). Padding vertical de sección generoso en desktop (88-150px) que se comprime a 24px horizontal en mobile (`≤900px`, único breakpoint del sitio). Grillas de 3 columnas (pilares, registros) y 2 columnas (autoridades) colapsan a 1 columna en mobile. El header es sticky (`top: 0`) en todo momento, incluido el panel de navegación mobile que vive dentro del mismo elemento sticky. Las secciones siguen cortándose en ángulo recto entre sí — no hay curvas SVG ni transiciones onduladas.

**Acentos circulares de fondo (`.deco-track` / `.deco-circle`, agregado 2026-08-27):** cinco círculos planos, sin blur ni animación, de 380-560px de diámetro, en `--color-brand`, `--color-brand-light` o `--color-navy` a opacidad muy baja (0.07-0.16), ubicados en los puntos de transición entre secciones (hero→acciones, acciones→SURi, SURi→autoridades, registros→contacto, contacto→footer). Es una extensión discreta del motivo del "sello" a la escala de la página completa — no reemplaza ni introduce blur, sombra o movimiento; se recortan contra el borde del `.wrap` y no requieren gating por `prefers-reduced-motion` porque no animan.

## Elevation & Depth

Plano por defecto. El sitio no usa sombra como recurso decorativo — aparece únicamente como respuesta a estado (hover) o para un elemento verdaderamente flotante (el sello de contacto). No hay glassmorphism ni `backdrop-filter` en ninguna superficie.

### Shadow Vocabulary
- **Sello flotante** (`box-shadow: 0 6px 20px -8px rgba(15, 23, 42, 0.18)`): el badge circular de "Contacto con AEDA" — el único elemento que tiene sombra en reposo, porque es literalmente un objeto que se posa sobre la página.
- **Hover-lift** (`box-shadow: 0 16px 32px -14px rgba(15, 23, 42, 0.28)`): tarjetas de autoridades al pasar el mouse/foco — combinado con `translateY(-5px) scale(1.012)`.

### Named Rules
**La Regla Plano-Por-Defecto.** Ninguna superficie tiene sombra en reposo salvo el sello de contacto. La sombra es siempre una respuesta a interacción, nunca un adorno permanente.

## Shapes

Dos lenguajes de forma conviviendo a propósito: todo lo rectangular (botones, inputs, tarjetas, badges de registro) usa un radio chico y consistente de 3-4px — nunca `rounded-lg` genérico ni pill fuera del CTA de nav. Todo lo que sea retrato o marca (fotos de autoridades, íconos de pilares, isologo del hero/contacto) es un círculo perfecto (`border-radius: 50%`). No hay una forma intermedia; el círculo está reservado para "esto es una persona, una marca, o un acento de fondo", el radio chico para "esto es un control o contenedor".

## Components

### Buttons
- **Shape:** radio de 3px, nunca completamente cuadrado ni pill (excepto el CTA "Contacto" del nav, que sí es un pill funcional por convención de nav — ver nota abajo sobre su radio real).
- **Primary (texto blanco sobre acento):** fondo `--color-brand-dark` en reposo, hover a `--color-navy` (ver Corrección de contraste — no usar `--color-brand` como fondo de texto blanco).
- **Outline sobre navy:** fondo `--color-bg` (papel), texto navy, hover invierte a fondo transparente + texto papel — usado para "Conocé más sobre SURi" sobre el navy.
- **Hover / Focus:** el ícono de flecha del botón se desplaza `translateX(3px)` en 0.2s, gateado detrás de `prefers-reduced-motion: no-preference`.

### Corrección de contraste (heredada, 2026-08-27)
Los botones de texto blanco sobre `--color-brand` (CTA "Contacto" del nav, submit del formulario) medían 4.42:1 — por debajo del mínimo AA de 4.5:1 para texto normal. Se corrigieron a `--color-brand-dark` en reposo y `--color-navy` en hover (7.26:1). Esta corrección se hizo originalmente durante el pivot orgánico pero es independiente de esa estética, así que se conservó al revertir a la dirección plana.

### Cards / Containers
- **Corner Style:** 4px de radio (autoridades) o sin borde (pilares, que usan solo la foto circular + texto).
- **Background:** blanco/papel, borde de 1px `--color-border`.
- **Shadow Strategy:** ninguna en reposo; ver Elevation para el hover-lift de autoridades.
- **Internal Padding:** 26px.

### Inputs / Fields
- **Style:** fondo blanco, borde 1px `--color-input-border`, radio 3px, padding 13-14px.
- **Focus:** contorno de 2px en `--color-brand` con 2px de offset (mismo tratamiento que los links).
- **Error / Disabled:** no hay estado de error por campo individual; el formulario reporta éxito/error a nivel de envío completo (`.form-status`, verde `--color-success` / rojo `--color-error`).

### Navigation
- Header sticky, fondo papel, borde inferior de 1px. Links en Lato 600, 14.5px. El CTA "Contacto" es la única pill de color del nav. En mobile (`≤900px`) el nav de texto desaparece y un botón hamburguesa (44×44px, dentro del mismo header sticky) despliega un panel vertical con los mismos 5 links a ancho completo — nunca un menú separado ni un overlay aparte.

### Skip link (agregado 2026-08-27)
Link "Saltar al contenido" oculto fuera de pantalla (`left: -9999px`), visible al recibir foco (`left: 16px; top: 16px`), fondo `--color-brand`, texto blanco. Primer elemento enfocable después del header, apunta a `#main-content` (el `<main>` ahora lleva ese `id`).

### El Sello Circular (componente de firma)
El mismo patrón —un círculo con foto, logo o color plano dentro— se repite en el sitio: el isologo del header (46px), el isologo blanco del hero (56px de alto), las fotos de pilares y autoridades (140px / 58px), el sello blanco con sombra de la sección de contacto (108px, el único con `box-shadow` en reposo), y ahora también los cinco acentos circulares de fondo entre secciones (ver Layout). Es el elemento que más unifica visualmente el sitio de punta a punta.

## Do's and Don'ts

### Do:
- **Do** usar `var(--color-*)` para cualquier color nuevo — nunca un hex literal nuevo sin agregarlo primero al `:root`.
- **Do** mantener el círculo (`border-radius: 50%`) reservado para fotos, marcas y acentos de fondo; el radio de 3px para todo lo demás.
- **Do** gatear cualquier animación/transición nueva detrás de `@media (prefers-reduced-motion: no-preference)`, siguiendo el patrón ya establecido para scroll-reveal, hover-lift y el ícono del botón de SURi.
- **Do** mantener Libre Baskerville exclusivamente en títulos; el cuerpo siempre en Lato.
- **Do** usar `--color-brand-dark` (nunca `--color-brand`) como fondo de botones con texto blanco, por contraste AA.

### Don't:
- **Don't** agregar una sombra decorativa a un elemento en reposo — la Regla Plano-Por-Defecto solo tiene dos excepciones y ya están documentadas.
- **Don't** introducir una tercera familia tipográfica (ni siquiera para un detalle chico como un label o un mono de datos).
- **Don't** usar el azul de marca en más de un elemento interactivo por vista — diluye la Regla del Acento Único.
- **Don't** cargar el video del hero fuera de la condición actual (desktop + sin `prefers-reduced-motion`) — es una decisión de accesibilidad y performance, no un descuido.
- **Don't** reintroducir glassmorphism, blobs difuminados/animados o curvas SVG entre secciones — fueron probados y revertidos el 2026-08-27; si se reconsidera esa dirección, debe ser una decisión explícita y nueva, no un drift incremental.
