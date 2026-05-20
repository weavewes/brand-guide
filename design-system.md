# 🎨 Design System — Lovable-Inspired (v5 — Complete)

---

## Filosofía de Sombras

- Sistema de profundidad **intencionalmente shallow**
- No floating cards con drop-shadows dramáticos
- Contención por bordes cálidos (`#eceae4`) contra la superficie crema
- **Solo shadow notable:** inset shadow en botones oscuros (multi-capa)
- El warm focus shadow es deliberadamente diffused y large: `rgba(0,0,0,0.1) 0px 4px 12px`

---

## Depth Profundo — Decorativo

- Hero: warm multi-color gradient wash (pinks, oranges, blues) detrás del hero — atmosférico, apenas visible
- Footer: gradient background con tonos cálidos
- Sin section dividers duros — spacing y background warmth manejan transiciones

---

## Do's and Don'ts

### ✅ Do
- Fondo crema (`#f7f4ed`) como foundation
- Camera Plain Variable en display con negative letter-spacing (-0.9px a -1.5px)
- Todos los grises de `#1c1c1c` a opacidades variadas
- Inset shadow en botones oscuros
- `#eceae4` borders para contención de cards (no shadows)
- Weight system narrow: **400** body/UI, **600** headings
- Full-pill (`9999px`) solo para action pills e icon buttons
- Opacity **0.8** en active states

### ❌ Don't
- No white (`#ffffff`) como fondo de página
- No box-shadows para cards
- No saturated accent colors — paleta warm-neutral
- No weight **700** — **600** es el máximo
- No `9999px` en botones rectangulares — pills son para icon/action toggles
- No sharp focus outlines — usar soft shadow
- No mixing border styles — `#eceae4` passive, `rgba(28,28,28,0.4)` interactive
- No increased letter-spacing en headings

---

## Iteration Guide — 7 Reglas

1. **Siempre usa cream (#f7f4ed) como base** — nunca blanco puro
2. **Deriva grises de #1c1c1c a opacidades variadas** — no hex values distintos
3. **Usa #eceae4 borders para contención** — no shadows
4. **Letter-spacing escala con tamaño:** -1.5px en 60px, -1.2px en 48px, -0.9px en 36px, normal en 16px
5. **Dos pesos:** 400 (todo excepto headings) y 600 (headings)
6. **El inset shadow en botones oscuros es la firma** — no omitirlo
7. **Camera Plain Variable weight 480** es solo para momentos especiales de display

---

## Example Component Prompts

### Hero Section
```
"Create a hero section on cream background (#f7f4ed). Headline at 60px Camera Plain Variable weight 600, line-height 1.10, letter-spacing -1.5px, color #1c1c1c. Subtitle at 18px weight 400, line-height 1.38, color #5f5f5d. Dark CTA button (#1c1c1c bg, #fcfbf8 text, 6px radius, 8px 16px padding, inset shadow) and ghost button (transparent bg, 1px solid rgba(28,28,28,0.4) border, 6px radius)."
```

### Card
```
"Design a card on cream (#f7f4ed) background. Border: 1px solid #eceae4. Radius 12px. No box-shadow. Title at 20px Camera Plain Variable weight 400, line-height 1.25, color #1c1c1c. Body at 14px weight 400, color #5f5f5d."
```

### Template Gallery
```
"Build a template gallery: grid of cards with 12px radius, 1px solid #eceae4 border, cream backgrounds. Each card: image with 12px top radius, title below. Hover: subtle border darkening."
```

### Navigation
```
"Create navigation: sticky on cream (#f7f4ed). Camera Plain 16px weight 400 for links, #1c1c1c text. Dark CTA button right-aligned with inset shadow. Mobile: hamburger menu with 6px radius."
```

### Stats Section
```
"Design a stats section: large numbers at 48px Camera Plain weight 600, letter-spacing -1.2px, #1c1c1c. Labels below at 16px weight 400, #5f5f5d. Horizontal layout with 32px gap."
```

---

## Quick Color Reference

| Uso | Color |
|-----|-------|
| Primary CTA | Charcoal (`#1c1c1c`) |
| Background | Cream (`#f7f4ed`) |
| Heading text | Charcoal (`#1c1c1c`) |
| Body text | Muted Gray (`#5f5f5d`) |
| Border passive | `#eceae4` |
| Border interactive | `rgba(28,28,28,0.4)` |
| Focus shadow | `rgba(0,0,0,0.1) 0px 4px 12px` |
| Button text on dark | `#fcfbf8` |

---

## Paleta de Colores — Completa

### Primary
- **Cream:** `#f7f4ed` — fondo de página, cards, superficies
- **Charcoal:** `#1c1c1c` — textos primarios, headings, botones oscuros
- **Off-White:** `#fcfbf8` — texto en botones oscuros

### Escala Neutro (por opacidad desde #1c1c1c)
| Opacidad | Uso |
|----------|-----|
| 100% | Textos primarios |
| 83% | Textos secundarios fuertes |
| 82% | Body copy |
| 40% | Bordes interactivos, outlines |
| 4% | Hover backgrounds sutiles |
| 3% | Overlays apenas visibles |

### Surface & Border
- `#eceae4` — bordes de cards, divisores (Light Cream)
- `#5f5f5d` — textos secundarios, placeholders

### Interactive
- Ring Blue: `rgba(59,130,246,0.5)`
- Focus Shadow: `rgba(0,0,0,0.1) 0px 4px 12px`

---

## Tipografía

### Familia
- **Primary:** Camera Plain Variable
- **Fallbacks:** `ui-sans-serif, system-ui`
- **Peso continuo:** 400, 480, 600 (eje variable permite valores intermedios como 480)

### Jerarquía

| Rol | Tamaño | Peso | Line Height | Letter Spacing |
|-----|--------|------|------------|----------------|
| Display Hero | 60px | 600 | 1.00-1.10 | **-1.5px** |
| Display Alt | 60px | 480 | 1.00 | normal |
| Section Heading | 48px | 600 | 1.00 | **-1.2px** |
| Sub-heading | 36px | 600 | 1.10 | **-0.9px** |
| Card Title | 20px | 400 | 1.25 | normal |
| Body Large | 18px | 400 | 1.38 | normal |
| Body | 16px | 400 | 1.50 | normal |
| Button | 16px | 400 | 1.50 | normal |
| Button Small | 14px | 400 | 1.50 | normal |
| Caption | 14px | 400 | 1.50 | normal |

### Principios
- Solo 2 pesos: **400** (body/UI) y **600** (headings)
- Headlines con **negative letter-spacing** para impacto editorial
- Body text con tracking normal para lectura cómoda

---

## Border Radius Scale

| Uso | Radio |
|-----|-------|
| Micro (4px) | Small buttons, interactive |
| Standard (6px) | Buttons, inputs, nav |
| Comfortable (8px) | Compact cards, divs |
| Card (12px) | Standard cards, images, templates |
| Container (16px) | Large containers, footer |
| Full Pill (9999px) | Action pills, icon buttons, toggles |

---

## Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Flat (Level 0) | No shadow, cream background | Page surface |
| Bordered (Level 1) | `1px solid #eceae4` | Cards, images |
| Inset (Level 2) | Multi-layer inset shadow | Dark buttons |
| Focus (Level 3) | `rgba(0,0,0,0.1) 0px 4px 12px` | Active/focus |
| Ring (Accessibility) | `rgba(59,130,246,0.5) 2px ring` | Keyboard focus |

---

## Botones

### Primary Dark (CTA principal)
- Background: `#1c1c1c`
- Text: `#fcfbf8`
- Padding: 8px 16px
- Border-radius: **6px** (NO pill)
- Inset shadow multi-capa (ver abajo)
- Active: `opacity: 0.8`
- Focus: `rgba(0,0,0,0.1) 0px 4px 12px shadow`

### Inset Shadow Multi-capa (Firma Lovable)
```css
box-shadow: 
  rgba(0,0,0,0) 0px 0px 0px 0px,
  rgba(0,0,0,0) 0px 0px 0px 0px,
  rgba(255,255,255,0.2) 0px 0.5px 0px 0px inset,
  rgba(0,0,0,0.2) 0px 0px 0px 0.5px inset,
  rgba(0,0,0,0.05) 0px 1px 2px 0px;
```

### Ghost / Outline
- Background: transparent
- Text: `#1c1c1c`
- Border: `1px solid rgba(28,28,28,0.4)`
- Border-radius: **6px**
- Active: `opacity: 0.8`

### Cream Surface
- Background: `#f7f4ed`
- Text: `#1c1c1c`
- Border-radius: **6px**
- Sin borde

### Pill / Icon Button
- Background: `#f7f4ed`
- Border-radius: **9999px** (full pill)
- Inset shadow como Primary Dark
- Opacity: **0.5** default, **0.8** active

---

## Cards & Containers

- Background: `#f7f4ed`
- Border: `1px solid #eceae4`
- Radius: **12px** (standard), **16px** (featured), **8px** (compact)
- **Sin box-shadow** por defecto — bordes definen límites
- Image cards: `1px solid #eceae4` con 12px radius

---

## Inputs & Forms

- Background: `#f7f4ed`
- Text: `#1c1c1c`
- Border: `1px solid #eceae4`
- Radius: **6px**
- Focus: ring blue `rgba(59,130,246,0.5)` outline
- Placeholder: `#5f5f5d`

---

## Navigation

- Nav horizontal limpia sobre fondo crema, fixed
- Logo left-aligned (128.75 x 22px)
- Links: Camera Plain 14–16px weight 400
- CTA: dark button con inset shadow, 6px radius
- Mobile: hamburger menu con botón 6px radius
- Borde sutil o sin borde on scroll

---

## Links

- Color: `#1c1c1c`
- Decoración: **underline** (default)
- Hover: primary accent (CSS variable `hsl(var(--primary))`)
- Sin cambio de color en hover — la **decoración** es la señal interactiva

---

## Image Treatment

- `1px solid #eceae4` border, 12px radius
- Fondos con gradiente suave detrás del hero
- Presentación estilo galería para showcases

---

## Distinctive Components

### AI Chat Input
- Large prompt input area con bordes suaves
- Suggestion pills con bordes `#eceae4`
- Voice recording / plan mode toggle como pills (9999px)
- Área cálida y invitadora — no clínica

### Template Gallery
- Card grid con templates de proyectos
- Cada card: imagen + título, `1px solid #eceae4`, 12px radius
- Hover: shadow sutil o borde más oscuro

### Stats Bar
- Métricas grandes: "0M+" en 48px+ weight 600
- Texto descriptivo debajo en muted gray
- Layout horizontal con espaciado generoso

---

## Responsive Breakpoints

| Name | Width |
|------|-------|
| Mobile Small | <600px |
| Mobile | 600–640px |
| Tablet Small | 640–700px |
| Tablet | 700–768px |
| Desktop Small | 768–1024px |
| Desktop | 1024–1280px |
| Large Desktop | 1280–1536px |

### Touch Targets
- Buttons: 8px 16px padding
- Pill buttons: radio 9999px para tap targets grandes
- Menu toggle: botón 6px radius

---

## Layout — Sistema de Espaciado

**Base unit:** 8px

**Escala:** 8, 10, 12, 16, 24, 32, 40, 56, 80, 96, 128, 176, 192, 208px

- Sections usan **80px–208px** vertical spacing
- Máximo content width: **~1200px** (centrado)
- Hero: single-column centrado con padding vertical masivo (96px+)
- Feature sections: grids de 2–3 columnas
- Footer full-width con layout multi-columna

---

## Stack Técnico

- **shadcn/ui** — componentes base
- **Radix UI** — primitivas
- **Tailwind CSS** — utilidades
- **React** — framework

---

## Próximo Paso

Cuando Héctor pase el stack y requerimientos del frontend, estamos listos para construir.

---

*Versión: v5 — Complete*
*Última actualización: 2026-05-07*
