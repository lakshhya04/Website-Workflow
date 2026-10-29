## Typography

Values marked (computed CSS) were read from the live site's computed styles and are authoritative. Everything else was estimated from the original 3420×20552 capture, read at 1710 px wide. That capture is assumed to be a 2x screenshot of a 1710 px viewport (inferred), so 1 px at that width = 1 CSS px. The computed h2 (72px) and lead (28px) sit close to my capture estimates, which supports that assumption. The h1 does not (see below).

- **Font families**
  - Display / headline: "Feature Display Condensed", a condensed serif (computed CSS). Used for headlines, the lead paragraph, feature lists and review quotes.
  - Body / UI: "forma-djr-micro", a grotesque sans (computed CSS).
  - Heavy extended grotesque (HEIST wordmark, product names, "SHOP NOW", "CART(0)", "FOLLOW @DRINKHEIST"): ultra-black, wide letterforms. The wordmark is a logo, so treat it as an image, not type (inferred). The computed family for button and product-name text was not supplied.
  - Mono (nav, labels, chart axis, meta lines, tabs, review fields): uppercase, regular weight. A Roboto Mono / Space Mono class face, not identifiable more closely (inferred).
- **Size scale, smallest to largest**
  - ~11 px: footer fine print, bag-label microcopy (approx).
  - ~13 px: mono nav, tab and meta labels, chart row labels, review fields (approx).
  - ~16 px: sans paragraph (approx).
  - 28 px: lead paragraph (computed CSS).
  - ~50 px: feature-list lines, review quotes, product roast names ("Medium Roast") (approx).
  - 72 px: h2, the section headlines (computed CSS).
  - 96 px: hero h1 (computed CSS).
  - HEIST wordmark: cap height ~236 px in the capture. Treat as a logo, not a type size (approx).
  - Discrepancy: my capture estimate for the "Coffee Without a Curfew." line was ~170 px, against the computed 96px. Either that line is not the h1, or the h1 size depends on viewport width and the capture was taken at a different width. Not resolved; build from 96px.
- **Ratio between steps:** h1 to h2 is 96 / 72 = 1.33. Lead to h2 is 72 / 28 ≈ 2.57. No consistent modular scale across the rest (inferred).
- **Line height:** h1 and h2 ~1.04 (computed CSS). Lead ~1.1 (approx, 36 px pitch measured at the capture). Body sans ~1.3 (approx, 20.5 px pitch at ~16 px).
- **Letter spacing**
  - h1, h2 and lead paragraph: -0.02em (computed CSS).
  - Body sans: not distinguishable from 0 (inferred).
  - Mono small-caps labels: slightly open, roughly +0.04em to +0.08em (inferred).
  - Heavy extended grotesque: not measurable at this size.
- **Weights**
  - Display serif: 400 on h1, h2 and lead (computed CSS). Hierarchy comes from size, not weight.
  - Heavy grotesque: black, only on buttons, product names, cart and the wordmark (approx, from the capture).
  - Mono: regular only (approx).
  - Body sans: regular only (approx).

## Spacing

- **Base unit:** 8 px (inferred). Evidence: card gutters are 16 px (receipt cards 376→392, product cards 847→863), the page margin is ~56 px (57→1653 at 1710 wide, within 1 px of 7×8), chart row pitch is ~48 px, receipt card inner padding is ~24 px. No measurement points to 4 px.
- **Vertical gap between sections**
  - Desktop: ~112–128 px of padding top and bottom (approx). Examples: receipts card bottom → next section edge ~115 px; next section edge → headline cap ~130 px; banner/hero edge → "World-Class" headline ~125 px.
  - Mobile: not shown in this capture. Not inferred.
- **Padding inside cards and buttons**
  - Receipt card: ~24 px inner padding, plus a cream mat ~12 px between the outer border and the photo or text block.
  - "SHOP NOW" hero button: ~48 px tall, ~318 px wide at this layout. Horizontal padding not separable from its width.
  - Nav "SHOP NOW" button: ~43 px tall, ~142 px wide.
  - Chart tabs: ~54 px tall, ~24 px left padding.
- **Max content width and measure**
  - Content is full-bleed with ~57 px margins and ran 57→1653 (1596 px) at 1710 wide. Whether it is capped at wider viewports is not visible.
  - Body measure: ~56 characters on the widest line ("We picked the top seller from the most Awarded Roasters."), ~400 px wide. The paragraph is centred in three lines, so the breaks may be manual (inferred).

## Colour

Rows marked (computed CSS) are authoritative and override my earlier pixel samples. Pixel samples from the original PNG are supporting values only: backgrounds carry a film-grain texture, so each is a single point inside noise (approx).

