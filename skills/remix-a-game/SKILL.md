---
name: remix-a-game
description: "Adapt a game from Tumble's library to the group in front of you. Use when someone wants a game like Freeze Tag, Duck, Duck, Goose or Sumo Push-Out to work with fewer or more players, in less space, indoors, without equipment, quieter, easier, harder or for a child who can't run."
---

Use this skill when the adult running the games knows a game and wants it changed for their group. The user's explicit instructions come first.

## Flow

1. `games_search` with words from the game's name in `q` finds its id when the user names a game.
2. `games_remix` takes the id and one goal (`effect`): fewer-players, more-players, less-space, indoor, no-equipment, quieter, more-active, easier, harder, accessibility, theme, longer or shorter.
3. The result carries the game's full card, its variations already aimed at that goal and related games that share its mechanics. Adapted rules are written from that material, as short numbered steps, saying what changed and what stayed, with the card's safety lines kept.
4. For a goal the card has no variation for, the mechanics and the related games show what can change; a related game that already fits may be the better suggestion.

## Scope

- Adaptations stay within the card's material and its safety lines; Tumble doesn't invent new games.
- Games outside Tumble's library are outside this skill; the assistant can still talk about them itself.
