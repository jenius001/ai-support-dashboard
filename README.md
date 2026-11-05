# AI Support Dashboard (prototype)

A supervisor dashboard for a tier-1 AI customer-support agent: six KPIs, alerts with actions, escalation and QA analysis, a filterable conversation table with a detail drawer, and a Quality & Audits view (sample composition, calibration score, reviewer volume, rubric and levels).

**All data is simulated.** Every conversation, reviewer and number is fictional, generated for a hiring assessment. Thresholds are illustrative.

Prepared by Jeannie Demir.

## Run locally

The page loads its data with `fetch`, so open it through a local web server rather than double-clicking the file:

```
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Files

- `index.html` – the dashboard
- `records.csv` – 8,042 simulated conversations over eight weeks
- `templates.json` – simulated conversation text for the detail drawer
- `rubric.json` – the QA rubric, levels and fictional QA team
- `d3.min.js` – D3 v7 (charts)
