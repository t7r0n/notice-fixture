# Notice Fixture

A per jurisdiction, per form regression harness for tax compliance agents - the release gate that lets Warp's AI agents file faster and prove it.

## Why This Exists

Warp's central claim is that AI agents file tax registrations, set up UI/SUTA, resolve tax notices, and handle quarterly filings across 10,000+ jurisdictions - at a 5 minute median filing time and <2% error rate (warp.co/a). The thing the public surface does not publish - and that any operator with a multi state payroll book will privately tell you is the actual constraint - is a trustworthy, auditable evaluation harness for those agents.

## What It Builds

- Replays synthetic `central` and `claim` cases against the project's evidence rules.
- Scores `central_coverage`, `claim_risk`, and `agents_precision` so regressions are visible in CSV and JSON.
- Plants `central drift` and `claim gap` failures as negative controls.
- Writes citation-locked decision claims; unsupported claims fail verification.
- Exports a review dashboard and demo pack for `notice-fixture` without hosted services.

## Local Run

```bash
uv sync
uv run notice-fixture all
uv run pytest -q
uv run ruff check .
```

## Outputs

- `outputs/analysis.json`
- `outputs/scenario_report.csv`
- `outputs/decision_report.md`
- `outputs/evidence_packet.md`
- `outputs/dashboard.html`
- `outputs/demo_pack.zip`

## Sources

- https://www.warp.co/a
- https://www.ycombinator.com/companies/warp
- https://www.joinwarp.com/blog/warp-yc
- https://www.warp.co/careers
- https://www.builtinnyc.com/company/warp-joinwarpcom/jobs
- https://www.checkhq.com/partners/warp
- https://www.dhrmap.com/news/new-york-based-warp-raises-18m-series-a-to-build-ai-driven-payroll-and-compliance-platform-for-startups
- https://www.linkedin.com/in/ayushsharma01/
- https://www.crunchbase.com/person/ayush-sharma-8e1a

## Boundary

This repository uses synthetic fixtures only. It has no credentials, no customer data, no outreach data, and no dependency on a hosted API.
