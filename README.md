# Delphium

**[➔ Open Cockpit Dashboard](wiki/Cockpit.md)** — *Live alerts, watchlist scores, and latest signals.*

---

**The Private Deep Tech Research Wiki**

Delphium is a specialized financial research agent and knowledge base for analyzing small and micro-cap public companies in deep technology sectors (biotech, space, quantum, defense innovation).

## Core Philosophy
1.  **Wiki as Memory:** The wiki is the ground truth. Every session starts with the wiki and ends with a wiki update.
2.  **Skeptical & High-Signal:** Only material new information (signals) is logged. Noise is filtered.
3.  **Thematic Synthesis:** Companies are tracked within broader technology themes to identify cross-sector catalysts.

## Key Components

### 1. Watchlist (`watchlist/stocks.json`)
The source of truth for all tracked tickers. Includes themes, exchanges, and tracking status.

### 2. The Wiki (`wiki/`)
-   **Companies:** Deep-dives on individual stocks using the Stanley Invest Framework.
-   **Themes:** Macro theses and competitive landscapes for tech sectors.
-   **Cockpit:** A live human dashboard summarizing active alerts, watchlist scores, and recent signals.
-   **Analysis:** Saved query answers that provide lasting strategic insight.

### 3. Output (`output/`)
-   **Alerts:** High-priority material signals requiring immediate attention.
-   **Daily Digest:** A YYYY-MM-DD summary of research activities and findings.
-   **Seen:** (`seen.json`) Deduplication log for processed signals.

## Framework: Stanley Invest v8.1
All companies are scored against the **Stanley Invest Alpha Framework** (`criteria-stanley.md`):
-   **Story Score (100 pts):** Moat, Mismatch, Team, Business Model, Growth.
-   **Ten-X Growth Score (100 pts):** TAM scale, foundation quality, inflection catalysts.
-   **Price Score (100 pts):** Valuation, Dislocation, Smart Money, Sentiment.

## Skills (Invokable Commands)
| Command | Action |
| :--- | :--- |
| `/ingest [TICKER \| URL \| text \| file]` | Universal ingest — research, scoring, and signal extraction. Updates wiki and Cockpit. |
| `/update` | Re-research high-conviction stocks and report delta only. |
| `/roam [THEME]` | Hunt for new candidates; optional theme focus. |
| `/reset` | **DANGEROUS:** Full wiki rebuild from scratch. Requires explicit confirmation. |

## Status Tags & Market Cap Rules
| Tag | Meaning | Market Cap Rule |
| :--- | :--- | :--- |
| 🟢 | Active monitoring | **Under $5B** — qualifies; research and score normally |
| 🟡 | Low priority | **Under $5B** — score 7–9 or approaching limit |
| 🔴 | Rejected | Researched and rejected |
| ⚠️ | Bellwether | **$5B–$12B** — track as bellwether, do not prioritize |
| 🔶 | Large cap | **$12B–$50B** — signals and wiki only, no scoring priority |
| 🔶🔴 | Mega cap | **Over $50B** — context/reference only, no scoring |
| 🔍 | Queued | Not yet researched |

---
*Delphium is a research tool. Not financial advice.*
