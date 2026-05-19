# Public Sync Delta

## sync_seq

1

## previous_seq

none

## status

first_public_sync_state

## instruction received

Create canonical research workflow rules and run a small controlled canonical-scoring search. Do not run broad brute-force optimisation. Do not add new prediction theory. Do not push anything.

## what was executed

- Established a local research-memory workflow with mandatory timestamped delta logs.
- Added a clipboard-first completion rule for future local task summaries.
- Marked older non-canonical optimisation state as stale/canonical-rescored.
- Ran a bounded canonical-scoring search with 100 trials.
- Logged every trial and generated ranked results plus a walk-forward summary.
- Updated local research memory and the local bridge summary.

## key findings

- No simple timing family in the controlled search met the canonical acceptance criteria.
- The best candidate was balanced between confirmed HIGH and LOW reversals.
- Failure was not caused by one-sided reversal direction output.
- Walk-forward validation remained weak.
- The current evidence still points to timing-window detection rather than reliable reversal-confirmation prediction.

## metrics

- trials run: 100
- accepted trials: 0
- best canonical match rate: 50.1667%
- best prediction count: 1800
- confirmed HIGH reversals: 460
- confirmed LOW reversals: 443
- trend continuations: 891
- ambiguous/noise cases: 6
- no reversal/out-of-range cases: 0
- train match rate: 49.8382%
- validation match rate: 50.8865%
- walk-forward minimum match rate: 50.3012%
- bullish match rate: 49.3684%
- bearish match rate: 51.0588%
- high-volatility match rate: 50.5515%
- low-volatility match rate: 49.5787%

## conclusion

The controlled canonical search did not materially beat chance. No accepted canonical model exists yet. Current simple timing-cycle families should not be treated as a reliable turning-date prediction edge.

## recommended next step

Pause broad optimisation. Review why balanced timing predictions still score near 50% under canonical reversal-confirmation scoring, then decide whether a separate direction hypothesis or filter phase is needed.

## compact running state

- Official scoring logic: predicted date is the reversal confirmation day; the prior trading day is the expected extreme.
- A valid HIGH reversal requires price rising into the prior day and reversing down on the predicted day.
- A valid LOW reversal requires price falling into the prior day and reversing up on the predicted day.
- Date-only proximity is not sufficient.
- Current best canonical result is 50.1667% from the controlled 100-trial search.
- No canonical result has met the 60% acceptance threshold.
- Walk-forward minimum for the best result is 50.3012%, below the 52% floor.
- Current project understanding: the system detects timing windows better than true reversal confirmations.
- Major unresolved issue: direction/reversal confirmation accuracy remains near chance.
- Weak approaches so far: date-only matching, nearby pivot-type matching, return-led optimisation, and simple timing-only cycle searches.
