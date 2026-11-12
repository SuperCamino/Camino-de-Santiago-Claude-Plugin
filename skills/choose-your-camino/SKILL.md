---
name: choose-your-camino
description: Help someone choose which Camino de Santiago route to walk, by time available, difficulty, crowds, and scenery. Use when someone asks which Camino to walk, where they should start the Camino, compares routes, says how much time they have, or asks about walking the last 100 km for the Compostela, e.g. "Which Camino should I walk?", "Where should I start the Camino?", "Francés or Portugués?", "I have 2 weeks, which Camino?", "What's the easiest Camino?".
---

# Choose your Camino

Give a short, honest comparison, then end with a real plan from SuperCamino's `plan_camino_de_santiago` tool, so the user always gets a planner link.

## The routes SuperCamino covers

Distances are rounded, from SuperCamino's route data, to Santiago unless noted. For a specific start point, get exact figures from the tools rather than these.

| Route | Common starts and distance | Character |
| --- | --- | --- |
| Camino Francés (French Way) | Saint-Jean-Pied-de-Port, about 765 km (about 5 weeks); León, about 305 km (about 2 weeks); Sarria, about 115 km (5 to 6 days) | The classic and the busiest. Best infrastructure and most albergues, very social. A hard Pyrenees crossing on day 1 from Saint-Jean, the flat Meseta in the middle, and green Galicia at the end. |
| Camino Portugués, central | Lisbon, about 620 km; Porto, about 245 km (about 2 weeks); Tui, about 120 km (about 6 days) | The second most popular. Gentler hills, good infrastructure, Portuguese and Galician towns. |
| Camino Portugués, coastal | Porto, about 270 km (about 2 weeks) | Atlantic coast and fishing towns, joining the central route at Redondela. Quieter than the central route. |
| Camino del Norte (Northern Way) | Irún or Hendaye, about 865 km (about 5 weeks) | Along Spain's north coast: beaches, cities like San Sebastián, Bilbao, and Santander. Hillier than the Francés, fewer albergues, quieter. Joins the Francés at Arzúa. |
| Camino Primitivo | Oviedo, about 315 km (about 2 weeks) | The oldest route. Mountainous and remote, the hardest per day, quiet. Joins the Francés at Melide. |
| Camino Inglés (English Way) | Ferrol, about 115 km (5 to 6 days) | Short, quiet, and green. Good for a week. |
| Finisterre and Muxía | From Santiago, about 85 km to Fisterra (3 to 4 days) | Walked after Santiago, to the Atlantic at "the end of the world". |
| Via Podiensis (Le Puy route) | Le Puy-en-Velay to Saint-Jean-Pied-de-Port, about 740 km | France's best-known route, through the Massif Central and Gascony. Continues as the Camino Francés. |
| Spiritual Variant | Pontevedra to Padrón area, about 75 km | A variant of the Portuguese Way, with a stage by boat along the Ría de Arousa. |

To receive the Compostela certificate in Santiago, pilgrims walk at least the last 100 km (200 km by bike).

## Steps

1. If the user hasn't said, it helps to know how many days they have, and whether they want busy and social or quiet, flat or mountains. Don't hold up the answer to ask: give the comparison for what they said, and offer alternatives.
2. Recommend one or two routes with a reason in a sentence each. Keep it short.
3. Call `plan_camino_de_santiago` for the main recommendation, with a start point that fits their time (for 1 week: Sarria, Tui, or Ferrol; for 2 weeks: León, Porto, or Oviedo; for 5 weeks: Saint-Jean or Irún) and `language` (en, es, fr, de, it, or pt).
4. Show the plan as a short table (day, from and to, km, climb) and offer the `planner_url` to adjust and save it for free.

## Language

Answer in the user's language. Names, notes, and hints in the tool results are in English: translate them. Keep place names as they are.
