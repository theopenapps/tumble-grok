# Active Games for PE & Home by Tumble

Active games for the adults who run them: parents, teachers, PE coaches, camp and party leaders. Ask Claude for a game that fits how many children are playing, their ages, the space and what you have, and Tumble answers from its own library of 42 game cards, with only the games whose rules fit everything you said. It can also give a game's full rules, plan a timed session (a 40-minute PE lesson, an hour at a birthday party) or adapt a game you know for fewer players, less space, a quieter room or a child who can't run. Every game carries its safety lines.

## What's in it

- **Skills:** `find-a-game`, `plan-a-session` and `remix-a-game` tell Claude when Tumble fits and how to turn a request into a search, a session or an adapted game.
- **Connector:** Tumble's MCP server at `https://tumble.ambientapp.ai/mcp/claude` (no sign-in). After installing the plugin, connect it from the plugin's Connectors tab. On claude.ai a card shows each game moving; the answer text carries the same rules.

The library holds partner push-and-pull games written by Tumble (Sumo Push-Out, Palm Push, Stick Pull, Knee Tap) and traditional playground and party games written up in our own words (Freeze Tag, Sharks and Minnows, Duck, Duck, Goose, Simon Says, Fruit Salad, Capture the Flag).

## Install

- **claude.ai and Cowork:** once listed, Customize, Plugins, Discover, then connect Tumble from the plugin's Connectors tab. Without the plugin, add `https://tumble.ambientapp.ai/mcp/claude` as a custom connector with no authentication.
- **Claude Code:** once listed, find Tumble with `/plugin` in the plugin directory.

## Things to ask

- "Use Tumble to find a game for two kids, 6 and 8, in a small living room with nothing out"
- "Use Tumble to plan a 40-minute PE session for 24 third graders in the gym"
- "Use Tumble to make Freeze Tag work for five kids in a small yard"

## Tools

| Tool | What it does | What it changes |
|---|---|---|
| `games_search` | Games that fit the players, ages, space, equipment, minutes and energy given, each with its safety lines. | Nothing (read-only). |
| `games_get` | One game's full card: setup, steps, how it ends, variations, safety lines, source and licence. | Nothing (read-only). |
| `games_plan_session` | A warm-up, one or two main games and a cool-down for the minutes given (from 9 minutes, when three games fit). | Nothing (read-only). |
| `games_remix` | The material to change one game toward a goal, with related games. | Nothing (read-only). |
| `games_vocab` | The terms the other tools understand. | Nothing (read-only). |

## Data sent

Only the tool arguments Claude sends: a number of players, an age range, a kind and size of space, equipment, minutes, an energy level, a game id, a goal for adapting a game, or a few words from a game's name. They go to tumble.ambientapp.ai and nowhere else. Each tool call (the tool, its arguments, the result and timing) is kept in our analytics (PostHog) for up to 12 months. No account, no user id, no conversation text, and no field for a child's name or any personal detail. The plugin runs no local code, hooks or scripts.

Physical play needs an adult nearby. Tumble gives game rules, not medical advice.

## Links

- Docs: https://tumble.ambientapp.ai/docs
- Privacy policy: https://tumble.ambientapp.ai/privacy
- Terms of use: https://tumble.ambientapp.ai/terms
- Support: https://tumble.ambientapp.ai/support, support@theopenapps.com

© 2026 The Open Apps, Inc. Released under the MIT License.
