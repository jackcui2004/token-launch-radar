# token-launch-radar

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/jackcui2004/token-launch-radar/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/jackcui2004/token-launch-radar/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

Token Radar ranks the 198 pre-token protocols in DefiLlama's sealed snapshot by implied launch value, and hands each one a concrete seven-step farm plan. The value model is a comparable multiple: each category is priced off the median market-cap-to-TVL of the live-token protocols in that same category, taken from the snapshot itself, then adjusted by seven-day growth, age with no token, and chain count. No protocol name is special-cased. The dashboard is a static page that renders offline: a sortable, filterable board, a detail view for every protocol with the model's own inputs, and a live-token view set aside from the ranking.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input input/snapshot.json
```

`input/snapshot.json` is the competition kit's sealed snapshot. The program reads it, writes the ranked board to `out/board.json`, the dashboard's data to `out/data.js`, and copies `dashboard/` and `screenshots/` to `out/`, then writes `out/dossier.json` with the vendored make.fun library. Open `out/dashboard/index.html` in a browser to use the board.

---

<sub>Entered on [make.fun](https://make.fun/?ref=rwj8kpnw&utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards</sub>
