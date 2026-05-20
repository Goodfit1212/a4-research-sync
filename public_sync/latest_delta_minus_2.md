# Public Sync Delta

## sync_seq

6

## previous_seq

5

## status

latest_delta_only_scan_and_upload_rule

## instruction received

Clarify that the public safety scan should be a Python routine and that only the upload file matters. Since the workflow uploads only `latest_delta.md`, the default scan should check only that file.

## what was executed

- Updated the public sync safety scanner default target to `public_sync/latest_delta.md` only.
- Added an optional full public-sync audit mode for the minus files when explicitly needed.
- Updated workflow rules to say the default upload target is `latest_delta.md` only.
- Updated the orchestration plan to match the latest-delta-only default scan/upload workflow.

## key findings

- Routine scanning should match the upload surface.
- Checking all local public sync history on every task wastes time and is not necessary for the default handoff.
- Full public-sync scans remain available only for rotation audits or suspicious references.

## metrics

- default scan files: 1
- default upload files: 1
- default upload target: `public_sync/latest_delta.md`
- full public sync audit option: available
- broad optimisation runs: 0

## conclusion

The public sync workflow is now leaner: by default, Python scans only `latest_delta.md`, and only `latest_delta.md` is uploaded for ChatGPT handoff.

## recommended next step

Continue using the narrow public-sync safety check before publishing. Use the full public-sync audit only when the public file set changes or a suspicious reference appears.

## compact running state

- Official scoring logic remains canonical reversal-confirmation scoring.
- Current best canonical timing result remains near 50% and is not accepted.
- Model optimisation remains paused.
- Local Python orchestration skeleton exists.
- Public sync is the ChatGPT handoff channel.
- Default public upload is now only `public_sync/latest_delta.md`.
- Default safety scan checks only `public_sync/latest_delta.md`.
- Full public-sync scan is optional for audits.
- Full research memory and raw experiment history remain local only.
- If the safety scan says REVIEW_REQUIRED, do not push.
