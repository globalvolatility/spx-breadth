# SPX Breadth Archive

Daily S&P 500 market-breadth readings for [Global Volatility Fund](https://globalvolatilityfund.com),
published after every trading day.

Served by GitHub Pages at **https://dashboard.globalvolatilityfund.com**.

- `_-x-nAkYzYBIMzzUjdVThA/` — the dated reports (`breadth_YYYY-MM-DD.html` + `.png`)
  plus `index.html` (the browsable archive) and `latest.html` (redirect to the newest).
  The folder name is kept from the previous GoDaddy hosting so that links already
  emailed out continue to resolve.
- `.nojekyll` — required: GitHub Pages would otherwise skip the report folder,
  because Jekyll ignores paths beginning with an underscore.
- `CNAME` — the custom domain.

Reports are generated and pushed automatically each evening by
`bin/spx-breadth-evening-email.sh` on the local machine.
