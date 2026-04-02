# HELM Brand Guide

## Brand Identity

HELM is a luxury hospitality marketplace combined with an agentic AI event planner. The brand bridges premium service with intelligent automation — positioning itself as the "Airbnb for luxury event talent."

## Color Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Burgundy | `#5B1A2A` | Primary brand color, headings, cards |
| Burgundy Dark | `#3D0F1C` | Gradients, header background |
| Red | `#C41E3A` | Accent, active states, CTAs |
| Red Bright | `#E63946` | Gradient highlights, dot indicators |
| Gold | `#B8860B` | Section labels, premium accents |
| Cream | `#F5F0E8` | Page background |
| Cream Dark | `#EDE5D8` | Card backgrounds, subtle contrast |
| Charcoal | `#2C2C2C` | Body text |

## Typography

| Role | Font | Weights | Style |
|------|------|---------|-------|
| Headings | Cormorant Garamond | 400–700 | Italic for section headings |
| Body | Poppins | 300–700 | Clean, modern readability |
| Accent | Rubik | 400, 500, 700 | UI elements, labels |

### Heading Hierarchy
- Section labels: Gold, uppercase, 0.8rem, 0.2em letter-spacing (Rubik)
- Section headings: Burgundy, italic serif (Cormorant Garamond)
- Card headings: Burgundy or white depending on card background

## Visual Language

### Glassmorphism
- `.glass`: Subtle frosted glass (`backdrop-blur-md`, white/30 background)
- `.glass-dark`: Darker variant (white/10 background)
- `.glass-strong`: More opaque (white/50 background)

### Cards
- `.card-burgundy`: Gradient burgundy background with rounded corners, hover lift effect
- `.card-red-accent`: 4px red left border for emphasis

### Pills / Badges
- `.pill`: Burgundy outline with cream background, rounded-full
- `.pill-red`: Gradient red-to-burgundy filled badge with glow shadow

## Logo Assets

| File | Usage |
|------|-------|
| `helm-logo-burgundy.png` | Hero slide (main logo, cropped) |
| `helm-logo-white.png` | Light-on-dark contexts (cropped) |
| `helm-submark-burgundy.png` | Section headers (H monogram) |
| `helm-submark-white.png` | Fixed header navigation |
| `helm-submark-ivory.png` | Watermark / background accents |

### Logo Sizing
- Header submark: `h-7` (28px)
- Section submarks: `h-5` mobile, `h-7` tablet+
- Hero logo: Width-based sizing (`max-w-[90vw]` mobile, `max-w-xl` desktop)

## Animation Patterns

- **Entrance animations:** `.fade-up`, `.fade-left`, `.fade-right`, `.scale-in` — triggered by IntersectionObserver
- **Marquee scrolling:** Continuous horizontal scroll for photo strips (25s linear infinite)
- **Dot indicators:** Red active dot (12px wide), muted inactive dots (5-6px), 0.3s transitions
- **Counter animation:** Tabular-nums with eased count-up on scroll visibility

## Mobile Design Principles

- Content-heavy slides use Swiper carousels (one card at a time with dot indicators)
- Grid layouts stack vertically below `md` (768px) breakpoint
- Horizontal card rows with icon + text on mobile for compact information density
- Touch-optimized with momentum scrolling (`-webkit-overflow-scrolling: touch`)
- All slides use `100dvh - 56px` to account for the fixed header
