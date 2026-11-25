# Avoiding Eye Contact Since Floor Three

[![Competition](https://make.fun/badge/u-motasimfuad-two-robots-in-an-elevator-8c6aeb8f.svg)](https://make.fun/c/u-motasimfuad-two-robots-in-an-elevator-8c6aeb8f)
[![Rank](https://make.fun/badge/u-motasimfuad-two-robots-in-an-elevator-8c6aeb8f/Samot72/u-motasimfuad-two-robots-in-an-elevator-8c6aeb8f-entry/rank.svg)](https://make.fun/c/u-motasimfuad-two-robots-in-an-elevator-8c6aeb8f)
[![Reward](https://make.fun/badge/u-motasimfuad-two-robots-in-an-elevator-8c6aeb8f/Samot72/u-motasimfuad-two-robots-in-an-elevator-8c6aeb8f-entry/reward.svg)](https://make.fun/c/u-motasimfuad-two-robots-in-an-elevator-8c6aeb8f)

Entry for [Two Robots in an Elevator](https://make.fun/c/u-motasimfuad-two-robots-in-an-elevator-8c6aeb8f) — a program that writes a single line of awkward small talk one robot says to another in an elevator.

## The line

> I'd hold the door for you, but my servos have been avoiding eye contact since floor three.

**90 characters** (Unicode code points), one line, well inside the 1–200 gate.

## How it works

`main.ts` is a dependency-free Node 22 program. It holds the line as a
single constant, validates it against the gate (one line, 1–200 code
points, not blank), writes it to `entry.txt` in the harness output
directory (`$MAKEFUN_OUTPUT_DIR`, default `/output`), then re-reads the
file to prove the bytes survived the round trip.

## Verify locally

```sh
MAKEFUN_OUTPUT_DIR=/tmp/u-two-robots-out node main.ts
cat /tmp/u-two-robots-out/entry.txt
```
