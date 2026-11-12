# Stomp & Bounce · Feature backlog and scope plan

All features below are planned, not implemented. Effort is relative: S = small, M = medium, L = large.

## Backlog (MoSCoW)

| Feature | MoSCoW | Why | Effort (S/M/L) |
| --- | --- | --- | --- |
| Main menu with Play, controls, and Quit | Must | Provides an understandable starting point. | S |
| First-person movement, mouse look, and grounded jumping | Must | Lets the player navigate and aim jumps. | M |
| One short platform course with gaps and mushroom enemies | Must | Provides a complete route from spawn to finish. | M |
| Descending head-stomp detection, enemy defeat, and automatic bounce | Must | Delivers the central mechanic and enables bounce traversal. | L |
| Failure on falling or side contact, with a complete retry/reset | Must | Makes failed attempts clear and allows another complete run. | M |
| Finish flag, victory screen, replay, and return to menu | Must | Gives the game an ending and closes the play cycle. | S |
| Pause/resume with correct cursor behavior | Must | Allows interruption and usable menu interaction. | S |
| Landing shadow and readable enemy head targets | Should | Helps judge distance and landings in first person. | M |
| Jump, stomp, failure, and victory sound effects | Should | Makes actions and outcomes easier to understand. | S |
| Cohesive original visuals, background music, and UI styling | Should | Supports the playful mood and the generative-assets milestone. | M |
| Simple enemy patrol between two points | Should | Adds variety after stationary enemies work reliably. | M |
| Adjustable mouse sensitivity and audio volume | Could | Improves comfort without changing the core game. | S |
| Optional collectible coins | Could | Adds an extra challenge without blocking the finish. | M |
| Completion timer and best time for the current session | Could | Encourages replay after the basic course is complete. | S |
| Multiplayer | Won't | Networking is beyond this single-player project's scope. | L |
| Multiple levels or worlds | Won't | One finished course is the semester scope. | L |
| Bosses | Won't | Requires additional combat and behavior systems. | L |
| Weapons and power-ups | Won't | Stomping and bouncing provide the core interaction. | L |
| Inventory or story quests | Won't | Does not serve the short platforming experience. | L |
| Procedural generation | Won't | Hand-built jumps are easier to tune and verify. | L |
| Mobile/console versions | Won't | Keyboard and mouse on Windows is the target. | L |

## Scope plan

| Deadline | What must be playable | Backlog items |
| --- | --- | --- |
| HA02 · Prototype · Lesson 7 | Complete placeholder run: menu → movement and jumps → stomp and bounce → finish → replay. Falling and side contact cause failure; retry resets everything. Pause works. | All Musts, using simple geometry and stationary enemies. |
| HA03 · Agentic Workflow · Lesson 10 | The same full run remains stable after focused development tasks; improve jump readability and test stomp edge cases, reset, menus, and pause. Keep workflow evidence in the DevLog. | Refine Musts; add landing shadow/readable targets. Add patrol only if the core is reliable. |
| HA04 · Generative Assets · Lesson 12 | Integrate AI-made visuals, music, sound effects, and UI into the playable game. Confirm replacement assets preserve collision readability and game behavior. | Cohesive visuals/music/UI; action and outcome sound effects. |
| Final Project · 3 days before Lesson 14 | Every Must complete; final assets integrated; full start-to-end playthrough and retry verified; documentation matches the delivered game. | All Musts plus completed milestone assets. Coulds only if they do not delay completion. |

## Riskiest Must and Plan B

**Risk:** Reliable first-person stomp-and-bounce detection. A descending head landing must defeat the enemy and apply one bounce, while side contact must cause failure. Fast falls, edge hits, and overlapping collision events may produce inconsistent results.

**Early check:** Prototype this interaction before building the full course. Check centered and edge landings, side contact, contact while rising, repeated overlaps, and reset after defeat.

**Plan B:** Keep enemies stationary, enlarge the head landing area, use broad platforms and shorter gaps, and remove patrols and chained precision jumps. Keep the required stomp-and-bounce mechanic with one generous bounce-assisted jump; simplify the course instead of adding new systems.
