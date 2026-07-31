# 🎤 SpeakUp Express — Speaker Resources

> Catálogo curado de 120+ sitios web donde los speakers de **SpeakUp Express** encuentran eventos presenciales, podcasts, summits virtuales, comunidades de organizadores y networking.

[![Status](https://img.shields.io/badge/status-live-c9a14a?style=for-the-badge)](https://x7q9qsvwxzkou.space.minimax.io)
[![Stack](https://img.shields.io/badge/stack-HTML%20%2B%20CSS%20%2B%20JS-6b8e5a?style=for-the-badge)]()
[![License](https://img.shields.io/badge/license-proprietary-c47a5a?style=for-the-badge)]()

🔗 **Live:** https://x7q9qsvwxzkou.space.minimax.io

---

## 📖 Sobre el proyecto

Landing page premium (Awwwards-style) que sirve como **catálogo de discovery + sales enablement** para los 12+ speakers de la red SpeakUp Express. Cada sitio del catálogo viene con 3 señales que permiten decidir dónde aplicar primero:

- **Tipo** — Outbound (speaker aplica) vs Inbound (organizer te busca)
- **Costo** — Free, Freemium, Paid, Full-service
- **Probabilidad de pago** — $$$ Alto, $$ Medio, Exposure, Ticket only

### Speakers cubiertos (12)

| Speaker | Nicho principal | Fit destacado |
|---|---|---|
| **Angie Pichardo** | Faith · Suicide/NDE Survivor | AAS, WomenSpeakers, AAS Stipend |
| **Dr. Phillip Meade** | Senior Pastor · Leadership | Premiere Bureau ($$$ Alto) |
| **Patricio Larrea** | Growth · LATAM | Web Summit, Digital Summit |
| **Angelie Kapoor** | Faith · Christian Women | Crowned, Listen To Her |
| **Kimberly Aschman** | Real Estate · Business | Florida Realtors, WCR, InvestHER |
| **Kelly White** | Career · Reinvention | WLS 2026, Women of Pavilion |
| **Philip Chan** | Multi-Exit · Finance | Web Summit, Mastermind Talks |
| **Russ Katzman** | Leadership · Enterprise | Talks at GS ($$$ Alto) |
| **Jeff Forrester** | Faith · Leadership | Church Conf List, Small Church Min. |
| **Evelena Dawson** | Affirmed Women | WomenSpeakers, Crowned |
| **Alex Berman** | Sales · Author | Premiere Bureau, Dreamforce |
| **Rachel Scheer** | Wellness · Nutrition | Wellness Show, Integrative Healthcare |

---

## ✨ Features

- **120+ sitios curados** en 7 categorías (CFP, Directories, Podcasts, Summits, Comunidades, Networking, Virtual Coffee)
- **Sección dedicada** "★ Más probables de pago" — 15 sitios top con fee estimado
- **138 external links** directos a las páginas de cada sitio
- **Responsive** mobile-first
- **Sin frameworks** — HTML + CSS + JS vanilla
- **Accesibilidad** básica (semantic HTML, focus states, alt text donde corresponde)

---

## 🎨 Design system

| Token | Valor | Uso |
|---|---|---|
| `--ink-900` | `#0d1410` | Background principal |
| `--paper-50` | `#f6efde` | Texto principal |
| `--gold-500` | `#c9a14a` | Acentos, números, CTAs |
| `--copper-500` | `#b87333` | Degradados, hovers |
| `--terracotta` | `#c47a5a` | Badges, alerts |
| `--sage` | `#6b8e5a` | Inbound, free |

**Tipografía:** Fraunces (display, editorial serif) + Inter (body) + JetBrains Mono (labels).

**Restricción de paleta:** No azul, no púrpura. Solo earth tones + monochrome + warm.

---

## 🚀 Cómo correr localmente

### Opción 1 — Abrir el HTML directo

```bash
# Solo necesitás un browser moderno
# Doble-click en index.html
```

### Opción 2 — Servidor local con Python

```bash
cd speakup-resources
python -m http.server 8080
# Abrir http://localhost:8080
```

### Opción 3 — Servidor local con Node

```bash
cd speakup-resources
npx serve .
# Abrir http://localhost:3000
```

---

## 📂 Estructura del proyecto

```
speakup-resources/
├── index.html              # Landing completa (107KB, 138 links)
├── spec.md                 # Design spec + asset strategy
├── README.md               # Este archivo
├── .gitignore              # Archivos ignorados por git
├── imgs/
│   ├── hero.jpg            # Conference hall golden hour
│   └── paper-texture.jpg   # Textura para overlay
└── videos/                 # Reservado para hero video loop (futuro)
```

---

## 🛠️ Tech stack

| Layer | Tech |
|---|---|
| Markup | HTML5 semántico |
| Styling | CSS3 (custom properties, grid, flex, scroll animations) |
| Scripts | Vanilla JavaScript (Intersection Observer) |
| Fonts | Google Fonts (Fraunces, Inter, JetBrains Mono) |
| Deployment | `mavis website_deploy` (space.minimax.io) |

**Sin build step. Sin dependencias. Sin frameworks.**

---

## 📦 Deploy

El sitio está deployado vía la herramienta `website_deploy` de Mavis:

```bash
# El deploy se hace desde la tool, no necesita CLI externo
# Resultado: https://<random>.space.minimax.io
```

Para re-deployar después de cambios:

1. Modificar `index.html` (o assets en `imgs/`)
2. Llamar `website_deploy` con el directorio como `dist_dir`
3. Copiar el nuevo URL

---

## 🗺️ Roadmap

- [ ] Hero video loop en MP4 (cuando se regeneren créditos de generación)
- [ ] Filtros visuales clickeables (chips arriba del catálogo para filtrar por tipo/costo)
- [ ] Sección comparativa de paid agencies (costo vs ROI)
- [ ] Versión PDF descargable del catálogo
- [ ] Internacionalización (EN/ES switcher)
- [ ] Auto-update mensual vía CMS (reemplazar HTML estático)
- [ ] Perfiles de cada speaker como sub-páginas con su lista personalizada de sitios

---

## 🤝 Contribuir

Este es un proyecto propietario de **SpeakUp Express**. Para sugerir sitios o actualizaciones:

1. **Jhon Cordero** (SMM) — `jhon.dev.30` en GitHub / `@Jhondev-30`
2. Abrir un issue con el tag `event-suggestion` o `speaker-update`
3. Formato sugerido: `Sitio: [nombre] | Categoría: [cat] | Speaker fit: [nombre] | Tipo: [Out/In] | Costo: [Free/Freemium/Paid]`

---

## 📊 Stats

| Métrica | Valor |
|---|---|
| Sitios en el catálogo | 120+ |
| Categorías | 7 |
| Speakers | 12 |
| External links | 138 |
| HTML size | 107 KB |
| Asset images | 2 |
| Deployment | space.minimax.io |

---

## 📄 Licencia

**Proprietary** — © 2026 SpeakUp Express · Orlando FL. Todos los derechos reservados.

Este proyecto es de uso interno de SpeakUp Express. Los links externos pertenecen a sus respectivos owners.

---

## ✍️ Autoría

- **Cliente:** SpeakUp Express (US-based, Orlando FL)
- **Project lead:** Jhon Cordero Perozo · SMM · [GitHub @Jhondev-30](https://github.com/Jhondev-30) · Barquisimeto, Venezuela
- **Built with:** Mavis AI · Julio 2026

---

*Última actualización: 31 jul 2026*
