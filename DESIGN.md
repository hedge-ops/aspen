<!-- SEED: re-run /impeccable document once there's code to capture the actual tokens and components. -->
---
name: Aspen
description: Quiet alpine luxury for tending the relationships that grow your career.
---

# Design System: Aspen

## 1. Overview

**Creative North Star: "The Cashmere Lodge"**

You step in from the cold and the room is already warm. Low light, wool and
sheepskin, pale wood, a single living thing in green on the mantel. Nobody is
selling you anything; you are simply welcomed. Aspen's surface is that room —
a restrained, almost entirely neutral palette of warm naturals, set in a serif
that carries quiet confidence and a clean sans that gets out of the way. The
name is the brief: Aspen the alpine resort, not aspen the tree. Luxury is shown
through material, space, and restraint, never through volume.

This system is **restrained by doctrine**. Color is carried by warm neutrals —
the tones of wool, sheepskin, undyed linen, pale wood — with one faint touch of
sage green used so sparingly it reads as a single sprig, not a theme. Motion is
smooth and calm: gentle fades and unhurried transitions, never choreography that
demands attention. The references are hospitality and lighting at their most
pared-back: The Little Nell *with the photography stripped away* (so warmth and
luxury must come from type, space, and tone alone), Patrizia Garganti *smaller
and more minimal*, and impeccable.style *in its early restraint, before the
clutter*.

It explicitly rejects everything pressured, hurried, busy, or loud — and the
whole loud HR/people-ops SaaS category (Lattice, Workday) that the strategic
brief names as the anti-reference. If a section raises its voice, it is wrong.

**Key Characteristics:**
- Warm, almost-monochrome neutral palette; sage is a whisper, not a wash
- Serif display + clean sans body; confidence through type, not decoration
- Generous space and soft contrast — the page lowers your heart rate
- Smooth, calm motion; nothing that hurries or demands
- Luxury read through material and restraint, never volume

## 2. Colors

A warm neutral palette in the register of wool, sheepskin, undyed linen, and
pale wood — almost monochrome, with a single faint sage accent. `[All hex / OKLCH
values to be resolved during implementation; the palette script seeds the anchor.]`

### Primary
- **Sage Whisper** `[to be resolved]`: The one living touch of green — a soft,
  desaturated sage. Used like a single sprig on a mantel: a small mark, a hover
  state, a focus ring. Never a fill, never a wash. Its rarity is the point.

### Neutral
- **Sheepskin** `[to be resolved]`: The warm near-white body background — the
  wool-and-pale-wood base the whole room is built on. Warmth comes from a faint
  natural tint, not from saturation.
- **Undyed Linen** `[to be resolved]`: A slightly deeper warm neutral for
  alternating sections and quiet surfaces, so rhythm comes from tone, not borders.
- **Driftwood** `[to be resolved]`: Muted mid-tone warm gray for secondary text
  and soft dividers.
- **Espresso Ink** `[to be resolved]`: The dark warm near-black for body and
  headings. Pushed dark enough to clear WCAG AA against the neutral grounds —
  elegant must never mean faint.

### Named Rules
**The Single Sprig Rule.** Sage appears on ≤5% of any screen. It is a touch, not
a theme. If green reads as a color scheme rather than a single living accent,
remove most of it.

**The Warm-By-Tone Rule.** Warmth is carried by the neutrals themselves, not by a
warm-tinted near-white standing in for cream. No paper/parchment/biscuit body
washes — the AI warm-neutral default is forbidden here.

## 3. Typography

**Display Font:** A serif with quiet confidence `[family to be chosen at
implementation]` (think editorial restraint, generous in the large sizes).
**Body Font:** A clean, neutral sans `[family to be chosen at implementation]`
that recedes and lets the prose breathe.

**Character:** Serif display sets the tone — composed, hospitable, assured, like
signage in a good hotel. The sans body does the quiet work of reading. The pair
contrasts on a real axis (serif vs. sans), never two near-identical sans faces.

### Hierarchy
- **Display** (serif, light–regular, clamp max ≤ 6rem, tight but ≥ -0.04em
  tracking): Hero headline only. One per page. `[exact scale at implementation]`
- **Headline** (serif): Section openers — calm, not shouting.
- **Title** (sans, medium): Feature and step headings.
- **Body** (sans, regular, line length capped 65–75ch): The reading voice.
- **Label** (sans, medium): Buttons, nav, small UI text. No tracked all-caps
  eyebrows.

### Named Rules
**The No-Eyebrow Rule.** No tiny tracked-uppercase kicker above every section.
The serif headline carries the section on its own.

## 4. Elevation

Flat by doctrine. Depth comes from warm tonal layering — Sheepskin against Undyed
Linen — not from drop shadows. Where lift is genuinely needed (a resting CTA, a
hover), it is a single soft, diffuse, warm-tinted shadow, never a hard gray box.
`[exact shadow values at implementation.]`

### Named Rules
**The Flat-Lodge Rule.** Surfaces are flat at rest. If a card looks like it's
floating in a 2014 app, the shadow is too dark and the blur too tight — soften it
or remove it.

## 5. Components

`[No components yet — this is a seed. The redesign will synthesize buttons,
nav, and section primitives from the tokens above, then a scan-mode re-run of
/impeccable document will capture them and generate the .impeccable/design.json
sidecar.]`

## 6. Do's and Don'ts

### Do:
- **Do** keep the palette warm-neutral and almost monochrome — sheepskin, linen,
  driftwood, espresso — with sage as a single sprig (≤5%).
- **Do** carry luxury through type, space, and tone, the way The Little Nell would
  *with its photography removed*.
- **Do** push body ink dark enough to clear WCAG AA (≥4.5:1) on every neutral
  ground. Soft contrast is the aesthetic; failing contrast is not.
- **Do** keep motion smooth and calm — gentle fades, unhurried easing — with a
  `prefers-reduced-motion: reduce` fallback on every animation.
- **Do** let the serif headline open each section on its own.

### Don't:
- **Don't** let the page feel pressured, hurried, busy, or loud. That is the
  single anti-reference; every choice answers to it.
- **Don't** evoke loud HR/people-ops SaaS (Lattice, Workday) — dense, corporate,
  conversion-funnel energy is forbidden.
- **Don't** ship the first-pass AI tells the redesign exists to escape: gradient
  text, identical six-card grids, emoji icons, pill eyebrow badges, numbered
  1·2·3 markers, cream-into-white washes.
- **Don't** turn sage into a color scheme. It is one living touch, not a theme.
- **Don't** use a warm-tinted near-white (paper/parchment/biscuit) as the body —
  warmth lives in the neutrals, not in an AI-default cream.
- **Don't** add tracked-uppercase eyebrows above sections.
