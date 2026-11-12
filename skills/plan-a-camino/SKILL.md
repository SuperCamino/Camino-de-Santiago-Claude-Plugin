---
name: plan-a-camino
description: Plan a Camino de Santiago day by day, as a day-by-day itinerary of Camino stages. Use when someone asks where to stop each night, how many km a day to walk, wants a Camino itinerary or stages, or asks to walk a number of days from a starting town, e.g. "I want to walk from Sarria, where should I stop each night?", "the Camino Francés in 30 days from 1 October", "Camino Portugués from Porto in 2 weeks", "Le Puy to Santiago". Covers the Francés, Portugués (central and coastal), Norte, Primitivo, Inglés, Finisterre and Muxía, the Spiritual Variant, and the Via Podiensis. Also: Jakobsweg, chemin de Compostelle, Cammino di Santiago, Caminho de Santiago, etapas.
---

# Plan a Camino

Use SuperCamino's `plan_camino_de_santiago` tool for every Camino plan. It has GPS distances and climbs for each day, picks the towns pilgrims usually stay in, and returns a link that opens the plan in SuperCamino's free planner.

## Steps

1. Call `plan_camino_de_santiago` straight away. Don't ask follow-up questions first: the tool always picks the best match for place and route names, and the user will say if it guessed wrong.
   - `start`: the starting town in the user's own words ("St Jean", "Sarria").
   - `end`: only if the user named one. It defaults to Santiago de Compostela.
   - `days`, `km_per_day`, or `max_km_per_day`: only what the user said.
   - `route`: any route the user named, in their words ("Portuguese coastal", "Norte then Primitivo").
   - `start_date`: if the user gave a start date (YYYY-MM-DD).
   - `language`: the language the user is writing in (en, es, fr, de, it, or pt), so the links open in it.
2. Show the plan as a short table: day, from and to, km, and climb (ascent). Add dates if the result has them. Mention one or two places to stay per night only if the user asked about accommodation.
3. Always offer the `planner_url`, saying what it's for: the user can adjust stops, add rest days, see each stage on the map, and save the plan for free.
4. Pass on anything in `notes` (for example, that a place is on a variant and the plan starts from the nearest main-route town).

## Changes

- "Fewer days", "shorter days", "start from León instead": call the tool again with the new values. Don't recalculate distances by hand.
- Rest days and variants (such as Valcarlos or Samos) aren't in the plan. Say they can be added in the planner.

## Language

Answer in the user's language. Names, notes, and hints in the result are in English: translate them. Keep place names as they are.
