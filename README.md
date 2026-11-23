# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/kurage-0108/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/kurage-0108/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in a single Python file of 3,732 bytes: negamax alpha-beta search with principal-variation search, a transposition table, quiescence search with check evasions, null-move and reverse-futility pruning, late-move reductions and check extensions, on a 10x12 board that flips after every move so the side to move is always White-perspective. Evaluation uses tapered PeSTO piece-square tables packed as complex numbers (middlegame and endgame values carried in one number), plus a king pawn-shield term and an endgame mop-up term. It plays on a fixed budget of 60,000 nodes per move — fully deterministic, no clock use — through the make.fun environment protocol.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8791 python3 main.py
```

(Point MAKEFUN_ENV_URL at a running make.fun env server, e.g. the practice server from the tiny-chess-01 kit.)

---

<sub>Entered on [make.fun](https://make.fun/?ref=5k40m5db&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
