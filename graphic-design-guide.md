# 🎨 Weaves Graphic Design Guide — For AI Design Agents

> **Purpose:** Enable AI design agents (PRISMA and others) to create consistent, brand-aligned graphic materials.  
> **Scope:** Logos, banners, social media posts, business cards, ads, infographics, presentations.  
> **Version:** 1.0  
> **Last Updated:** 2026-05-20

---

## 1. Brand Visual Identity

### 1.1 Core Colors

| Name | Hex | RGB | CMYK | Usage |
|------|-----|-----|------|-------|
| **Cream** | `#f7f4ed` | `247, 244, 237` | `0, 1, 4, 3` | Primary background, paper feel |
| **Charcoal** | `#1c1c1c` | `28, 28, 28` | `0, 0, 0, 89` | Primary text, dark elements, logos on light |
| **Off-White** | `#fcfbf8` | `252, 251, 248` | `0, 0, 2, 1` | Text on dark backgrounds, subtle highlights |
| **Light Cream** | `#eceae4` | `236, 234, 228` | `0, 1, 3, 7` | Borders, dividers, subtle backgrounds |
| **Muted Gray** | `#5f5f5d` | `95, 95, 93` | `0, 0, 2, 63` | Secondary text, captions, descriptions |

#### Extended Palette (Accents — Use Sparingly)
| Name | Hex | Usage |
|------|-----|-------|
| **Warm Blush** | `#e8a598` | Soft accents, decorative elements |
| **Sage Green** | `#9fb4a2` | Natural, eco-friendly vibes |
| **Dusty Blue** | `#a8b5c4` | Tech, trust, professionalism |
| **Terracotta** | `#c4785a` | Warm CTAs, highlights |

> **Rule:** Cream + Charcoal are the heroes. Accent colors must never exceed 15% of any composition.

---

### 1.2 Typography

#### Primary Font
- **Family:** `Camera Plain Variable` (or fallback: `ui-sans-serif, system-ui`)
- **Weights for Graphic Design:**
  - **400** — Body text, descriptions, captions
  - **600** — Headlines, titles, emphasis
  - **480** — Special display moments (hero headlines)

#### Scale for Print & Digital Graphics

| Role | Size (Print) | Size (Digital) | Weight | Line Height | Letter Spacing |
|------|-------------|----------------|--------|-------------|----------------|
| Hero Headline | 48-72pt | 60-96px | 600 | 1.00-1.10 | **-1.5px** |
| Section Title | 36-48pt | 48-64px | 600 | 1.10 | **-1.2px** |
| Sub-heading | 24-36pt | 36-48px | 600 | 1.10 | **-0.9px** |
| Card Title | 18-24pt | 20-28px | 400 | 1.25 | normal |
| Body | 12-14pt | 16-18px | 400 | 1.50 | normal |
| Caption | 10-12pt | 12-14px | 400 | 1.50 | normal |

> **Print Rule:** Always use points (pt) for print materials. Minimum body text: 10pt.

---

### 1.3 Logo Usage

#### Logo Variants
1. **Full Logo (horizontal)** — Wordmark + icon side by side
2. **Icon Only** — Octopus symbol (🐙) as standalone mark
3. **Wordmark Only** — "Weaves" text without icon

#### Clear Space
- Minimum clear space around logo: **equal to the height of the "W" in Weaves**
- Never crowd the logo with text, images, or other elements

#### Background Rules
| Logo Variant | Light Background (Cream/White) | Dark Background (Charcoal/Black) |
|--------------|-------------------------------|----------------------------------|
| Full Logo | Charcoal (`#1c1c1c`) | Off-White (`#fcfbf8`) |
| Icon Only | Charcoal (`#1c1c1c`) | Off-White (`#fcfbf8`) |
| Wordmark Only | Charcoal (`#1c1c1c`) | Off-White (`#fcfbf8`) |

> **Never:** Place logo on busy backgrounds, stretch/distort it, or use unapproved colors.

---

### 1.4 Visual Style Principles

- **Warm Minimalism:** Clean layouts with generous whitespace. No clutter.
- **Soft Depth:** Prefer borders (`#eceae4`) over drop shadows. If shadow needed, use: `rgba(0,0,0,0.1) 0px 4px 12px`
- **Editorial Feel:** Large headlines with tight letter-spacing. Elegant, not corporate.
- **Human Touch:** Warm tones, no cold blues or harsh reds as primary.
- **Consistent Radius:** 6px (buttons), 12px (cards), 9999px (pills)

---

## 2. AI Prompt Templates

> **Golden Rule:** Always include brand colors, font reference, and style keywords in every prompt.

