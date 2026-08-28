# Manual Overleaf Sync Gate

## Trigger

Load when a paper uses separate local and synchronized copies through Overleaf, Dropbox, rclone, or a similar service.

## Invariants

- Work in the normal local project copy by default, outside live synchronized directories.
- Pull and push are separate manual operations. Perform only the direction explicitly authorized by the user.
- Do not start mounts, background services, scheduled jobs, or continuous synchronization.
- Prefer in-place content updates. Do not mirror, delete destination-only files, replace whole directories, or rename synchronized content without separate authorization.
- Never place passwords, tokens, API keys, or credential files in paper or synchronization directories.

## Start Checkpoint

At the beginning of paper writing, revision, compilation, or synchronization work, remind the user to consider pulling the latest synchronized version. Do not pull merely because it was recommended. If the user continues without pulling, keep the work local and note that remote edits may be missing.

## Manual Pull

After explicit authorization:

1. Resolve and state the exact synchronized source and local destination.
2. Inspect both sides for overlapping changes.
3. Update existing local files in place and add genuinely new files.
4. Verify the intended content arrived.

Stop before overwriting when both sides changed the same file, the paths are uncertain, or login is required. Ask the user to complete authentication.

## Local Work

Continue editing the local copy after pulling. Keep temporary and generated build artifacts out of the synchronized directory unless the project requires them.

## Manual Push

At the end of paper editing, remind the user that changes remain local. After explicit push authorization:

1. Resolve and state the exact local source and synchronized destination.
2. Identify the files that will change and inspect for overlapping remote edits.
3. Update synchronized files in place while preserving destination-only files.
4. Verify propagation and report conflicts or delays.

Distinguish Git or GitHub push from paper synchronization push. Authorization for one never authorizes the other; ask when the target is unclear.
