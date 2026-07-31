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
