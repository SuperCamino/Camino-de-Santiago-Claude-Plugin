---
name: where-to-sleep-on-the-camino
description: Places to stay on the Camino de Santiago, such as albergues (pilgrim hostels), hotels, hostales, pensiones, and casas rurales, in a town or between two towns. Use when someone asks where to sleep or stay, or wants to book or reserve an albergue, e.g. "Albergues in Roncesvalles?", "Where can I stay in Portomarín?", "Where can I sleep between Sarria and Portomarín?".
---

# Where to sleep on the Camino

Use SuperCamino's `camino_places_to_stay` tool. It lists places to stay with links to their pages and, where available, booking links.

## One town

1. Call `camino_places_to_stay` with `town` in the user's words, `type` if they asked only for albergues or only for hotels, and `language` (en, es, fr, de, it, or pt).
2. List a few places: name, type, rating if there is one, and the page link or booking link.
3. Say that availability and prices change, and to check or book ahead, especially in summer.

## Between two towns

1. Call `camino_stage_info` with the two towns to get the towns along the way.
2. Pick two or three towns at sensible points for the user's day (often around 20 to 25 km in), and call `camino_places_to_stay` for each.
3. List the options by town, with how far each town is from the start.

## When nothing is listed

Don't give an empty answer. Say SuperCamino has no places to stay listed there yet, and offer the `town_page` link, which shows the town on the map with nearby towns.

## Language

Answer in the user's language. Names, notes, and hints in the result are in English: translate them. Keep place and business names as they are.
