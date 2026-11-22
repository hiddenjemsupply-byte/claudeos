# Field Xerox: Design System

> Photocopied paper, faded film, heavy lowercase type, and photos cropped into square stair-steps. Quiet captions sit at the edges.

Derived from a reference poster that reads "nature is beatiful" (sic). This system uses the correct spelling.

---

## 1. Principles

1. **Shout or whisper.** Type is either huge (display) or tiny (caption and micro). Nothing goes in between.
2. **Color comes from photography.** The page is paper and ink, and all hue lives inside the photos.
3. **Nothing is a clean rectangle.** Every photo has stepped, pixel-notched corners.
4. **Everything is copied.** Grain, ink bleed, and slight softness apply to every layer, type included.
5. **Text is found, not written.** Captions read like fragments torn from a longer page and often break off mid-sentence.

---

## 2. Color

### Paper & ink (UI and type)

| Token | Hex | Use |
|---|---|---|
| `--paper` | `#F2F1EC` | Canvas, caption plates |
| `--paper-shade` | `#E4E2D9` | Code blocks, secondary surfaces |
| `--paper-fold` | `#D6D3C8` | Dividers, hairlines |
| `--pencil` | `#9A988F` | Disabled, "don't" markers |
| `--graphite` | `#5F5E59` | Micro text, labels |
| `--ink-soft` | `#2A2A28` | Captions |
| `--ink` | `#151515` | Display type, ornaments, rules |

### Film (photo tints, placeholders, rare accents only)

| Token | Hex | Reads as |
|---|---|---|
| `--haze` | `#A3B5B6` | Overcast sky |
| `--stone` | `#C2B98F` | Sunlit granite |
| `--cliff` | `#A7A07A` | Rock face in shadow |
| `--meadow` | `#7D8C4E` | Grass |
| `--sweater` | `#5B7A57` | Knit green |
| `--moss` | `#56653A` | Mid-forest |
| `--pine` | `#34482F` | Deep conifers |
| `--earth` | `#6A4B33` | Boots, bark |

**Rules**
- Type is always `--ink`, `--ink-soft`, or `--graphite`. Never set type in a film color.
- Photo treatment: `saturate(.72) contrast(.92) sepia(.12)`, plus a light grain layer on top (screen blend, ~55%).

---

## 3. Typography

**Family:** neo-grotesk. Use `"Helvetica Neue", Helvetica, Arial, sans-serif`.
Alternates: Neue Haas Grotesk Display, Inter Tight 800, Archivo 800.

| Role | Weight | Size | Line height | Tracking | Notes |
|---|---|---|---|---|---|
| Display | 800 | `clamp(64px, 11vw, 148px)`; posters use 15–19% of canvas width | .86 | −0.045em | lowercase, ink-bleed filter |
| H1 | 800 | 56px | .9 | −0.04em | lowercase, ink-bleed |
| H2 | 700 | 32px | 1 | −0.03em | lowercase |
| Body | 400 | 15px | 1.4 | 0 | docs and UI only, never on posters |
| Caption | 500 | 11px (~2.2% of poster width) | 1.12 | −0.01em | max ~22ch, flush left, ragged right |
| Micro | 500 | 7.5px (~1.4% of poster width) | 1.15 | 0 | `--graphite`; texture, not for reading |
| Label | 600 | 10px | — | +0.14em | UPPERCASE, docs only |

**Rules**
- Display is always lowercase, one word per line, and steps down and across the page.
- On posters, avoid sizes between ~18px and ~40px.
- Never center text.

---

## 4. Space & grid

- **Base grid:** 8pt. Tokens: `--s1 4`, `--s2 8`, `--s3 16`, `--s4 24`, `--s5 40`, `--s6 64`, `--s7 104`.
- **Step unit** (`--step`): the size of one notch in a crop. Default 28px; on a 9:16 poster, ~2.5% of width (18–22px at 420px wide). Every notch is 1×, 2×, or 3× step.
- **Composition grid:** 12 columns, no gutters. Elements snap to column edges and overlap freely.
- **Negative space:** keep 30–40% of the canvas as bare paper.

---

## 5. Components

### 5.1 Stepped crop (signature)
A photo container clipped with `clip-path: polygon(...)` so its corners notch out in square stair-steps.

