# Backrooms Build Brawl

A 3D arena game based on the drawings and story of **August Spangler**. **Version 2 — Capture the Flag** (audited Nov 23, 2026): 3v3 CTF with the Funny Arsenal, nine playable characters, and Bonk-to-Build fort building.

**Art & Story by August Spangler • Directed by August & Corey Spangler • Built by AI**

## The idea

Shoot, build, and bonk in the Backrooms. Captain Clark battles the Balloon Smiler
and friends — and when you get bonked, you don't just wait to respawn. You get
**60 seconds as a ghost to build defenses** around the spot where you fell
(**Bonk-to-Build**), then you respawn and fight from your own fort.

## This build

The full game (the navigation prototype passed its gate and the director's playtest):

- Three bot rivals — Balloon Smiler (rusher), Crab Boss (strafing tank), Hazmat Explorer
  (cover-user and flanker) — fighting you *and each other*, with a live scoreboard
- Bots play the whole game: when bonked, each bot does its own Bonk-to-Build and
  raises a small fort before respawning
- Grid pathfinding that updates live when blocks change; bots reroute around new
  walls and bonk through destructible blocks when trapped
- 5-minute matches; ties go to Sudden Bonk overtime (first bonk wins, 30 quiet
  seconds is a draw)
- Two-zone arena: Yellow Rooms + flooded Water Rooms, landmarks, minimap, pre-built cover
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
