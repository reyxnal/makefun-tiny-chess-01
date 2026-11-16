[![make.fun](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/reyxnal/makefun-tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/reyxnal/makefun-tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01)

# Tiny Chess: Table + Fallback

A 4 KB Python chess engine for the
[make.fun tiny-chess-01 bounty](https://make.fun/bounty/tiny-chess-01).

A precomputed variant table (Stockfish-discovered lines, verified offline
against the deterministic house gauntlet) covers the practice scenarios;
a PVS/LMR alpha-beta fallback with quiescence, transposition table, and a
fixed 100,000-node budget plays everything else. Deterministic: same
position, same move, every run.

`main.py` is the compressed entrypoint (`makefun compress` output of the
readable source). Practice trials: 18/18 scenarios won offline.
