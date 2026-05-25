# Rent vs. Own Calculator

A free, interactive calculator that compares the long-term financial outcomes of renting vs. owning a home.

**Live site:** [rentvsown.org](https://rentvsown.org)

## What it does

This tool runs a month-by-month simulation comparing two scenarios with identical starting cash. The buyer puts the down payment into a home; the renter invests that same money. Each month, whichever party pays less in housing costs invests the difference at the assumed investment return rate.

At any point on the time horizon, you can see:

- The buyer's net worth (home equity plus investment account)
- The renter's net worth (investment portfolio)
- The crossover year — when one side first overtakes the other
- A year-by-year line chart of the comparison
- A breakdown of home value, loan balance, equity, cumulative rent paid, and PMI status

## Why most rent-vs-buy calculators fall short

Most online calculators oversimplify by ignoring opportunity cost, fixing assumptions you should be able to adjust, or hiding the levers that matter most. This one exposes every variable that materially affects the answer:

- Home cost, down payment, mortgage rate, and loan term
- Property tax, insurance, HOA, and maintenance (each adjustable)
- Inflation, home appreciation, and investment return rates
- Current rent and rent growth rate
- PMI (auto-activates when down payment is below 20%, drops at 20% equity)
- Time horizon from 5 to 40 years

Type any value directly or use the sliders. Results update live.

## Key insight

The two assumptions that move the needle the most are **home appreciation rate** vs. **investment return rate**. Because the buyer is leveraged (earning appreciation on the whole home, not just the down payment), buying often pulls ahead even when those rates are equal. When investment returns substantially exceed appreciation, renting tends to win — especially over shorter horizons.

## What's not modeled

- Closing costs (typically 2–5% of home price upfront)
- Selling costs (typically 6% on the way out)
- Mortgage interest and property tax deductions (relevant only if you itemize)
- Imputed rent / phantom income
- Geographic differences in tax law

Real-world outcomes will skew slightly toward renting for short horizons (selling costs eat into buyer's equity) and slightly toward buying for high-income itemizers in high-tax states.

## How it's built

A single self-contained HTML file. No backend, no database, no tracking. All calculation happens in your browser via JavaScript. [Chart.js](https://www.chartjs.org/) is inlined into the file so the calculator works fully offline once loaded.

To run locally, just open `index.html` in any modern browser. No build step required.

## Disclaimer

This calculator is for educational and informational purposes only. It is not financial, legal, tax, or investment advice. Always consult a qualified financial advisor, tax professional, and real estate professional before making major financial decisions.

## License

MIT — see [LICENSE](LICENSE). Free to fork, modify, and host your own version.
