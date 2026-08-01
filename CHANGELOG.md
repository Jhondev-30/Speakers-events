# Changelog

Todos los cambios notables a este proyecto serán documentados acá.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
y este proyecto adhiere a [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] — 2026-07-31

### Added
- Catálogo inicial con 120+ sitios curados
- 12 speakers profile cards con monograma, nicho y bio
- Sistema de 4 badges por sitio: tipo, costo, probabilidad de pago, fit
- Sección dedicada "★ Más probables de pago" con 15 sitios top
- Sección "Cómo leer este catálogo" con legend de badges
- Tabla editorial de top picks por speaker
- Hero cinematográfico con imagen de conference hall
- Marquee horizontal de sitios top
- Responsive mobile-first
- 138 external links a páginas reales
- Footer con 4 columnas (brand, speakers, categorías, recursos)

### Design
- Paleta earth tones (charcoal-green + antique gold + warm cream)
- Tipografía: Fraunces (display) + Inter (body) + JetBrains Mono (labels)
- Scroll animations con Intersection Observer
- Hover lift effects en cards
- Reveal staggered en grids

### Tech
- HTML5 semántico single file
- CSS3 con custom properties
- Vanilla JS (sin frameworks, sin build step)
- Google Fonts via CDN
- Deploy vía `mavis website_deploy` (space.minimax.io)

## [v7.0] - 2026-08-01 - Modal expandible con flujo de cada sitio

### Agregado
- **Botón +Info** en cada cat-card (esquina superior derecha) — click abre modal detallado
- **Modal con 5 secciones**: Tipo de acceso / Cómo funciona / Paso a paso / Tips / Fit con nuestros speakers
- **8 templates de flujo** segun tipo de sitio:
  - cfp-open: Sessionize, Papercall, etc (cualquier speaker aplica)
  - cfp-curated: Web Summit, FinCon (invitacion, competitivo)
  - directory: AAS, WomenSpeakers (auto-listing)
  - agency: BigSpeak, Premiere (application + screening)
  - podcast-match: PodMatch, PodMeUp (auto-apply)
  - podcast-pitch: PodPitch, Interview Valet (asistido)
  - community: Meetup, Rotary, Eventbrite (outreach directo)
  - database: Rephonic, ListenNotes (research tools)
  - newsletter: Famesoup, Spreaker (leads pasivos)

### Clasificacion automatica
- 18 cfp-open
- 12 cfp-curated
- 6 directory
- 4 podcast-match
- 7 podcast-pitch
- 76 community (incluye conferencias con CFP anual)
- 2 database

### Archivos
- index.html (231 KB) - 125 cat-cards con data-flow + modal + handlers

