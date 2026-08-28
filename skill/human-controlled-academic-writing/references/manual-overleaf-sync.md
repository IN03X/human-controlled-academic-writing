# Manual Overleaf Sync

Use this card when a paper project has a local working copy and a separate synchronized copy connected to Overleaf through Dropbox, rclone, or a similar service.

## Default Boundary

- Work in a normal local project directory by default, outside any live Dropbox, Overleaf, rclone mount, or other synchronized directory.
- Treat the synchronized directory as a transfer boundary. Do not edit, copy into, pull from, or otherwise change it until the user explicitly asks for that direction of synchronization.
- Use the project's configured synchronization directory, which may be under `runbang/`. Do not infer that the current Codex workspace is the sync directory.
- Do not start rclone mounts, background services, scheduled jobs, or continuous synchronization. Use a manual, one-shot operation only after explicit authorization.

## Start-of-Task Pull Checkpoint

At the beginning of paper writing, revision, compilation, or synchronization work, remind the user that the latest paper may need to be pulled into the local working copy.

- Do not perform the pull merely because it was mentioned or recommended.
- Pull only when the user explicitly says to pull, download, sync down, or otherwise authorizes that operation.
- If the user chooses to continue without pulling, keep all work local and briefly note that the local copy may not include the newest remote edits.

## Manual Pull

Before pulling:

1. Resolve and state the exact synchronized source and local destination.
2. Inspect both sides for changes that could conflict.
3. If both sides changed the same file or the direction is ambiguous, stop and ask the user before overwriting anything.

During the pull, update existing files in place and add genuinely new files. Do not delete destination-only files, replace a directory wholesale, or use mirror operations with deletion semantics unless the user separately authorizes the reviewed deletion set.

If authentication, OAuth, a password, or an account login is required, stop and ask the user to complete it. Never write passwords, tokens, API keys, or credential files into a paper project or synchronized directory.

## Local Editing

- After a pull, continue work only in the local working copy unless the user explicitly requests direct synchronized-folder editing.
- Prefer modifying file contents over deleting and recreating files. Avoid moves and renames when an in-place edit can achieve the same result.
- Keep generated files and temporary build artifacts out of the synchronized directory unless the project explicitly requires them.

## Manual Push

At the end of a paper-editing task, remind the user that the changes remain local and ask whether they want to push or sync them to Overleaf.

Push only after explicit authorization. Before pushing, identify the exact local source, synchronized destination, and files that will change. Update files in place, preserve destination-only files, and stop on unclear two-sided changes. Afterward, verify that the synchronized copy received the intended content and report any conflict or delayed propagation.

When the user says `push`, distinguish a Git/GitHub push from a paper synchronization push. If the target is not clear from context, ask. Authorization for one does not authorize the other.

## Stop Conditions

Pause and ask the user when any of these occurs:

- source or destination path is uncertain;
- both copies contain overlapping changes;
- the operation would delete, replace, move, or rename synchronized content;
- login or credential input is required;
- a background or continuous synchronization service would need to be enabled.