| Role | Hex | Basis |
|---|---|---|
| bg | #DDD6C7 | computed CSS (my pixel sample read #d1cabc on the grained page, approx) |
| surface | #eeeade | approx (pixel sample of the chart panel; review cards look the same) |
| surface-sunken | #ddd6c8 | approx (inactive tab; visually the same as bg, not separately confirmed) |
| border | #161414 | computed CSS (button border; card borders look the same, approx) |
| border-strong | #161414 | approx (no heavier border visible) |
| text | #161414 | computed CSS |
| text-muted | not filled | |
| text-faint | not filled | |
| accent | #FF3B27 | computed CSS, used on buttons and actions only |
| accent-hover | not filled | |
| accent-contrast | #161414 | computed CSS (button text) |
| focus | not filled | |

Supporting values (pixel samples, approx):
- Cream text and wordmark on dark/blue: #ddd6c8. This matches the computed bg to within one unit, so it is probably the same colour.
- Hero blue: #2b73f5 at mid-height of the gradient.
- Chart highlight bar: #4589e8.
- Chart comparison bars: #c5bca9.
- Dark section: #181214, close to the computed text colour #161414.

Note: the capture also shows the accent as the top banner and the footer fill, not just on buttons. The computed-CSS note says buttons and actions only, so treat the banner and footer fill as a separate use I observed, not part of the rule.

The hero gradient runs from near-black navy at the top to saturated blue and back to dark. The sections after it fade blue → dark → warm orange → beige (approx, from the capture). Exact stops can't be sampled reliably in one pass.

## Shape and depth

- **Buttons (computed CSS):** background #FF3B27, text #161414, border 2px solid #161414, border-radius 2px. Hard edges, no shadow.
- **Border radius, other components:** 0 on cards, tabs, images, chart bars and product tiles (approx, from the capture). Exceptions are all small or likely third-party:
  - The chat bubble and the video mute buttons are circles.
  - The "AUG 2026" chip and the Light Labs badge have a small radius, roughly 4 px (approx).
- **Border widths and colours:** #161414 (computed CSS on buttons; the rest approx).
  - Buttons: 2px (computed CSS).
  - Cards, product tiles and chart bars: ~2 px (approx).
  - Receipt cards: ~3 px outer border, a cream mat, then a ~2 px border on the photo inside.
  - Horizontal rules between feature-list items: ~2 px.
  - The red box around the bean image is #ff3c26-family, 2 px, and is an overlay, not a component (inferred).
- **Shadows:** none on buttons (computed CSS). None on any of the page's other own components either (approx, from the capture). The one exception is the Light Labs badge, which has a faint soft shadow, written as `0 1px 3px rgba(0, 0, 0, 0.2)` (inferred). It is probably a third-party widget, so I would not count it as part of the site's system.

## Motion

A static capture shows no motion. Everything below is inference from layout, not observation.

- **What probably animates (inferred):**
  - Rows of review cards, brewing-guide tiles and the Instagram strip are cropped at the right and left edges, which implies horizontal scrolling or dragging.
  - Video tiles have mute toggles, so they autoplay.
  - The chart bars are likely drawn in on view.
  - The bean image is split into two offset halves, which suggests a scroll-linked or glitch effect.
- **What does not animate:** I can't tell. Nothing visible rules motion out for the static elements.
- **Durations and easing:** not determinable. No values given.
- **Scroll-driven:** possibly the bean split and the chart bars. Not confirmed.

## Rules

1. Set every headline in one condensed serif at weight 400, and let size carry the hierarchy (h1 96px, h2 72px, lead 28px).
2. Use line-height about 1.04 and letter-spacing -0.02em on headlines and the lead.
3. Use uppercase mono, small and slightly letterspaced, for every label, nav item and metadata line.
4. Reserve the ultra-heavy extended grotesque for the wordmark, buttons and product names. Do not use it for body or headings.
5. Keep corners hard: 2px on buttons, 0 on everything else. Round only things that are functionally circular, such as media controls.
6. Draw every container with a 2 px #161414 border and no shadow.
7. Run content edge to edge with equal ~56 px side margins and 16 px gaps between tiles.
8. Pad sections by ~120 px top and bottom and put one idea in each.
9. Alternate warm beige sections with full-bleed saturated or dark gradient sections, and add grain over all of them.
10. Use one hot orange-red (#FF3B27) for buttons and actions only, and keep every other colour muted or photographic.

## Do not copy

1. The HEIST wordmark, the globe-and-bean seal, and the stamp-like legal lines ("© MCMLMMXXV", "HEIST GLOBAL, INC."). They are their brand identity.
2. The saturated blue/orange duotone product photography and the per-product colour worlds (yellow for Smooth Talker, blue for Blueprint). They come from their packaging and would look wrong on a site without that product.
3. The heist and receipt conceit: the barcode review cards, "30-day escape plan", and "the receipts don't lie". The motif only works for their product and tone.
