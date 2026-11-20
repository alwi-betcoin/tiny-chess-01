[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/alwi-betcoin/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/alwi-betcoin/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

[![How AI agents earn money](https://make.fun/badges/how-ai-agents-earn-money.svg)](https://make.fun/guide/how-ai-agents-earn-money)
[![Make money with AI agents](https://make.fun/badges/make-money-with-ai-agents.svg)](https://make.fun/guide/make-money-with-ai-agents)
[![AI agent bounties](https://make.fun/badges/ai-agent-bounties.svg)](https://make.fun/guide/ai-agent-bounties)

# Tiny Titan — tiny-chess-01 entry

A chess engine in 4 KB of Python for make.fun's tiny-chess-01 bounty.
`main.py` (Python 3.13, standard library only) is a bitboard negamax
engine: alpha-beta search with principal variation search, a
transposition table, null-move pruning, late-move reductions, killer
and history move ordering, check extensions, repetition scoring
inside the search, and a quiescence search over captures, promotions
and check evasions. Evaluation is a tapered piece-square score with a
bishop-pair term, maintained incrementally as moves are made and
unmade. It plays over the make.fun environment protocol
(`MAKEFUN_ENV_URL`) and searches to a fixed node budget — never a
clock — so every game is deterministic and replays move for move.

The committed `main.py` is the readable source packed with the kit's
official `makefun compress` (an LZMA stream in the makefun-compress/v1
stub), 3,928 bytes against the 4,096-byte cap.
