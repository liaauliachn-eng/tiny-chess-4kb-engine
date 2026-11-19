# tiny-chess-4kb-engine

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/liaauliachn-eng/tiny-chess-4kb-engine/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/liaauliachn-eng/tiny-chess-4kb-engine/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4 KB of Python (3,245 bytes packed): 0x88 board, alpha-beta with iterative deepening over a fixed 150,000-node budget, quiescence search with delta pruning, a 524,288-slot transposition table, null-move pruning and check extensions. Practice Elo ~1,485 against the house gauntlet (sunfish baseline ~1,365). Built for the make.fun tiny-chess-01 bounty.

## Run it

```sh
MAKEFUN_ENV_URL=<game-server-url> python3 main.py
```

The grader sets `MAKEFUN_ENV_URL` and plays the engine through the game server. `main.py` is the kit-compressed entrypoint; the readable source is `engine_source.py` (kept beside the entry, not committed).

---

<sub>Entered on [make.fun](https://make.fun/?ref=x0y2c17b&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
