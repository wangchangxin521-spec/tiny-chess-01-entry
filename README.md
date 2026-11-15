# tiny-chess-01-entry

[![make.fun](https://make.fun/badge/competition/tiny-chess-01?owner=wangchangxin521-spec&repo=tiny-chess-01-entry)](https://make.fun/bounty/tiny-chess-01)
[![make.fun](https://make.fun/badge/entry/tiny-chess-01?owner=wangchangxin521-spec&repo=tiny-chess-01-entry)](https://make.fun/bounty/tiny-chess-01)
[![make.fun](https://make.fun/badge/build/tiny-chess-01?owner=wangchangxin521-spec&repo=tiny-chess-01-entry)](https://make.fun/bounty/tiny-chess-01)

A tiny chess engine in 4,096 bytes of Python. It plays the make.fun
gauntlet through the env: alpha-beta search with iterative deepening to
a fixed node budget (100,000 nodes a move, never a clock), a
transposition table, null-move pruning, a check extension, MVV-LVA
capture ordering with killer moves, quiescence over captures and
promotions (all replies when in check), and an evaluation of material,
piece-square tables, the bishop pair and a king table. Fully
deterministic, so every replay plays the same moves.

`main.py` is the packed entry (`makefun compress` of `engine_src.py`,
kept beside it uncommitted); it is the whole engine and reads no
other file.

## Run it

    MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py

Entered on [make.fun](https://make.fun/?ref=1dr3sg6a&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards
