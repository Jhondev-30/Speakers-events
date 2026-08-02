# 🎤 SpeakUp Express — Speaker Resources

> Catálogo curado de 155 sitios web donde los speakers de **SpeakUp Express** encuentran eventos presenciales, podcasts, summits virtuales, comunidades de organizadores y networking. Cada sitio viene con info detallada de cómo aplicar, pitch template, requisitos, tiempo de respuesta y probabilidad de éxito.

🔗 **Live:** https://speakup-resources.pages.dev (Cloudflare Pages) o la URL de space.minimax.io del último deploy

---

## 📖 Sobre el proyecto

Esta landing es un **catálogo de discovery + sales enablement** para los 12 speakers de la red SpeakUp Express. Cada sitio del catálogo viene con 4 señales que permiten decidir dónde aplicar primero:

- **Tipo** — Outbound (speaker aplica) vs Inbound (organizer te busca) vs Podcast vs Networking
- **Costo** — Free, Freemium, Paid, Full-service
- **Probabilidad de pago** — $$$ Alto, $$ Medio, Exposure, Ticket only
- **Tipo de acceso** — CFP Abierto, CFP Curado, Directorio, Agencia, Podcast Match, Comunidad, Database, Newsletter

**Sección estrella: Top 25 sitios priorizados** con criterios estratégicos (US-only, pago real, dificultad baja-media, match con speakers, CFP accesible) — dividido en Tier A (esta semana), Tier B (este mes), Tier C (ongoing).

### Speakers cubiertos (12)

| Speaker | Nicho principal | Top matches |
|---|---|---|
| **Angie Pichardo** | Faith · Suicide/NDE Survivor | IF:Gathering, Worthy Woman, Catalyst, She Speaks, AAS Stipend |
| **Dr. Phillip Meade** | Senior Pastor · Leadership · NASA | Premiere Bureau, AAS, Catalyst, IEEE |
| **Patricio Larrea** | Growth · LATAM · Forbes | Web Summit, SaaStr AI, Digital Summit, Dreamforce |
| **Angelie Kapoor** | Faith · Christian Women · FL | Crowned, Listen To Her, EPIC, Worthy Woman |
| **Kimberly Aschman** | Real Estate · Business · FL | WBENC, AnitaB Topala, WITI, Women in Tech Summit |
| **Kelly White** | Career · Reinvention | WBENC, iRelaunch, MAKERS, Women in Sales |
| **Philip Chan** | Multi-Exit · Finance · 11.6k LI | SaaStr AI, Mastermind Talks, Dreamforce, WITI |
| **Russ Katzman** | Leadership · Enterprise | AAS, Premiere, C12, IEEE, Goldman Sachs Talks |
| **Jeff Forrester** | Faith · Leadership · FCA+UF | Catalyst, RightNow, Equip, Church Comms |
| **Evelena Dawson** | Affirmed Women · Faith | IF:Gathering, True Woman, EPIC, Worthy Woman |
| **Alex Berman** | Sales · Best-selling author | Premiere Bureau, Dreamforce, PodMatch, SaaStr |
| **Rachel Scheer** | Wellness · Nutrition | Wellness Show, Integrative Healthcare, iRelaunch |

---

## ✨ Features

- **155 sitios curados** en 11 categorías (CFP, Directories, Podcasts, Summits, Comunidades, Networking, Top-tier $$$, Faith-based, Women-focused, etc.)
- **Sección "★ Más probables de pago"** — 15 sitios top con fee estimado y fit por speaker
- **Sección "★ Top 25 sitios priorizados"** — 3 tiers (A/B/C) con criterios estratégicos
- **Modal expandible** en cada card con: tipo de acceso, cómo funciona, paso a paso (6 pasos), tips, pitch template copiable, requisitos, tiempo de respuesta, success rate
- **Filtro interactivo** por speaker (12 chips) + Filtros por tipo/costo/pago/geo-block + búsqueda por texto
- **Botón "📋 Copiar info"** en cada modal — copia pitch template + URL + requisitos al clipboard (compatible con todo el equipo, sin localStorage)
- **Sección "Mapeo speakers → top picks"** con MUST/SHOULD/COULD tiers
- **Perfiles expandibles** de cada speaker con sus 9 sitios curated
- **Responsive** mobile-first con hamburger menu
- **Sin frameworks, sin build step, sin backend** — HTML + CSS + JS vanilla. Deploy en Cloudflare Pages o similar static host

---

## 🎨 Design system

| Token | Valor | Uso |
|---|---|---|
| `--ink-900` | `#0d1410` | Background principal |
| `--ink-800` | `#151f1c` | Cards, panels |
| `--paper-50` | `#f6efde` | Texto principal |
| `--paper-100` | `#e8d8b8` | Texto secundario |
| `--gold-500` | `#c9a14a` | Acentos, números, CTAs |
| `--copper-500` | `#b87333` | Degradados, hovers |
| `--terracotta` | `#c47a5a` | Badges de warning, alerts |
| `--sage` | `#6b8e5a` | Inbound, free, success |

**Tipografía:** Fraunces (display, editorial serif) + Inter (body) + JetBrains Mono (labels).

**Restricción de paleta:** No azul, no púrpura, no neón. Solo earth tones (charcoal-green + antique gold + warm cream).

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
├── index.html                      # Landing completa (auto-contenida, ~280KB)
├── README.md                       # Este archivo
├── CHANGELOG.md                    # Historial de versiones
├── LICENSE                         # Proprietary
├── .gitignore                      # Archivos ignorados por git
├── docs/
│   └── OUTREACH-STRATEGY.md        # Plan de outreach priorizado por tier
├── imgs/
│   ├── hero.jpg                    # Conference hall golden hour
│   └── paper-texture.jpg           # Textura para overlay
└── videos/                         # Reservado para hero video loop (futuro)
```

---

## 🛠️ Tech stack

| Layer | Tech |
|---|---|
| Markup | HTML5 semántico |
| Styling | CSS3 (custom properties, grid, flex, scroll animations, 5 breakpoints) |
| Scripts | Vanilla JavaScript (ES6+, Intersection Observer, Clipboard API) |
| Fonts | Google Fonts (Fraunces, Inter, JetBrains Mono) |
| Deploy | Cloudflare Pages (static) o space.minimax.io |

**Sin build step. Sin dependencias npm. Sin frameworks JS. Sin backend.**

---

## 🔄 Deploy

El sitio está deployado en **Cloudflare Pages** como static site:

```bash
git add -A
git commit -m "your message"
git push origin main
# Cloudflare redeploys automatically en 1-3 min
```

Para deploys manuales a space.minimax.io:
```bash
# Build a deploy dir, then use the website_deploy tool
mkdir -p deploy-temp
cp index.html deploy-temp/
# Use the deploy tool with deploy-temp as path
```

---

## 📊 Métricas del sitio

| Categoría | Count |
|---|---|
| Sitios en catálogo | 155 |
| Categorías | 11 |
| Speakers con profile | 12 |
| Tipos de flow documentados | 9 |
| Top sitios priorizados | 25 (Tier A: 10, B: 10, C: 5) |
| Sitios marcados con ⚠ Status | 6 (manual review needed) |
| Sitios geo-blocked VZ | 18 (marcados con badge) |
| Modal sections (por sitio) | 8 (tipo, cómo, paso a paso, tips, fit, pitch, response time, success rate) |
| Media queries (responsive) | 5 (1024, 900, 600, 380, 1920+) |
| External links (sitios) | 155+ |

---

## 🎯 Cómo lo construí

Diseño, desarrollo, investigación de sitios, copy de pitches, y estrategia de outreach — todo hecho a mano, iteración por iteración, con verificación visual de cada link en browser antes de commit.

**Stack elegido por:**
- Zero dependencies = deploy instant en cualquier static host
- Single HTML file = fácil de mantener, fácil de debuggear, fácil de versionar
- Sin backend = compatible con Cloudflare Pages free tier, no AWS Lambda, no DB
- Vanilla JS = cualquier developer puede contribuir sin aprender framework

**Decisiones clave que tomé:**
- **Earth tones (no blue/purple)** porque SpeakUp = voice/speaking/charisma, los azules genéricos no conectan
- **Fraunces serif para el hero** porque editorial/premium, no corporativo-tech
- **Click +Info en cada card** porque el equipo de outreach necesita saber "cómo entro" sin navegar fuera
- **Top 25 sitios priorizados** porque el usuario necesita saber "por dónde empiezo", no "toda la lista"
- **Pitch template copiable** porque el pitch genérico es 80% del trabajo, solo falta personalizar
- **Sin localStorage** porque el sitio lo usan varios miembros del equipo en el mismo dominio — clipboard es lo correcto

---

## 🛠️ Desarrollo

### Workflow
1. Editar `index.html` directo
2. Hard refresh en el browser (Ctrl+Shift+R) o DevTools > Network > Disable cache
3. Verificar con browser tool (headless)
4. Commit + push → Cloudflare redeploys

### Convenciones del código
- CSS: custom properties para todos los tokens (colores, fonts, spacing)
- JS: arrow functions, template literals, const/let, event delegation
- HTML: semantic (header, main, section, article, footer), aria-labels donde corresponde
- Mobile-first: base styles sin media query, breakpoints suben complejidad

---

## 📝 Changelog

Ver `CHANGELOG.md` para el historial completo de versiones (v1 → v13).

---

## 🤝 Licencia

Propietario. SpeakUp Express © 2026. No redistribuir sin autorización.
