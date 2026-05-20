# Public Sync Delta

## sync_seq

2

## previous_seq

1

## status

direction_filter_hypothesis_design_complete

## instruction received

Design direction/filter hypotheses only. Do not run broad optimisation. Analyse why timing windows are near 50% under canonical reversal-confirmation scoring. Compare confirmed reversals with trend continuations using pre-confirmation conditions, rank simple candidate filters, estimate safest filters to test first, and update public sync delta. Do not push until approved.

## what was executed

- Ran a diagnostic-only comparison of confirmed reversals versus trend continuations on the current best canonical timing family.
- Compared pre-confirmation features including trend slope, volatility, distance from recent high/low, recent momentum, candle direction into the prior day, and prior move size.
- Ranked simple candidate filter hypotheses.
- Updated local research memory.
- Rotated the local public sync state so the previous public delta is now `latest_delta_minus_1.md`.
- Did not run broad optimisation.
- Did not implement a new model.
- Did not push anything.

## key findings

- Confirmed reversals and trend continuations remain very hard to separate with simple pre-confirmation features.
- Baseline reversal rate in the diagnostic set is 50.3344%.
- The best simple candidate filter improved reversal rate only to 51.1547%.
- Several intuitive filters, including exhaustion and support/resistance distance proxies, reduced reversal rate in this first diagnostic.
- Current evidence still supports the view that timing windows alone are near chance for reversal confirmation.

## metrics

- diagnostic rows: 1794
- confirmed reversal rate: 50.3344%
- trend continuation rate: 49.6656%
- best candidate filter: prior move size filter
- best candidate reversal rate: 51.1547%
- best candidate lift: +0.8203%
- best candidate coverage: 48.2720%
- low-volatility filter lift: +0.2787%
- directional momentum filter lift: +0.0158%
- trend exhaustion proxy lift: -1.9474%
- support/resistance distance proxy lift: -3.1773%

## conclusion

Simple diagnostic filters do not yet explain why canonical reversal accuracy remains near 50%. The safest filters to test first are low-complexity filters with small positive lift, but none should be treated as a reliable direction model yet.

## recommended next step

Run a small controlled filter validation phase only if approved. Start with prior move size, low-volatility regime, and directional momentum filters, and require walk-forward validation before accepting any improvement.

## compact running state

- Official scoring logic: predicted date is the reversal confirmation day; prior trading day is the expected extreme.
- Date-only proximity is not sufficient.
- Current best canonical timing result remains 50.1667% and is not accepted.
- Best diagnostic filter lift is only +0.8203%, so no direction filter is accepted yet.
- Current project understanding: timing windows are detected better than true reversal confirmations.
- Major unresolved issue: pre-confirmation direction accuracy remains near chance.
- Optimisation status: broad optimisation is paused.
- Safest filters to test first: prior move size, low volatility, directional momentum.
- Weak approaches so far: date-only matching, nearby pivot-type matching, return-led optimisation, simple timing-only search, and naive exhaustion/support-resistance proxies.
- Public sync status: local sync updated to sequence 2; no push until approved.