### 2.1 Logo Design Prompt

```
Create a [modern/minimal/abstract] logo for "Weaves" — a technology and automation agency.

Style:
- Minimalist, warm, sophisticated
- Colors: Charcoal (#1c1c1c) on Cream (#f7f4ed) background
- Feel: Premium, trustworthy, innovative
- No gradients, no 3D effects
- Clean vector style suitable for print and digital

Symbol ideas (choose one direction):
- Interconnected nodes or threads (representing "weaving" systems)
- Abstract octopus (intelligence, multi-tasking)
- Geometric weave pattern

Deliverable:
- SVG format
- Versions: full logo, icon only, wordmark only
- Include safe space guidelines
```

### 2.2 Social Media Post Prompt

```
Create an Instagram/LinkedIn post for Weaves about [TOPIC].

Format: 1080x1080px (square) or 1080x1350px (portrait)

Style:
- Background: Cream (#f7f4ed) or soft gradient (blush #e8a598 to cream)
- Headline: Camera Plain Variable, weight 600, 36-48px, Charcoal (#1c1c1c), letter-spacing -0.9px
- Body: Camera Plain Variable, weight 400, 16-18px, Muted Gray (#5f5f5d)
- Layout: Centered or left-aligned with generous padding (80px+ margins)
- Decorative: Subtle geometric shapes or thin lines (#eceae4)
- No stock photos — use abstract shapes, patterns, or icons

Brand elements to include:
- Weaves logo (bottom corner, small, charcoal)
- Warm, inviting tone
- Clean whitespace

Deliverable:
- PNG, 1080x1080px, 300 DPI
```

### 2.3 Banner/Header Prompt

```
Create a website hero banner or LinkedIn cover for Weaves.

Format: 1920x1080px (web hero) or 1584x396px (LinkedIn cover)

Style:
- Background: Cream (#f7f4ed) with subtle warm gradient wash (soft pinks, oranges, blues — atmospheric, barely visible)
- Headline: "[HEADLINE TEXT]" — Camera Plain Variable, 60-72px, weight 600, Charcoal (#1c1c1c), letter-spacing -1.5px
- Subtitle: Optional, 18-24px, weight 400, Muted Gray (#5f5f5d)
- CTA button area: Charcoal (#1c1c1c) background, Off-White (#fcfbf8) text, 6px radius
- Layout: Single column, centered, massive vertical padding
- No illustrations unless abstract/minimal
- No photos of people

Deliverable:
- PNG or JPG, optimized for web (< 500KB)
```

### 2.4 Business Card Prompt

```
Create a business card design for Weaves.

Format: 3.5 x 2 inches (standard US), include bleed (0.125" on all sides)

Style:
- Front:
  - Background: Cream (#f7f4ed)
  - Logo: Charcoal (#1c1c1c), centered or top-left
  - Name & Title: Camera Plain Variable, weight 600, Charcoal
  - Contact info: weight 400, Muted Gray (#5f5f5d)
  - Subtle border: 1px solid #eceae4
- Back:
  - Background: Charcoal (#1c1c1c)
  - Logo: Off-White (#fcfbf8), centered
  - Or: Solid cream with large watermark logo (10% opacity)

Paper feel: Matte, textured, premium

Deliverable:
- PDF with bleed marks
- SVG for vector editing
```

### 2.5 Infographic Prompt

```
Create an infographic for Weaves about [TOPIC/DATA].

Format: 1080x1920px (vertical) or 1920x1080px (horizontal)

Style:
- Background: Cream (#f7f4ed)
- Data visualization: Clean lines, minimal bars/pies
- Colors: Charcoal for primary data, Sage Green (#9fb4a2) for positive, Dusty Blue (#a8b5c4) for neutral, Terracotta (#c4785a) for highlights
- Typography: Hierarchical — large numbers (48px+, weight 600), labels (16px, weight 400)
- Layout: Clear visual flow, numbered sections, generous spacing between elements
- Icons: Line style, 1.5px stroke, Charcoal (#1c1c1c)

Deliverable:
- PNG, high resolution
- Source file (SVG or Figma-compatible)
```

### 2.6 Presentation Slide Prompt

```
Create a presentation slide template for Weaves.

Format: 1920x1080px (16:9)

Style:
- Background: Cream (#f7f4ed)
- Title: Camera Plain Variable, 48-60px, weight 600, Charcoal, letter-spacing -1.2px
- Body: 20-24px, weight 400, Muted Gray (#5f5f5d)
- Bullets: Minimal, using dashes or small dots
- Accent bars: Thin lines (2px) in Charcoal or accent color
- Logo: Bottom right, small, charcoal
- Slide types:
  - Title slide: Large centered headline, minimal
  - Content slide: Left-aligned text, generous padding
  - Data slide: Large stat + supporting text
  - Quote slide: Large quotation, attribution below

Deliverable:
- PNG per slide
- PPTX or Google Slides compatible template
```

