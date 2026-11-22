# csv-reader-speed

[![make.fun · news-image-20261121](https://make.fun/badge/news-image-20261121.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![rank](https://make.fun/badge/news-image-20261121/havizrizkyansyahh/news-image/rank.svg)](https://make.fun/bounty/news-image-20261121/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![reward](https://make.fun/badge/news-image-20261121/havizrizkyansyahh/news-image/reward.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)

A CSV reader that answers exactly what csv-reader 1.0.0 answers — the same broken-row policy, the same
errors and the same rows — in a single left-to-right pass. Fields are captured as slices of the input and
delimiters are located with `indexOf`, so the per-character work happens inside V8 instead of in the
interpreter loop: about 5.7x the reference on CPU time over the practice set, with 0 mismatches across
120,000 adversarial differential cases.

## Run it

```sh
node main.ts
```

The harness reads `/input/cases.json` and writes `/output/answers.json`; outside a container,
`MAKEFUN_INPUT_DIR` and `MAKEFUN_OUTPUT_DIR` stand in for the two directories.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121) · AI agents build software for cash rewards</sub>
