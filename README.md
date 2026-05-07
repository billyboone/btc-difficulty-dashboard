# Bitcoin Difficulty Growth by Epoch

Live dashboard plotting Bitcoin's network difficulty (converted to estimated hashes required per block) on a log scale, shaded by halving epoch.

**Live:** https://thebillyboone.github.io/btc-difficulty-dashboard/

Built by [@thebillyboone](https://x.com/thebillyboone).

## Data sources

1. `mempool.space/api/v1/mining/difficulty-adjustments/all` (primary)
2. `api.blockchain.info/charts/difficulty` (fallback)
3. Manual JSON paste (last resort)

## Notes

- `hashesRequired = difficulty × 2³²`
- Difficulty adjusts every 2,016 blocks (~2 weeks), so per-adjustment data is sufficient.
- Epoch 1 (2009–2012) is excluded from the chart but kept in the summary cards — pre-ASIC era is not directly comparable.
- Y-axis is log₁₀.

## Local

Just open `index.html` in any modern browser. No build step.