| Class | Shape |
|---|---|
| `.step-a` | Top-left notch (2×1 step), bottom-right notch (1×2 step) |
| `.step-b` | Left-side ladder plus a bottom-left bite |
| `.step-c` | Top-right shelf, bottom-left 1×1 |
| `.step-d` | Plus/cross: all four corners notched |

```html
<div class="photo step-a" style="--step:24px">
  <img src="meadow.jpg" alt="">
</div>
```

Display words and caption plates sit inside the notches, so the crop and the type interlock.

### 5.2 Caption plate
A paper-colored block with 8px padding (4px at poster scale) that overlaps a photo edge. It holds one caption-size fragment.

### 5.3 Sparkle
A four-point star with concave sides (SVG path below). Three sizes: 34 / 22 / 13px. Use 3–5 per composition, always on bare paper.

```svg
<path d="M12 0 C12.6 7.6 16.4 11.4 24 12 C16.4 12.6 12.6 16.4 12 24
         C11.4 16.4 7.6 12.6 0 12 C7.6 11.4 11.4 7.6 12 0Z"/>
```

### 5.4 Crosshair
Hairline registration mark: 1px `--ink` at 75% opacity. The vertical arm is longer than the horizontal (≈ 2:1), and the crossbar sits ~42% down. Use 1–2 per composition.

---

## 6. Texture & effects

**Paper grain:** fixed full-page overlay, SVG `feTurbulence` (fractalNoise, baseFrequency .9, 3 octaves), multiply blend, ~20% opacity.

**Ink bleed (display type):**
```svg
<filter id="ink-bleed">
  <feTurbulence type="fractalNoise" baseFrequency=".85" numOctaves="2" seed="4" result="noise"/>
  <feDisplacementMap in="SourceGraphic" in2="noise" scale="3.2" xChannelSelector="R" yChannelSelector="G" result="rough"/>
  <feGaussianBlur in="rough" stdDeviation=".7" result="soft"/>
  <feMerge><feMergeNode in="soft"/><feMergeNode in="rough"/></feMerge>
</filter>
```

**Ink soft (captions, ornaments):** same idea at displacement scale 1.1 and blur .25.

**Never:** drop shadows, rounded corners, glossy gradients, or glass/blur UI.

---

## 7. Composition recipe (9:16 poster)

1. **Word 1** (display) top-left, slightly hanging off the margin.
2. **Crop 1** below and right of it, using its top-left notch to tuck under word 1.
3. **Word 2** sits in the right-hand notch of crop 1.
4. **Word 3** spans left, overlapping the bottom of crop 1.
5. **Crops 2 and 3** cascade diagonally toward the bottom-right, and the largest can bleed off the right edge.
6. **Captions:** one at top-right beside word 1, then 2–4 plates in the gaps between crops, plus one micro block near the bottom.
7. **Ornaments:** 3–5 sparkles and 1–2 crosshairs in leftover paper.
8. Add grain over everything.

---

## 8. Do / Don't

| Do | Don't |
|---|---|
| Keep an extreme scale gap (display ≈ 16% of width, caption ≈ 2%) | Use mid-size type on posters |
| Tuck words into crop notches | Show photos as clean rectangles |
| Desaturate and warm every photo | Set type in film colors |
| Grain everything, including type | Use rounded corners, shadows, or gradients on UI |
| Leave 30–40% bare paper | Center anything |
| Crop captions mid-sentence | Use uppercase display type |

---

## 9. CSS token block

```css
:root{
  --paper:#F2F1EC; --paper-shade:#E4E2D9; --paper-fold:#D6D3C8;
  --ink:#151515; --ink-soft:#2A2A28; --graphite:#5F5E59; --pencil:#9A988F;
  --haze:#A3B5B6; --stone:#C2B98F; --cliff:#A7A07A; --meadow:#7D8C4E;
  --sweater:#5B7A57; --moss:#56653A; --pine:#34482F; --earth:#6A4B33;

  --font:"Helvetica Neue",Helvetica,Arial,sans-serif;
  --fs-display:clamp(64px,11vw,148px); --fs-h1:56px; --fs-h2:32px;
  --fs-body:15px; --fs-caption:11px; --fs-micro:7.5px;
  --lh-display:.86; --lh-caption:1.12;
  --tr-display:-0.045em; --tr-caption:-0.01em;

  --s1:4px; --s2:8px; --s3:16px; --s4:24px; --s5:40px; --s6:64px; --s7:104px;
  --step:28px;
}
```

See `design-system.html` for live tokens, the four crop masks, the ornaments, and two worked poster templates.
