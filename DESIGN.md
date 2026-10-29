---
name: Vesper
description: Decaf, done properly. Ink on oat, one hot-red action, serif headlines.
colors:
  oat-canvas: "#DDD6C7"
  ink: "#161414"
  ink-muted: "#5A544A"
  hairline: "#C3BAA8"
  hot-red: "#FF3B27"
  hot-red-pressed: "#E63320"
  focus-blue: "#2B73F5"
typography:
  display:
    fontFamily: "DM Serif Display, Times New Roman, serif"
    fontSize: "4rem"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.032em"
  headline:
    fontFamily: "DM Serif Display, Times New Roman, serif"
    fontSize: "2.0625rem"
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: "-0.018em"
  lead:
    fontFamily: "Hanken Grotesk, system-ui, -apple-system, sans-serif"
    fontSize: "1.3125rem"
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: "0em"
  body:
    fontFamily: "Hanken Grotesk, system-ui, -apple-system, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: "0em"
  button:
    fontFamily: "Hanken Grotesk, system-ui, -apple-system, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: "0em"
  caption:
    fontFamily: "Hanken Grotesk, system-ui, -apple-system, sans-serif"
    fontSize: "0.875rem"
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: "0em"
rounded:
  sm: "6px"
spacing:
  xs: "12px"
  sm: "16px"
  md: "24px"
  lg: "32px"
  xl: "64px"
  section: "128px"
  hero: "192px"
components:
  button-primary:
    backgroundColor: "{colors.hot-red}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "12px 24px"
  button-primary-hover:
    backgroundColor: "{colors.hot-red-pressed}"
---

# Design System: Vesper

## Overview

**Creative North Star: "The Dusk Counter"**

A shop counter at closing time: warm oat light, ink-dark type, and one bold red sign on the counter that says where to act. The page is confident, editorial and calm. Headlines are set large in a display serif and left-aligned, the copy that follows is plain, and almost everything else is air.

Colour is rationed. The oat canvas, ink text and hairlines carry the whole page, and the single hot red appears only on the action. Structure comes from spacing and thin rules, not from boxes, shadows or ornament.

**Key Characteristics:**
- Left-aligned, type-led layout on one shared edge.
- One accent, used for the action only.
- Hairline rules divide sections and list rows, and there are no shadows at rest.
- A strong size step between display headlines and body copy, with a single weight on the headings.
- Generous, scale-based vertical space: 128px between desktop sections, 64px on mobile.

## Colors

A warm neutral palette with a single saturated signal.

### Primary
- **Hot Red** (#FF3B27): the action colour, used on the primary button and nowhere else. Text on it is ink, never white.
- **Hot Red Pressed** (#E63320): the button's hover state.

### Neutral
- **Oat Canvas** (#DDD6C7): the page background and the page's only large surface.
- **Ink** (#161414): headings, body text, link text, and the hard border around the button.
- **Ink Muted** (#5A544A): the lead paragraph and footer tagline, text that supports and doesn't lead.
- **Hairline** (#C3BAA8): 1px rules between sections, proof rows and above the footer.
- **Focus Blue** (#2B73F5): the keyboard focus ring only.

### Named Rules
**The One Signal Rule.** Hot red marks an action and nothing else. A heading, rule, icon or background is never red.

**The Ink-on-Red Rule.** Text on the accent is ink (#161414), not white.

Note: the dark-mode block in `design/tokens.css` still holds the earlier green palette and has not been redesigned for Vesper, so there is no confirmed dark theme.

## Typography

**Display Font:** DM Serif Display (with Times New Roman, serif)
**Body Font:** Hanken Grotesk (with system-ui, sans-serif)

**Character:** A heavy, high-contrast serif for statements set against a quiet, neutral grotesque for everything the visitor has to read or click. DM Serif Display ships in one weight, so headlines never use bold.

### Hierarchy
- **Display** (400, 4rem / 64px on desktop and 2.5625rem / 41px on mobile, line-height 1.02, tracking -0.032em): the single hero headline. Only one element on the page uses the top size.
- **Headline** (400, 2.0625rem / 33px on desktop and 1.625rem / 26px on mobile, line-height 1.15, tracking -0.018em): section headings.
- **Lead** (400, 1.3125rem / 21px, line-height 1.3, Ink Muted): the paragraph under the hero headline, capped at 68ch.
- **Body** (400, 1.0625rem / 17px, line-height 1.55): proof points and running copy, capped at 68ch.
- **Button label** (500, 1.0625rem / 17px, line-height 1.15): the one place a heavier weight appears.
- **Caption** (400, 0.875rem / 14px): the footer line and links.

### Named Rules
**The Two-Weight Rule.** Only 400 and 500 appear on a screen. Hierarchy comes from size, not weight.

**The Tight Display Rule.** Large type always carries negative tracking, and the larger the type, the tighter it sits.

## Layout

A single left-aligned column inside a 1180px container with 24px side gutters. Every block shares the same left edge. Sections are separated by a 1px hairline and padded on both sides of it: 128px on desktop, 64px on mobile. The hero is the one exception, with 192px above it on desktop. Body copy and the proof list are capped at 68ch.

The only breakpoint is 48em. Below it the hero headline steps down to 41px and the section headline to 26px, and spacing drops to the 64px step. The footer wraps its links under the tagline when there is no room.

Spacing uses a 4px base on an 8px rhythm, taken from the tokens: 12, 16, 24, 32, 64, 128 and 192px are the steps in use.

## Elevation & Depth

Flat. The page uses no shadows at rest; depth is conveyed only by hairline rules and by the hard ink border on the button. Shadow tokens exist in `design/tokens.css` for floating elements, but nothing on this page floats.

### Named Rules
**The Borders-Before-Shadows Rule.** Separate things with a rule or a border. A shadow is reserved for something floating over the page.

## Shapes

Squared-off and plain. The button takes a small 6px radius with a heavy 2px ink border. Everything else is rectangular, separated by 1px hairlines. There are no pills, no large radii and no decorative shapes.

## Components

Refined and restrained. The accent is kept for the action, and every other component is quiet.

### Buttons
- **Shape:** gently squared (6px radius) with a 2px solid ink border.
- **Primary:** Hot Red (#FF3B27) background, Ink label at 500 weight, padding 12px 24px.
- **Hover / Focus:** background shifts to Hot Red Pressed (#E63320) over 120ms. Keyboard focus draws a 2px Focus Blue ring offset by 2px.

### Proof list
- **Style:** rows of plain body copy, each topped by a 1px hairline, with 16px vertical padding. No bullets, icons or cards.

### Navigation
- **Style:** the footer holds a caption-size tagline on the left and three plain text links on the right, with 24px between them. Links are Ink and fade to Ink Muted on hover over 120ms; keyboard focus uses the same Focus Blue ring as the button. There is no header navigation.

## Do's and Don'ts

### Do:
- **Do** use Hot Red (#FF3B27) only for the primary action, with Ink (#161414) text on it.
- **Do** keep every block on one left edge and cap running copy at 68ch.
- **Do** set the hero at the display size and let nothing else on the page use it.
- **Do** space sections with the 128px desktop and 64px mobile steps, and nothing in between.
- **Do** separate content with 1px Hairline (#C3BAA8) rules.

### Don't:
- **Don't** use more than the 400 and 500 weights on one screen.
- **Don't** add shadows to anything that isn't floating over the page.
- **Don't** use gradients, emoji icons or three-column icon-card grids.
- **Don't** use a radius above 16px on anything except a pill button or an avatar.
- **Don't** centre-align body copy longer than two lines.
- **Don't** colour a heading with the accent.
