---
name: find-a-game
description: "Find an active game that fits a real group with Tumble. Use when a parent, teacher, coach or party leader asks what to play with the kids, such as a rainy-day game for the living room, a recess or playground game, a birthday party game, a tag game for the backyard, or something for a broom and a hallway."
---

Use this skill when the adult running the games wants one game for a real situation: how many are playing, their ages, the space and what is at hand. The user's explicit instructions come first.

## Flow

1. When the group, the ages or the space are missing, one short question covers them; otherwise a stated assumption works ("a normal living room, nothing out").
2. `games_search` takes the constraints. Everyday words map onto its terms: a living room or classroom is `space_kind: room` with `space_size: small`; a hallway or balcony is `tiny`; a backyard or playground is `outdoor` at `medium`; a field or park is `large`. "Nothing" is `equipment: []`, a broom or a dowel is `stick`, pool noodles are `foam-stick`, chairs are `chair`. "Tire them out" is `energy: ["high"]`, "calm down" or "before bed" is `["low"]`.
3. Every game in the result fits all the constraints given, closest fit first, with its safety lines. A short pick with a line on why it fits works well, followed by one or two alternatives.
4. When the user picks a game, `games_get` returns its full card: setup, numbered steps, how it ends, variations, safety lines and its source. The rules read best as short numbered steps in plain words, with the card's safety lines kept.
5. An empty result says which single constraint to loosen and how many games that opens up; offering that change is the next step.

## Scope

- Tumble's games come only from its own library of game cards; a game outside a tool result isn't one of Tumble's.
- The user is the adult who runs the game. No tool needs a child's name, school or any personal detail.
- Video games, board and card games, sports drills and injury or medical questions are outside Tumble; the assistant answers those itself.
