# Wan Advertising — Link-in-Bio Design Spec

## Style Direction
Brutalist. Raw, confident, high-contrast. Sharp corners (no border-radius), thick black borders, hard offset drop-shadows (not soft/blurred). Feels like a printed agency deck, not a soft SaaS landing page.

---

## Colors

| Name   | Hex       | Usage                                   |
| --------| -----------| -----------------------------------------|
| Cream  | `#F2EEE4` | Page background                         |
| Black  | `#141210` | Text, borders, header logo bg           |
| Orange | `#F4B71B` | Accent — dot, index tags, status strip  |
| White  | `#FFFFFF` | Card backgrounds (header, link buttons) |

Optional background texture: faint 40px grid drawn with 1px black lines at low opacity over the cream background (subtle graph-paper feel).

---

## Typography

- **Display / headings:** `Archivo Black` (Google Fonts) — bold, uppercase, tight letter-spacing (-0.01em)
- **Body / tagline:** `Space Grotesk` — regular weight
- **Labels / mono details (index numbers, status strip, footer):** `JetBrains Mono` — uppercase, letter-spacing 0.06–0.08em, small size (10–13px)

Font sizes (mobile → desktop):
- H1 (agency name): 26px → 34px
- Tagline: 12.5px → 13.5px
- Link title: 16px → 18px
- Index/mono labels: 10–11px throughout

---

## Layout & Spacing

- Mobile-first, single column, max-width ~460px, centered
- Desktop breakpoint at `760px`: max-width grows to ~560px, padding/shadows scale up
- Larger desktop breakpoint at `1100px`: max-width ~620px
- Consistent 16–20px page padding on mobile; 44px+ inside header on desktop

---

## Components

### Header card
- White background, 3px black border, 8px/8px hard black shadow (offset, no blur)
- Contains: brand logo mark (`image/wan-dark.png`, ~44px tall), agency name, tagline
- Tagline separated by a 2px black top border, with an orange "." accent at the end

### Status strip
- Full-width orange bar, 3px black border, mono uppercase text
- Left: "Status" label · Right: "Open for projects" (white text)

### Link buttons (x4: Website, Instagram, TikTok, WhatsApp)
- White background (WhatsApp button uses inverted black background as the accent/primary CTA)
- 3px black border, 6px/6px hard shadow (8px on desktop)
- Left side: black square index tag (01–04) + link name (bold, uppercase) + small gray subtext line
- Right side: orange arrow "→"
- Hover: button shifts up-left 3px, shadow grows to 9px/9px, background shifts to cream
- Active/tap: shadow collapses to 3px/3px (pressed effect)

### Footer
- Centered, small orange horizontal line (60px wide, 3px tall) above text
- Mono uppercase small text: agency name + location

---

## Interaction Notes
- All link buttons open in new tab (`target="_blank" rel="noopener"`)
- No JavaScript required — pure CSS hover/active states
- Reduce-motion: disable hover transform/transition for users with `prefers-reduced-motion`

---

## Content (placeholders — replace with real values)
- Agency name: Wan Advertising
- Tagline: "Banner & signboard printing."
- Website: `https://wanadvertising.com`
- Instagram: `https://instagram.com/wanadvertising`
- TikTok: `https://tiktok.com/@wanadvertising`
- WhatsApp: `https://wa.me/60000000000` *(replace with real number, country code + digits only)*
- Footer location: Kuala Lumpur