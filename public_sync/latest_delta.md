# Public Sync Delta

## sync_seq

12

## previous_seq

11

## status

focused_robustness_45_60_72_complete

## instruction received

Run focused robustness testing around the 45/60/72 trading-cycle high-volatility family. Do not accept the model yet, do not change scoring rules, and do not add new theory. Test neighbouring cycle lengths, volatility threshold variations, pivot sensitivity, duplicate merge windows, confirmation filters, and minimum prediction-count thresholds. Keep full logs local and update condensed public sync after completion.

## what was executed

- Added and ran a focused local robustness runner.
- Reused canonical reversal-confirmation scoring.
- Tested neighbouring Gann-time variants around the 45/60/72 trading-cycle high-volatility family.
- Stopped after 82750 checkpointed variants because the full generated grid was much larger and the result already answered the immediate robustness question.
- Kept full trial logs local only.
- Updated local research memory.

## key findings

- A near-promising cluster exists.
- Best ranked robustness variant reached 61.6487% canonical match rate with 60.7843% walk-forward minimum.
- Positive variants are sparse.
- Most neighbouring variants collapsed under the robustness floor.
- The strongest cluster shifted from 45/60/72 to nearby 42/60/69, still within the tested neighbourhood.

## metrics

- tested variants: 82750
- near-promising variants: 408
- near-promising share: 0.4931%
- collapse variants: 80246
- collapse share: 96.9740%
- best ranked canonical match rate: 61.6487%
- best ranked walk-forward minimum: 60.7843%
- best ranked prediction count: 279
- best ranked validation match rate: 60.8108%
- best ranked confirmed HIGH reversals: 68
- best ranked confirmed LOW reversals: 104
- best ranked bullish match rate: 62.2642%
- best ranked bearish match rate: 61.2717%
- highest canonical-rate variant: 62.4242%

## conclusion

The family is not broadly robust, but a sparse high-volatility neighbouring cluster is promising enough for narrower second-pass robustness. No model is accepted yet.

## recommended next step

Run a narrower second-pass robustness test around 42/60/69 and 42/60/72 trading cycles, duplicate merge day 3, pivot sensitivity 2.75-3.5, and volatility thresholds 0.60-0.65.

## compact running state

- Official scoring remains canonical reversal-confirmation scoring.
- Full constrained Gann-time grid best was 58.9041%, not accepted.
- Focused robustness found a sparse cluster above 60%.
- Current best robustness variant is 61.6487% canonical with 60.7843% walk-forward minimum.
- Near-promising share is only 0.4931%, so broad robustness is weak.
- Best cluster is high-volatility trading-cycle 42/60/69 neighbourhood.
- Full logs remain local only.
- Public sync contains condensed sanitized results only.
- No scoring rule change or new theory was added.
- Main project repo must not be pushed.
