# Public Sync Delta

## sync_seq

9

## previous_seq

8

## status

heavy_local_canonical_search_complete

## instruction received

Start heavy local testing under the latest autonomy rules. Use local Python, canonical reversal-confirmation scoring, a constrained Gann-time search, start with 1000 trials, expand to 10000 if stable and no accepted model appears, keep full logs local only, and publish a condensed public sync delta.

## what was executed

- Completed and verified the local Python research orchestrator.
- Ran a controlled local canonical Gann-time search.
- Started with 1000 trials and expanded to 10000 after no accepted model appeared.
- Used canonical reversal-confirmation scoring as the primary score.
- Kept full trial logs local only.
- Updated local research memory with factual results.

## key findings

- No accepted model was found.
- Best canonical match rate improved above the prior controlled search but remained below the 60% acceptance threshold.
- Best candidate had strong walk-forward minimum, but primary canonical accuracy was still insufficient.
- The result suggests filters may improve stability in some slices, but not enough to accept a model.

## metrics

- logged trials: 10000
- real canonical constrained-search trials: 9995
- eligible trials with prediction count >= 100: 4552
- accepted trials: 0
- best canonical match rate: 53.3981%
- best walk-forward minimum: 70.0%
- best prediction count: 103
- best validation match rate: 55.2632%
- confirmed HIGH reversals: 25
- confirmed LOW reversals: 30
- trend continuations: 48

## conclusion

The heavy local search did not meet acceptance. The best candidate remains below the required 60% canonical match rate, so no model should be treated as accepted.

## recommended next step

Review whether the best candidate is a small-sample/filter artifact before any further expansion. Do not change scoring rules or add new theory without explicit approval.

## compact running state

- Official scoring logic remains canonical reversal-confirmation scoring.
- Heavy local orchestrated search completed.
- Current best canonical result is 53.3981%, not accepted.
- Best walk-forward minimum is 70.0%, but primary canonical rate is too low.
- Accepted model count remains zero.
- Model optimisation can continue locally under autonomy rules, but scoring/theory changes require approval.
- Full logs remain local only.
- Public sync contains condensed results only.
- Public sync rotates and uploads the three-file state together.
- Main project repo must not be pushed.
