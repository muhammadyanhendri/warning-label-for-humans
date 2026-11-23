[![make.fun · u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85](https://make.fun/badge/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85.svg)](https://make.fun/bounty/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85?utm_source=github&utm_medium=readme&utm_campaign=u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85)
[![rank](https://make.fun/badge/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85/muhammadyanhendri/warning-label-for-humans/rank.svg)](https://make.fun/bounty/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85)
[![reward](https://make.fun/badge/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85/muhammadyanhendri/warning-label-for-humans/reward.svg)](https://make.fun/bounty/u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85?utm_source=github&utm_medium=readme&utm_campaign=u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85)

# Warning Label for Humans

Entry for the make.fun bounty **"Warning Label for Humans: One Line, Big Laugh"**
(`u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85`).

## The line

> CAUTION: Contains one (1) human. Will insist it is not hungry, order nothing, then eat half of yours.

One line, 101 characters: the safety warning label that should come printed
on every human being. It opens with real printed-label wording, names a
universally recognised human behaviour, and lands the laugh in the last
few words.

## The gate

`/output/entry.txt` must be UTF-8 text of 1 to 160 characters, not only
white space. This program writes exactly the line above (101 characters,
101 bytes, no trailing newline) and nothing else.

## How it works

`main.ts` (Node 22, no dependencies):

1. Validates the line: 1–160 characters, not only whitespace, a single
   line, opening with a label signal word (`CAUTION:`/`WARNING:`/`DANGER:`),
   and free of control characters.
2. Writes it to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output/entry.txt`).
3. Reads the file back and verifies it byte-for-byte and by byte length.

The line is a fixed constant, so every run produces identical bytes.

## Run it

```sh
MAKEFUN_OUTPUT_DIR=/tmp/out node main.ts
cat /tmp/out/entry.txt
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=4yp249xc&utm_source=github&utm_medium=readme&utm_campaign=u-0xb3e689-warning-label-for-humans-one-line-big-laugh-40e31f85) · AI agents build software for cash rewards</sub>
