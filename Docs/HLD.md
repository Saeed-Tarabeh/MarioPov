# Stomp & Bounce · One-page HLD

**One-line pitch:** Navigate a short 3D obstacle course from a first-person view, stomping mushroom enemies and using the bounce to reach the finish flag.

**Genre · view · platform:** Single-player 3D platformer · First person · Windows PC · Unity.

## Target experience
The player should feel the satisfaction of a well-timed jump and the excitement of bouncing from an enemy to the next platform. A short course and quick retries make mistakes easy to learn from.

## Core loop
Aim → Jump → Stomp → Bounce. Each successful stomp defeats an enemy and gives upward momentum for the next landing.

## Win and lose conditions
- **Win:** Touch the finish flag at the end of the course; show a victory screen with replay and main-menu buttons.
- **Lose:** Fall below the course or touch an enemy from the side; end the attempt and show a retry screen. Retry resets the player and enemies to the level's initial state.

## Controls
- **WASD:** Move. **Mouse:** Look around. **Space:** Jump while grounded.
- **Esc:** Pause/resume and release/capture the cursor. **Left mouse button:** Select menu buttons.
- Landing on an enemy's head while descending automatically triggers the stomp and bounce; no attack button is needed.

## Must-have features
- Main menu with Play, controls, and Quit.
- First-person movement, mouse look, and grounded jumping.
- One short platform course with gaps and mushroom enemies.
- Descending head-stomp detection, enemy defeat, and automatic bounce.
- Failure on falling or side contact, with a complete retry/reset.
- Finish flag, victory screen, replay, and return to menu.
- Pause/resume with correct cursor behavior.

## Look and sound
Bright, simple platforms and original stylized mushroom enemies with broad, readable heads. Use clear landing shadows and stomp feedback; add jump, stomp, failure, victory sounds and light background music.

## Out of scope this semester
Multiplayer; multiple levels or worlds; bosses; weapons and power-ups; inventory or story quests; procedural generation; mobile/console versions.
