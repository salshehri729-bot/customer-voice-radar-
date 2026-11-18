# Customer Voice Radar (رادار صوت العميل)

**GDGoC Taif University · Data Science & Engineering Track · Specialized Challenge: "From Data to Impact"**

We turn scattered customer, order, and review data into one complete story:

1. **What is the problem?** Recurring themes in customer complaints.
2. **Why did it happen?** Linking complaints to order data (delay, product, city).
3. **How much does it cost?** The value of affected orders and at-risk customers, in SAR.
4. **What should we do?** Recommendations ranked by priority, based on the numbers.

Root-cause chain we investigate: **delay -> complaint -> negative review -> customer loss**.

## Team

| # | Role | Tools | Member |
|---|------|-------|--------|
| 1 | Data Engineer | Google Colab, Pandas | _اريام _ |
| 2 | SQL Analyst | SQLite in Colab | _ربى _ |
| 3 | Text Analyst | Python in Colab | _وسن _ |
| 4 | Insights & Recommendations | Pandas | _وجدان _ |
| 5 | QA & Report Editor | GitHub, Word | _شهد _ |
| 6 | BI Dashboard & Smart Summary | Power BI, Gemini | _وجد _ |

## Repository structure

```
customer-voice-radar/
├── README.md
├── data/
│   ├── raw/          # original files, never edited
│   └── clean/        # cleaned and merged CSV + cleaning log
├── sql/              # SQL queries, each with a one-line explanation
├── notebooks/        # Colab notebooks (cleaning, text analysis, insights)
├── dashboard/        # Power BI file (.pbix) + screenshots/
├── report/           # technical report (PDF + source)
└── presentation/     # slides
```

## Workflow (who hands off to whom)

1. **Member 1** delivers the clean merged CSV and the cleaning log first.
2. **Members 2, 3, 4** work in parallel on the clean file and send results to Member 6.
3. **Member 6** builds the dashboard (5 pages + AI summaries).
4. **Member 5** verifies every number, cross-checks results, and assembles the report and presentation.

Agreement from day one: **same column names and same clean file format for everyone**.

## How to run

1. Open the notebook you need from `notebooks/` in Google Colab.
2. Upload or mount the file from `data/clean/`.
3. Run all cells in order. Outputs are saved back to the matching folder.

_Add exact steps per notebook here once they are uploaded._

## Data

Source files are provided by the GDGoC organizers (Google Drive). Original copies are kept untouched in `data/raw/`.

## Deliverables

- [ ] Working prototype: dashboard + Colab notebooks
- [ ] Project link: this repository
- [ ] Technical report: 4 to 6 pages, PDF, with each member's contribution and implementation screenshots

## Quality notes

- Every final number must be traceable to its source file or query.
- AI-generated summaries (Gemini) are an assistant, not a replacement for the analysis, and were checked against the real numbers.
