# Operator Brief: Warp

Warp gets a local, deterministic pressure test around central, claim, and agents. The useful part is not the dashboard; it is the repeatable evidence path from fixture to failure to operator action.

## Highest-leverage checks

- central evidence replay -> block release until cited evidence is regenerated (central_coverage, evidence ev_0000).
- registrations operator packet -> accept only if decision claims cite fixture evidence (claim_risk, evidence ev_0099).
- agents regression harness -> open a regression issue with trace and benchmark delta (agents_precision, evidence ev_0022).
- claim boundary probe -> route to reviewer with evidence packet (registrations_latency, evidence ev_0121).

## What makes this useful

The workflow is intentionally local and deterministic. A reviewer can run the same fixture set, inspect the evidence IDs, open the dashboard, and see exactly why a recommendation passed, went to review, or blocked.
