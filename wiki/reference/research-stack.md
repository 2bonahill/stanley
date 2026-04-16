# Research Stack
Sources to use when researching any ticker. Run parallel fetches where possible.

## Financials & Market Data
- **stockanalysis.com** — `https://stockanalysis.com/stocks/[TICKER]/` — market cap, revenue TTM, shares, price. Most reliable for WebFetch; primary source.
- **Finviz** — `https://finviz.com/quote.ashx?t=[TICKER]` — fundamentals, analyst ratings, insider table. Fast cross-check.
- **Yahoo Finance quote** — `https://finance.yahoo.com/quote/[TICKER]/` — price, 52-week range. Falls back to stockanalysis if dynamic loading fails.
- **Yahoo Finance profile** — `https://finance.yahoo.com/quote/[TICKER]/profile/` — business description, leadership names.
- **macrotrends.net** — `https://www.macrotrends.net/stocks/charts/[TICKER]/[company-name]/market-cap` — historical cap trend.

## Leadership & Scientific Team
- **Company website /about or /leadership** — most reliable for confirmed bios.
- **Crunchbase** — `https://www.crunchbase.com/organization/[company-name]` — founding date, founders, funding history.
- **Web search** — `"[Name] PhD [Company] CEO"` — confirm academic credentials.

## Insider Trading & Ownership
- **OpenInsider** — `http://openinsider.com/[TICKER]` — full buy/sell history, dollar amounts, % ownership change. Most detailed.
- **Finviz insider table** — `https://finviz.com/quote.ashx?t=[TICKER]` — quick first look, same page as fundamentals.
- **Yahoo Finance insider** — `https://finance.yahoo.com/quote/[TICKER]/insider-transactions/` — aggregated activity.

## Patents & IP
- **Google Patents** — `https://patents.google.com/?assignee=[Company+Name]` — count, recency, technology areas.
- **Justia Patents** — `https://patents.justia.com/assignee/[company-name]` — quick overview.

## Pipeline & Clinical Trials (Biotech)
- **ClinicalTrials.gov** — `https://clinicaltrials.gov/search?term=[Company]` — active trials, phase, status, enrollment.
- **SEC EDGAR 8-K search** — `https://www.sec.gov/cgi-bin/browse-edgar?action=getcompany&company=[TICKER]&type=8-K` — material events (partnerships, trial results, FDA decisions).
- **SEC EDGAR Company Facts JSON** — `https://data.sec.gov/api/xbrl/companyfacts/CIK[CIK].json` — clean structured financials. Find CIK via `https://www.sec.gov/cgi-bin/browse-edgar?company=[TICKER]&action=getcompany`.

## News & Social Signals
- **stockanalysis.com news** — `https://stockanalysis.com/stocks/[TICKER]/news/` — recent headlines.
- **Yahoo Finance news** — `https://finance.yahoo.com/quote/[TICKER]/news/` — fallback.
- **Web search** — `"[TICKER] [Company] news 2026"` — catch anything not in the above.
- **Twitter/X** — check `wiki/twitter-intel.md` for existing signals before fetching live.
