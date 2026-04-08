# Portfolio Redesign Plan — "The Atelier"

## Aesthetic Direction

**Concept**: Art converging with advanced UI — vintage craft meets sophisticated digital interactions. The site should feel like walking into a designer's private studio where classical illustration, typography, and hand-drawn warmth coexist with razor-sharp modern interactions.

**Tone**: Editorial / Art-Nouveau-meets-Digital — warm, textured, unmistakably human.

**Core Principle**: The juxtaposition itself is the message. Nostalgic visual language (serif typography, ornamental dividers, aged textures, classical references) paired with contemporary web functionality (smooth scroll reveals, dynamic text treatments, magnetic hovers, parallax depth).

---

## Design System

### Typography
- **Display**: `Cormorant Garamond` (serif) — classical, elegant, high contrast. Used for name, section headings, and key statements.
- **Body**: `DM Sans` — clean geometric sans-serif for readability. Subheadings, paragraphs, labels.
- **Accent/Mono**: `JetBrains Mono` — for tech tags, code references, subtle technical identity.

### Color Palette (Dark Vintage)
| Token         | Value                        | Usage                        |
|---------------|------------------------------|------------------------------|
| `--bg`        | `#0d0c0b`                    | Page background              |
| `--bg-warm`   | `#141310`                    | Slightly lifted background   |
| `--card`      | `#1a1918`                    | Card surfaces                |
| `--gold`      | `#c9a84c`                    | Primary accent (antique gold)|
| `--cream`     | `#e8e0d0`                    | Primary text                 |
| `--muted`     | `#8a8478`                    | Secondary text               |
| `--copper`    | `#b5634b`                    | Warm accent / hover states   |
| `--border`    | `rgba(201,168,76,0.12)`      | Subtle gold borders          |

### Decorative Elements
- **Ornamental SVG dividers** between sections (flourish/scroll motifs) instead of plain `<hr>`
- **Dot grid / crosshatch texture** as subtle background overlay
- **Decorative corner brackets** on cards and featured elements
- **Hand-drawn style underlines** on key phrases

---

## Dynamic Text Treatments

1. **Hero Name — Character Stagger Reveal**: Each letter of "Vinh Le" animates in individually with slight rotation and fade, like being typeset by hand. Triggered on page load.

2. **Typewriter Subtitle**: The role/tagline types out character by character with a blinking caret cursor, evoking a vintage typewriter.

3. **Section Heading Scramble**: When section headings scroll into view, characters briefly scramble through random glyphs before resolving to the correct text — a "decoding" effect that nods to the digital.

4. **Scroll-Triggered Line Reveals**: Body text and list items slide up with staggered delays, paragraphs fade in line-by-line.

5. **Handwritten Annotations**: Key callouts (like "Top 3", "Hackathon") use a script font with a slight rotation, as if hand-annotated on the page.

---

## Section-by-Section Plan

### Navigation
- Translucent warm-dark glass with gold accent border on scroll
- Name in Cormorant Garamond serif (classical feel)
- Nav links in DM Sans (modern)
- Active link indicated by a small ornamental dot, not a background highlight
- Mobile: slide-down drawer with ornamental top border

### Hero
- Full viewport, centered layout (not split grid — more editorial)
- Large serif name with character stagger animation
- Typewriter subtitle beneath
- Ornamental flourish SVG below subtitle
- Photo in an ornate circular frame with gold gradient border and subtle paper texture
- CTA buttons: gold fill primary, outlined secondary with gold border
- Social links as small gold-tinted icons
- Scroll indicator with ornamental arrow

### About
- Clean editorial single-column layout
- Section heading with scramble-in effect
- Decorative initial cap (drop cap) on first paragraph
- Warm cream text on dark background
- Coursework as small refined tags with gold accents

### Experience
- Vertical timeline with ornamental gold line (not plain gradient)
- Small decorative diamond markers at each position
- Cards with subtle paper texture overlay
- Tech tags in monospace font with vintage label styling

### Projects
- Magazine-style grid with varying card sizes
- Featured project gets a larger "editorial spread" layout
- Cards have decorative corner brackets
- Hover: card lifts with warm gold glow and subtle tilt
- Project images with subtle vignette overlay
- Badge annotations in handwriting-style font

### Skills
- Organized in columns with ornamental category headers
- Skill chips styled as vintage brass labels
- Subtle shimmer animation on hover

### Education
- Cards with ornamental top border (gold filigree pattern)
- Decorative cap/gown icon in vintage line-art style
- Quote section styled as a pulled editorial quote with large decorative quotation marks

### Contact
- Centered editorial layout
- Contact cards with ornamental left border
- Email/LinkedIn/GitHub as refined link cards with gold hover accents
- Decorative closing ornament

### Footer
- Minimal with ornamental divider
- Social icons in warm gold
- Copyright in small serif italic

---

## Technical Implementation

- **Single HTML file** (GitHub Pages compatible)
- **Tailwind CDN** for utility classes
- **Google Fonts** for Cormorant Garamond, DM Sans, JetBrains Mono
- **Pure CSS animations** for reveals, staggers, typewriter, shimmer
- **Vanilla JS** for: cursor effects, scroll spy, text scramble, intersection observer reveals, typewriter engine
- **SVG ornaments** inline for decorative elements
- **No build step required** — ships as static HTML

---

## Key Differentiators from Current Site

| Current                          | Redesign                                    |
|----------------------------------|---------------------------------------------|
| Purple/blue gradient palette     | Warm gold/cream on deep warm black           |
| Syne + Outfit (modern sans)     | Cormorant Garamond serif + DM Sans           |
| Plain `<hr>` dividers           | Ornamental SVG flourishes                    |
| Standard fade-up reveals        | Text scramble, character stagger, typewriter  |
| Uniform card grid               | Editorial magazine-style layout               |
| Generic tech aesthetic           | Vintage atelier meets digital craft           |

---

*This redesign signals: "A human made this with care." The vintage craft aesthetic is deliberate — it's the antithesis of algorithmic, cookie-cutter portfolio sites.*
