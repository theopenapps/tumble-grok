---
name: plan-a-session
description: "Plan a timed play session with Tumble, with a warm-up, one or two main games and a cool-down. Use when a teacher, coach or parent wants a PE lesson, a recess or after-school block, a camp slot, a party schedule or an hour of active games at home."
---

Use this skill when the adult running the games wants a whole session for a set number of minutes rather than a single game. The user's explicit instructions come first.

## Flow

1. `games_plan_session` takes the minutes plus the same constraints as a search: players, ages, space, equipment and energy. A PE lesson in the gym is `space_kind: gym`; a class of third graders is ages 8 to 9.
2. From 9 minutes, whenever three games fit the group, the plan has a warm-up that builds up, one or two main games at the most active level, and a cool-down that winds down. Every slot fits the constraints and the minutes add up to the total.
3. The session reads well as a numbered list in order: phase, minutes, game, one line on how it runs, and its safety lines. `games_get` gives the full rules of any slot the user wants to see.
4. A shorter session, or a group that only one or two games fit, gets a main game and a note that says why; more time or a looser constraint (a wider age range, a bigger space) can add the missing phases.

## Scope

- Sessions are built only from Tumble's game library.
- Training plans and drills for a team sport (football, basketball, swimming) are outside Tumble.
- Physical play needs an adult nearby; contact games ask for partners of a similar size and soft ground.