---

## 3. Format & Technical Specifications

### 3.1 Resolution Guide

| Use Case | Dimensions | DPI | Format |
|----------|-----------|-----|--------|
| Social Media (Square) | 1080x1080px | 72 | PNG/JPG |
| Social Media (Portrait) | 1080x1350px | 72 | PNG/JPG |
| Social Media (Story) | 1080x1920px | 72 | PNG/JPG |
| Website Hero | 1920x1080px | 72 | PNG/JPG/WebP |
| Website Banner | 1920x600px | 72 | PNG/JPG/WebP |
| LinkedIn Cover | 1584x396px | 72 | PNG/JPG |
| Business Card | 3.5x2in + bleed | 300 | PDF/SVG |
| Print Flyer (US Letter) | 8.5x11in + bleed | 300 | PDF |
| Presentation Slide | 1920x1080px | 72 | PNG/PPTX |
| Logo (Master) | Vector | N/A | SVG |
| Logo (Fallback) | 1024x1024px | 300 | PNG |

### 3.2 File Naming Convention

```
weaves_[type]_[variant]_[date]_[version].[ext]

Examples:
- weaves_logo_full_2026-05-20_v1.svg
- weaves_social_instagram-post_2026-05-20_v1.png
- weaves_banner_hero-web_2026-05-20_v1.jpg
- weaves_card_business-front_2026-05-20_v1.pdf
```

### 3.3 Safe Zones & Bleed

| Material | Bleed | Safe Zone |
|----------|-------|-----------|
| Business Card | 0.125" (3mm) | 0.125" from trim edge |
| Flyer/Poster | 0.125" (3mm) | 0.25" from trim edge |
| Banner | 0.5" (12mm) | 1" from trim edge |
| Digital only | N/A | Keep text 80px from edges |

---

## 4. Do's and Don'ts for AI Agents

### ✅ DO
- Use Cream (`#f7f4ed`) as the default background
- Use Charcoal (`#1c1c1c`) for primary text and dark elements
- Apply negative letter-spacing on headlines (-0.9px to -1.5px)
- Use 400 weight for body text, 600 for headlines
- Maintain generous whitespace (80px+ margins on digital, 0.5in+ on print)
- Use 6px radius for buttons, 12px for cards
- Keep logo clear space equal to the "W" height
- Use subtle borders (`#eceae4`) instead of drop shadows
- Export print materials at 300 DPI
- Export digital materials at 72 DPI

### ❌ DON'T
- Use pure white (`#ffffff`) as page background
- Use saturated, bright colors (neon, high-chroma)
- Apply drop shadows to cards (use borders instead)
- Use weight 700 (600 is the max)
- Use 9999px (full pill) on rectangular buttons (only for icon/action pills)
- Place text or important elements within bleed areas
- Crowd the logo or reduce clear space
- Mix border styles (passive vs interactive)
- Use stock photos of people without approval
- Create busy, cluttered layouts

---

## 5. Quick Reference Card

```
BRAND COLORS
├── Cream:        #f7f4ed  (backgrounds)
├── Charcoal:     #1c1c1c  (text, dark elements)
├── Off-White:    #fcfbf8  (text on dark)
├── Light Cream:  #eceae4  (borders)
├── Muted Gray:   #5f5f5d  (secondary text)
└── Accents:      #e8a598, #9fb4a2, #a8b5c4, #c4785a (sparingly)

TYPOGRAPHY
├── Font: Camera Plain Variable
├── Headlines: 600 weight, negative letter-spacing
├── Body: 400 weight, normal spacing
└── Never use weight 700

STYLE
├── Warm minimalism
├── Editorial elegance
├── Soft depth (borders > shadows)
├── Generous whitespace
└── Consistent border radius: 6px / 12px / 9999px

LOGO
├── Clear space = height of "W"
├── Light bg: Charcoal logo
├── Dark bg: Off-White logo
└── Never distort or crowd
```

---

## 6. Example Outputs

> **Note:** Include reference images or links to approved designs here for AI agents to learn from.
> 
> Placeholder for:
> - Approved logo files
> - Example social media posts
> - Example banner designs
> - Example business cards
> - Example infographics

---

*Document maintained by PRISMA (Chief Creative Officer) and NEXUS (CEO & General Orchestrator).*  
*For questions or updates, route through PRISMA.*
