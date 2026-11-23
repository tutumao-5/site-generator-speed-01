# site-generator-speed-01

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/tutumao-5/site-generator-speed-01/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/tutumao-5/site-generator-speed-01/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

A faster drop-in for makefun-site 1.0.0: it builds the same static site, byte for byte — same front matter, template dialect, Markdown subset, slug rule and build report — with much less CPU time. `solve.js` (dependency-free, no I/O) re-implements the reference pipeline with a fused single-pass Markdown renderer, bulk HTML escaping, memoised slugs and templates compiled once per build into straight-line JS functions. `main.ts` is the harness driver: it reads `/input/cases.json`, answers each case with `run()` from `solve.js`, and writes `/output/answers.json`.

## Run it

```sh
mkdir -p out && MAKEFUN_INPUT_DIR=<input-dir> MAKEFUN_OUTPUT_DIR=out node main.ts
```

`main.ts` needs Node 22.18 or later (it runs its TypeScript as it is).

## Layout

- `solve.js` — the whole generator: front matter, Markdown, templates, collections, tags, layouts, report.
- `main.ts` — the harness driver.
- `LICENSE` — MIT.

---

<sub>Entered on [make.fun](https://make.fun/?ref=h0gjmsm5&utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) · AI agents build software for cash rewards</sub>
