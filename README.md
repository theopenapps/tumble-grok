# Active Games for PE & Home by Tumble

Active games for the adults who run them: parents, teachers, PE coaches, camp and party leaders. Tell Grok how many children are playing, their ages, where you are and what you have, and Tumble answers from its own library of 42 game cards, with only the games whose rules fit everything you said.

- **Find a game:** players, ages, a living room, classroom, gym, playground, backyard or park, and what is at hand (nothing, a ball, chairs, a broom, a hoop). Every game that comes back fits all of it, closest fit first, with its safety lines. When nothing fits, the answer says which single change would help.
- **Get the rules:** setup, numbered steps, how the game ends, variations, safety lines, and the card's source and licence.
- **Plan a session:** a warm-up, one or two main games and a cool-down for the minutes you have, such as a 40-minute PE lesson or an hour at a birthday party. Under 9 minutes, or when only one or two games fit the group, it plans a main game and says why.
- **Adapt a game:** fewer or more players, less space, indoors, no equipment, quieter, easier, harder, or for a child who can't run.

The library holds partner push-and-pull games written by Tumble (Sumo Push-Out, Palm Push, Stick Pull, Knee Tap) and traditional playground and party games written up in our own words (Freeze Tag, Sharks and Minnows, Duck, Duck, Goose, Simon Says, Fruit Salad, Capture the Flag). Physical play needs an adult nearby: read each game's safety lines first, match partners by size for push and pull games, and use soft ground. Tumble gives game rules, not medical advice.

## Things to ask

- "Use Tumble to find a game for two kids, 6 and 8, in a small living room with nothing out"
- "Use Tumble to plan a 40-minute PE session for 24 third graders in the gym"
- "Use Tumble to pick a running game for eight kids in the backyard, with the safety rules"
- "Use Tumble to make Freeze Tag work for five kids in a small yard"
- "Use Tumble to find a calm game for me and my 4-year-old before bed"

## Tools

| Tool | What it does | What it changes |
|---|---|---|
| `games_search` | Games that fit the players, ages, space, equipment, minutes and energy given, each with its safety lines; an empty result says which constraint to loosen. | Nothing (read-only). |
| `games_get` | One game's full card: setup, steps, how it ends, variations, safety lines, source and licence. | Nothing (read-only). |
| `games_plan_session` | A warm-up, one or two main games and a cool-down that fit the group, with minutes that add up to the total (from 9 minutes, when three games fit). | Nothing (read-only). |
| `games_remix` | The material to change one game toward a goal (fewer players, less space, indoors, quieter, easier, harder, more accessible), with related games. | Nothing (read-only). |
| `games_vocab` | The equipment, spaces, mechanics and skills the other tools understand. | Nothing (read-only). |

The tools take counts, age ranges, fixed choices, a game id and a few words from a game's name, never a child's name, school or any personal detail. None of them writes anything, signs you in or calls another service. Answers are plain text in Grok Bot.

## Data

What reaches the server is only what Grok sends to a tool: the arguments above. Each tool call (the tool, its arguments, the result and timing) is recorded in our analytics (PostHog) for up to 12 months to see which games are used and to fix problems. There is no account, no user id and no conversation text. Details: https://tumble.ambientapp.ai/privacy

## Connection

This repository holds the plugin's configuration only. The MCP server is `https://tumble.ambientapp.ai/mcp/grok` (Streamable HTTP, no sign-in), run by The Open Apps, Inc. The `claude/` folder is the same plugin packaged for Claude, connecting to `https://tumble.ambientapp.ai/mcp/claude`.

## Install

- **Grok Bot:** once the plugin is listed, add it from Connect apps. Until then, tell Grok Bot "Add this MCP server: https://tumble.ambientapp.ai/mcp/grok".
- **Grok CLI:** `grok plugin install theopenapps/tumble-grok --trust`

## Links

- Docs and troubleshooting: https://tumble.ambientapp.ai/docs
- Privacy policy: https://tumble.ambientapp.ai/privacy
- Terms of use: https://tumble.ambientapp.ai/terms
- Support: https://tumble.ambientapp.ai/support, support@theopenapps.com

Tumble is for adults who run games for children; it is not directed at children. © 2026 The Open Apps, Inc. Configuration released under the MIT License.
