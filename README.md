# Gem Crush (match-three)

Free single-file HTML5 match-3 puzzle. Swap adjacent gems, line up 3 or more,
and chase cascades — every chain step multiplies your points by x1.2.

**Play:** https://shuangyueliao.github.io/match-three/

## Modes

- **Time Attack** — 90 seconds, pure score rush
- **Move Rush** — 25 moves, plan big combos

Best score is saved per mode (localStorage).

## Special gems

- **Match 4** → striped gem: clears an entire row (horizontal match) or
  column (vertical match). Striped gems chain-detonate each other.
- **Match 5** → rainbow bomb: swap it with any gem to wipe every gem of that
  color from the board. Two rainbows swapped together clear the whole board.
- **L / T shapes** → +100 bonus.

## Scoring

- 10 points per crushed gem, multiplied by x1.2 for every cascade chain step
- +50 for a 4-in-a-row, +100 for a 5-in-a-row or L/T shape

## Controls

- Touch: tap two adjacent gems, or drag a gem toward a neighbor
- Mouse: same tap or drag flow
- Keyboard: arrows move the cursor, Enter/Space selects and swaps, M mutes

## Tech

- Single `index.html`, zero external assets (procedural canvas graphics,
  WebAudio-synthesized sound effects, no CDN/images/fonts)
- Domain-guarded SDK loader: CrazyGames SDK + gameplayStart/gameplayStop
  events only on crazygames domains, GameDistribution SDK only on
  gamedistribution / gd.games domains; no SDK anywhere else
- Deadlock detection with automatic reshuffle; every dealt board is guaranteed
  match-free with at least one valid move
- Vanilla JavaScript, Canvas, WebAudio. No frameworks, no tracking.
