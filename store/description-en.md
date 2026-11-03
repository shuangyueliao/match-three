# Gem Crush — Store Submission Materials

## Short description (CrazyGames / GameDistribution / itch.io)

Swap gems, line up 3+. Match 4 for a striped gem that clears a row or
column, match 5 for a rainbow bomb that wipes a whole color. Cascades
multiply your score x1.2 per chain!

## Details

- Genre: Puzzle / Casual / Match-3
- Controls: Mouse / Touch — tap two adjacent gems or drag a gem toward a
  neighbor. Keyboard: arrows move the cursor, Enter/Space selects and swaps,
  M mutes.
- Modes: Time Attack (90 seconds) and Move Rush (25 moves), each with its own
  saved best score (localStorage).
- Features: cascade combo scoring (x1.2 per chain), striped gems (row/column
  clear with chain detonation), rainbow bombs (whole-color wipe), L/T bonus
  (+100), deadlock detection with auto reshuffle, guaranteed-solvable boards,
  particle effects, bounce easing, synthesized sound.
- Tech: Vanilla JavaScript, Canvas, WebAudio. Single-file HTML5 (45 KB, no
  external assets), works offline once loaded. No frameworks, no tracking.

## Tags

match-3, match3, puzzle, casual, gems, jewels, swap, collapse, arcade, single-file

## CrazyGames submission checklist
- [x] Self-contained index.html (SDK loads only on crazygames domains)
- [x] gameplayStart / gameplayStop / loadingStart / loadingStop / happytime events wired
- [x] Responsive (square canvas scales to fit, portrait-friendly)
- [x] No external links inside gameplay, no analytics
- [ ] Cover: cover-16x9.png (1280x720) — screenshot the board from a live game
- [ ] Screenshots: 2-3 in-game shots (1280x800)

## GameDistribution submission checklist
- [x] match-three-gd.zip contains only index.html
- [x] Game loads on gamedistribution / gd.games domains (GD SDK v2 auto-loads
      via the domain-guarded loader; no other SDK loads elsewhere)
- [x] No revenue-sharing or ad code beyond the official GD SDK script

## itch.io
- Upload match-three-itch.zip (rename to gem-crush.zip), mark
  "This file will be played in the browser", entry file: index.html,
  viewport 480x520, kind: html, embed options: fullscreen button recommended
- Pricing: $0 (donations optional)
- Suggested page tags: match-3, puzzle, casual, html5, single-file
