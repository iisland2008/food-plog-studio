---
name: food-plog-studio
description: Create original vertical food-introduction plogs and covers in a warm, spacious, hand-drawn photo-collage style. Use when the user asks for a 美食 plog、探店拼贴、菜单海报、早餐/甜品/餐厅介绍图，or explicitly invokes this skill with any theme. Keep the visual DNA consistent while changing the composition and motifs; do not activate for ordinary food photography or unrelated graphic design.
---

# Food Plog Studio

Turn any supplied theme into an original food-centered vertical plog. Preserve the visual system, not any reference image's literal arrangement.

## Required visual direction

Before generating, read [references/visual-system.md](references/visual-system.md). Treat its palette, spacing, typography, photo treatment, and originality rules as invariants. Read [references/prompt-recipes.md](references/prompt-recipes.md) when shaping an ImageGen prompt or choosing a layout family.

The stable visual DNA is:

- warm restrained backgrounds; natural food colors provide most of the saturation;
- real, appetizing food photography or photorealistic food cutouts mixed with naïve hand-drawn outlines and a few doodles;
- portrait editorial collage with asymmetric balance, generous breathing room, and a clear reading path;
- relaxed handwritten or typewriter-like lettering with short, sensory annotations;
- matte, lightly grainy, tactile finish rather than glossy commercial polish.

## Interpret the request

Use the user's theme as the changing content layer. It may be a dish, ingredient, city, season, mood, color, holiday, restaurant, trip, or abstract idea. If it is not already food-specific, translate it into a coherent food story through menu choices, ingredients, serving atmosphere, or copy. Make tasteful assumptions and proceed unless a missing fact would materially change the result.

Honor supplied dishes, photos, exact wording, language, dietary facts, and brand constraints. Do not invent factual claims about a real restaurant or product. If the user supplies images, label their roles as subject/reference/edit target and inspect them before generation.

## Choose one layout family

- `hero-cover`: one dominant dish, atmospheric real-world background, 1–3 short text lines, sparse star or ingredient doodles. Best for covers and a single recommendation.
- `journal-collage`: 3–7 irregular food cutouts over a subdued photo or warm neutral background, each with a short note. Best for restaurant visits, travel food diaries, and roundups.
- `sunny-menu`: butter-yellow or cream field, top-down plated foods arranged like a playful menu, black hand lettering, ample clean space. Best for breakfast, seasonal menus, recipes, and cheerful themes.

Do not recreate the object positions, crop, title wording, background scene, or doodle set of a reference. Change at least three of these axes for every new work: focal placement, supporting-item path, background family, accent color, doodle vocabulary, title construction, crop, or label placement.

## Build the content layer

Keep copy compact and personal, not sales-heavy. Prefer:

- a 4–12 character Chinese title or 1–4 word English title;
- a one-line mood/subtitle when useful;
- 3–6 annotations of roughly 6–22 Chinese characters, each describing taste, texture, aroma, temperature, pairing, or a specific recommendation;
- only verified prices, addresses, names, and ingredients.

Use at most two typographic voices: a bold naïve handwritten display face and a lighter handwritten/typewriter annotation face. Avoid dense paragraphs.

## Generate

Use the built-in ImageGen path for the bitmap artwork. Build a structured prompt from [references/prompt-recipes.md](references/prompt-recipes.md) and include exact visible text verbatim. Keep the prompt focused on the chosen layout family rather than combining all recipes.

For dense or accuracy-critical Chinese copy, favor a visually finished base with deliberate blank annotation zones and fewer in-image words. Provide the exact copy separately if the image model cannot render it faithfully. Never silently substitute garbled or invented text.

Generate without asking for confirmation when the theme is sufficient. If the user requests several distinct versions, make separate calls with distinct prompts. Treat user photos as content inputs, not permission to copy the reference composition.

## Inspect and refine

Check the output against all of these:

1. Food is appetizing and recognizable; no malformed utensils, dishes, hands, or ingredients.
2. The palette is warm and restrained, with no unrelated neon or icy-tech colors.
3. One focal item is clear; the page feels asymmetric but balanced, with 20–35% quiet space.
4. Cutouts have handmade, slightly irregular outlines; doodles remain sparse and theme-specific.
5. Typography feels relaxed and editorial; visible text is correct and readable.
6. The work is recognizably in this visual family but not a replica of any reference.

If one criterion fails, iterate with one targeted change while restating the invariants. Return the final image inline. For a workspace-bound asset, save it in the requested/project location and report its full path; otherwise a preview may remain in the default generated-image location.
