# ICT Pathfinder — Brand & Web Style Guide

Version 0.1 · 23 October 2026

## Brand foundation

**Name:** ICT Pathfinder  
**Tagline:** Architecture, services & automation  
**Audience line:** for Higher Education Institutions and Alliances

ICT Pathfinder connects enterprise architecture, IT service management, configuration data, and automation for higher education. Its visual identity expresses direction, connected systems, and institutional collaboration.

Write clearly and confidently. Use concrete language that works for university leadership, IT teams, and architects. Keep all public brand and interface copy in English. Avoid suggesting that the project is officially endorsed by another organisation.

## Colour palette

| Colour | HEX | RGB | Role |
| --- | --- | --- | --- |
| Pathfinder Deep Blue | `#2E307C` | 46, 48, 124 | Wordmark, headings, navigation, primary buttons, structural icons |
| Pathfinder Cyan | `#0099D2` | 0, 153, 210 | Navigation arrow, connections, waypoints, selected accents |
| White | `#FFFFFF` | 255, 255, 255 | Main canvas and reversed text on deep blue |
| Canvas | `#F3F7FC` | 243, 247, 252 | Proposed secondary page and section background |
| Ink | `#202644` | 32, 38, 68 | Proposed body text |
| Muted | `#586580` | 88, 101, 128 | Proposed secondary text |
| Border | `#DCE3EF` | 220, 227, 239 | Proposed dividers and component boundaries |

Deep Blue follows the [GÉANT June 2026 colour specification](https://resources.geant.org/wp-content/uploads/2026/06/GEANT-branding-guidelines-2026-1.pdf). Cyan references the [Digitalverbund Bayern website](https://digitalverbund.bayern/). Supporting neutrals are project choices.

Use white and light surfaces generously, deep blue for structure, and cyan selectively. Keep the logo in its two established colours.

### Readability

- Deep Blue on white has approximately **11.48:1** contrast; use it for headings, links, and text.
- White on Deep Blue is suitable for primary button labels.
- Cyan on white has approximately **3.24:1** contrast. Reserve it for graphical accents and larger visual elements; use Deep Blue for small text.
- Muted on white has approximately **5.85:1** contrast.
- Indicate status and selection with text, icons, or shape as well as colour. Check contrast when introducing new combinations.

## Logo and symbols

**Master asset:** [ict-pathfinder-logo.svg](ict-pathfinder-logo.svg)

The SVG has a transparent background and outlined lettering; no font installation is required.

| Element | Meaning |
| --- | --- |
| Central navigation arrow | Direction, decisions, and progress |
| Connected routes and waypoints | Dependencies, services, and institutional complexity |
| Graduation cap | Higher education and academic achievement |
| University main building | Institutions and governance |
| Server rack | ICT infrastructure and operations |
| Diploma | Educational outcomes and qualifications |

Preserve proportions, symbol positions, wording, and colours. Keep clear space around the logo of at least half the height of the graduation cap. Place the current asset on white or a very light, uncluttered background.

As an initial web guideline, display the complete three-line logo at **640 CSS pixels or wider**. Verify readability at the actual size. For narrower layouts, prepare a dedicated compact or symbol-only asset rather than shrinking all three lines. Compact, monochrome, and reversed variants are not yet supplied.

Do not stretch, rotate, add shadows, recolour individual symbols, or place the logo on photography. Keep any future compact version recognisably related to the master.

## Typography

Use a system sans-serif stack for web content:

```css
font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
```

Keep the supplied wordmark artwork intact; the web font does not replace it.

- Body: 16–18 px, regular, line height 1.5–1.65.
- Headings: deep blue, weight 600–700, line height 1.15–1.3.
- Labels and metadata: 14–16 px; avoid long uppercase passages.
- Prose width: approximately 65–75 characters per line.

## Website and interface elements

- **Layout:** generous whitespace, consistent alignment, and an 8 px spacing rhythm: 8, 16, 24, 32, 48, 64.
- **Navigation:** deep blue text on white; mark the current page with an underline or indicator and accessible current-page semantics.
- **Primary buttons:** deep blue with white text; short action labels such as “Explore the platform”.
- **Secondary buttons:** white with deep blue text and outline.
- **Links:** deep blue and underlined within prose.
- **Cards:** white on Canvas, subtle borders, 8 px corners, minimal shadows.
- **Forms:** visible labels, clear borders, helpful error text, and persistent keyboard focus indicators.
- **Icons:** simple, consistent line icons. Use server and network imagery for IT capabilities; academic imagery for institutional context.
- **Diagrams:** deep blue for structure, cyan for paths and emphasis. Label relationships and use a legend where needed.
- **Motion:** brief and purposeful; respect reduced-motion preferences.

Avoid decorative network clutter behind text, excessive gradients, and colour-only status indicators.

## Starter CSS tokens

```css
:root {
  --brand-deep-blue: #2E307C;
  --brand-cyan: #0099D2;
  --surface: #FFFFFF;
  --canvas: #F3F7FC;
  --text: #202644;
  --text-muted: #586580;
  --border: #DCE3EF;
  --radius: 0.5rem;
  --space-unit: 0.5rem;
  --font-sans: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
}
```

This is the initial identity baseline. Validate small-size logo legibility and component accessibility as the website takes shape.
