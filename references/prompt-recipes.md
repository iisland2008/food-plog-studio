# ImageGen prompt recipes

Use one recipe per image. Replace bracketed fields with the user's content and omit irrelevant lines.

## Shared prompt spine

```text
Use case: ads-marketing
Asset type: original vertical food plog / editorial social poster
Primary request: Create an original food-introduction plog about [theme].
Scene/backdrop: [chosen background family and setting]
Subject: [hero dish] with [supporting foods/ingredients]
Style/medium: photorealistic appetizing food combined with handmade editorial scrapbook collage; naïve hand-drawn outlines and sparse doodles; matte tactile finish; not a vector-only illustration
Composition/framing: portrait 3:4; [layout-family geometry]; one clear hero; asymmetric balance; 5–8% safe margins; 20–35% quiet space
Lighting/mood: warm natural or ambient light, gentle realistic shadows, cozy and personal
Color palette: [palette]; food provides the saturated accents; restrained overall color count
Materials/textures: visible ceramic, paper, crumbs, glaze, wood or soft wall texture; subtle film grain
Text (verbatim): "[exact title]"; "[exact subtitle/annotations]"
Typography: relaxed naïve hand lettering, slightly irregular baseline, airy spacing; at most two typographic voices; high contrast and readable
Constraints: original composition; accurate food anatomy; handmade 3–6 px outlines; sparse theme-specific doodles; preserve exact supplied facts
Avoid: copying any reference layout or motif placement, logos unless supplied, watermark, neon palette, glossy commercial ad look, dense paragraphs, malformed utensils, garbled or invented text
```

## Recipe A — hero-cover

```text
Scene/backdrop: a slightly darkened warm [restaurant/interior/table/window] scene with tactile wood, plaster, or linen texture
Subject: one large cutout of [hero dish] with appetizing detail and a thin irregular [ochre/chalk-white] outline
Composition/framing: portrait 3:4; hero placed off-center across the central third; 25–40% of the canvas; calm space reserved for a short title near [lower-left/lower-center/side]
Doodles: 2–5 original [ingredient/star/steam] marks orbiting the dish, unevenly spaced
Text: title plus at most one small descriptor
```

Vary hero location, title zone, background setting, outline color, and doodle vocabulary from project to project.

## Recipe B — journal-collage

```text
Scene/backdrop: full-bleed, slightly darkened [place/mood] photograph with enough calm surface for notes
Subject: [3–7 foods], each as an irregular photorealistic cutout; one hero is clearly larger than the rest
Composition/framing: portrait 3:4; loose [S-curve/diagonal/triangle] reading path; alternating food clusters and notes; varied rotation and scale; 20–30% breathing room
Outlines: chalk-white handmade borders with small natural inconsistencies and occasional light offset shadows
Doodles: 3–8 tiny, theme-specific marks placed only where they support the reading path
Text: one compact title and 3–6 short sensory annotations, never a continuous paragraph
```

## Recipe C — sunny-menu

```text
Scene/backdrop: flat butter-yellow or warm-cream paper field with subtle paper grain
Subject: top-down plated [menu items], photorealistic and naturally shadowed, with ceramic and glass variation
Composition/framing: portrait 3:4; 5–8 foods in a loose editorial flat-lay; large title in one corner; uneven but generous gaps; one plate anchors the lower or upper third
Typography: ink-brown naïve uppercase or simple Chinese hand lettering with a smaller loose handwritten secondary voice
Doodles: minimal black/brown ingredient labels, curved underlines, or tiny sparkle marks
Text: dish names or very short labels only
```

## Text-density fallback

When exact Chinese text exceeds what ImageGen can reliably render:

```text
Create the complete plog artwork with intentional empty annotation zones and no placeholder gibberish. Render only the short exact title "[title]". Keep the blank zones visually integrated so accurate copy can be added separately.
```

After generation, inspect every visible character. If text remains wrong, do not present it as final accurate copy; return the clean art plus the exact text and placement plan.
