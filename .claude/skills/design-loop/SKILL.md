---
name: design-loop
description: Screenshot the running app with Playwright, score it against design/references and design/tokens.css, fix the single worst category, and repeat. Use when asked to polish, audit, or improve how a page looks.
---

Run a design loop on the URL I give you (default http://localhost:3000) until it passes or you hit 5 rounds.

Setup, once:
- Read design/TASTE.md and design/tokens.css.
- Open the reference images in design/references/ and any *-DESIGN.md there. These are the standard. We match their discipline, not their brand or copy.

Each round:
1. Use the Playwright MCP to navigate to the page. Screenshot at 1440x900 and at 390x844. Save to design/screenshots/round-N-desktop.png and -mobile.png.
2. Open both screenshots and look at them.
3. Score the build out of 5 on each of these, with one specific sentence of evidence per score. No score without evidence.
   - Type: is there a real hierarchy, or sizes that are all nearly the same?
   - Rhythm: are vertical gaps on the scale, and is section spacing consistent?
   - Density: is there enough air, and is it distributed or all in one place?
   - Restraint: how many colours, weights, radii and shadow levels are in play?
   - Alignment: does everything sit on a shared grid, or is it close-but-not?
   - Focus: is there exactly one primary action visible?
4. Take the single lowest score. Fix only that. Say what you are changing and what token value you are changing it to before you edit.
5. Re-screenshot and re-score. If the score did not move, revert the change and try a different fix. Do not stack failed fixes.

Stop when every category is 4 or higher, or after 5 rounds. Then print a table of round-by-round scores.

Do not add features. Do not add sections. Do not add copy. This loop only changes type, space, colour and shape.
