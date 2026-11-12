---
name: camino-stage-difficulty
description: Distance, climb, and difficulty of one stage of the Camino de Santiago between two towns. Use when someone asks how hard a day is, how far it is between two places, or what's along the way, e.g. "How hard is Saint-Jean to Roncesvalles?", "Distance from Sarria to Portomarín?", "What's between León and Astorga?".
---

# How hard is this stage?

Use SuperCamino's `camino_stage_info` tool. It has GPS distances, total ascent and descent, and the towns along the way.

## Steps

1. Call `camino_stage_info` with `from` and `to` in the user's own words, `route` if they named one, and `language` (en, es, fr, de, it, or pt).
2. Give the distance, the total ascent and descent, and the start and end altitude. Explain the climb in plain words. For example, 1,000 m or more of ascent in a day is a hard mountain stage, a few hundred metres is moderate, and under 200 m is mostly flat.
3. Mention the towns along the way where a pilgrim can stop for food, water, or a shorter day, using `places_along_the_way`.
4. Offer the `map_url`: it shows the stage on SuperCamino's interactive map with its elevation profile and places to stay.

## Special cases

- **Over 45 km:** that's more than a day's walk. Offer to split it into days with the `plan_camino_de_santiago` tool.
- **Two places on different routes:** the result has a `stages` list instead of one map link, because a stage stays on one route (e.g. the Camino del Norte joins the Camino Francés at Arzúa). Explain that it's several stages, give each one's distance and climb, and offer each stage's `map_url`.
- **Places given backwards:** pass on the note; the details are given in walking direction.

## Language

Answer in the user's language. Names, notes, and hints in the result are in English: translate them. Keep place names as they are.
