# Backrooms Build Brawl — Prototype Gate

A 3D arena prototype based on the drawings and story of **August Spangler**.

**Art & Story by August Spangler • Directed by August & Corey Spangler • Built by AI**

## The idea

Shoot, build, and bonk in the Backrooms. Captain Clark battles the Balloon Smiler
and friends — and when you get bonked, you don't just wait to respawn. You get
**60 seconds as a ghost to build defenses** around the spot where you fell
(**Bonk-to-Build**), then you respawn and fight from your own fort.

## This build

This is the *prototype gate* build — it exists to prove the hardest part first:
a bot that can chase you through a maze you keep rebuilding.

- One Balloon Smiler bot with grid pathfinding that updates live when blocks change
- The bot reroutes around new walls and bonks through destructible blocks when trapped
- Bonk-to-Build ghost mode: 60-second build window, RESPAWN NOW button, safe-respawn check
- Swept projectile collision, instanced block rendering — built to hold 30+ FPS on a Chromebook
- Test Lab (press `P` in a match) with one-button versions of the design review tests
- Debug overlay (backquote key) showing bot paths
- Keyboard/trackpad controls and gamepad support

Play it: open `index.html` in a browser (internet needed once for the Three.js CDN).

## Council process

Designed by an AI council, in the open:
1. **Gemini** — design completeness pass (what the spec forgot)
2. **ChatGPT** — hostile review (top failure modes, the kill question, mandatory rules)
3. **Claude** — build, with the other two passes folded in as amendments

Full council record is in the "Backrooms Build Brawl — Council" Google Drive folder.

## Not yet tested

- A real low-end Chromebook (the performance gate)
- Real pointer lock with a human clicking
- A plugged-in Xbox controller
