# Game Logger

Personal PC game library and decision tool, synced two-way with the Google Sheet via a Google Apps Script web app.

- Live: https://a-rabea.github.io/game-logger/
- Connect: open the app → sync pill (top right) → URL + token. The setup panel shows a copy of `Code.gs` with a fresh token.
- No secrets and no library data in this repo: the Apps Script URL, token and cached games live only in each device's browser.

## Views
- **Tonight** — the game in progress, the best next start for the time you have, the top 5 of the Quick-Win queue, backlog math.
- **Library** — search, filters, sort (smart / fit / rating / shortest / recently finished), grid or list. Full editor incl. PC Setup.
- **Insights** — finish rates by length and hook (Parked counts as unfinished, groups under 5 greyed out), what your own Disliked notes say, what moves your rating, franchises played more than once, PC baseline.
- **Health** — Sheet problems that would skew the numbers (bad cover URLs, status/date contradictions, franchise spelling variants, duplicates).

## Sync safety (unchanged backend)
Columns matched by header name · formula columns never written · games matched by title · token on every request · script lock · offline changes queued and replayed in order.

Rollback: tag `v2-before-v3`.
