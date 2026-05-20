# Failure Matrix: Notice Fixture

| Scenario | Failure mode | Metric | Gate | Evidence |
| --- | --- | --- | --- | --- |
| central evidence replay | central_drift | central_coverage | block release until cited evidence is regenerated | ev_0000 |
| registrations operator packet | registrations_blindspot | registrations_latency | accept only if decision claims cite fixture evidence | ev_0007 |
| registrations operator packet | registrations_blindspot | registrations_latency | accept only if decision claims cite fixture evidence | ev_0011 |
| agents regression harness | agents_misroute | agents_precision | open a regression issue with trace and benchmark delta | ev_0014 |
| claim boundary probe | claim_gap | claim_risk | route to reviewer with evidence packet | ev_0021 |
| agents regression harness | agents_misroute | agents_precision | open a regression issue with trace and benchmark delta | ev_0022 |
| central evidence replay | central_drift | central_coverage | block release until cited evidence is regenerated | ev_0028 |
