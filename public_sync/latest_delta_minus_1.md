# Public Sync Delta

## sync_seq

7

## previous_seq

6

## status

public_sync_rotation_upload_rule_corrected

## instruction received

Each time the latest public delta is uploaded, rotate the previous files first: move `latest_delta_minus_1.md` to `latest_delta_minus_2.md`, move `latest_delta.md` to `latest_delta_minus_1.md`, then write/upload the newest `latest_delta.md`.

## what was executed

- Corrected the workflow rule so each public sync publishes a consistent rotated set.
- Updated the local orchestration plan to match the rotation/upload rule.
- Rotated local public sync files.
- Created this new condensed public delta.
- Prepared to safety scan and publish all three public sync files together.

## key findings

- Publishing only `latest_delta.md` leaves remote minus files stale.
- The remote sync repo should receive the rotated three-file state together.
- Safety scanning should cover the files being uploaded.

## metrics

- sync_seq: 7
- previous_seq: 6
- public sync files to upload: 3
- broad optimisation runs: 0

## conclusion

Public sync should always rotate and upload the three-file state together so ChatGPT can see the latest delta plus the two previous states consistently.

## recommended next step

Use the three-file public sync state as the standard GitHub handoff after each completed task.

## compact running state

- Official scoring logic remains canonical reversal-confirmation scoring.
- Current best canonical timing result remains near 50% and is not accepted.
- Model optimisation remains paused.
- Local Python orchestration skeleton exists.
- Public sync is the ChatGPT handoff channel.
- Public sync now rotates and uploads the three-file state together.
- Safety scan covers uploaded public sync files.
- Full research memory and raw experiment history remain local only.
- If safety scan says REVIEW_REQUIRED, do not push.
- No broad optimisation should resume until approved.
