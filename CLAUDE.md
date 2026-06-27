# CLAUDE.md

See AGENTS.md for the operating manual. It is the schema this repo's agent
follows to maintain the lore and systems wikis.

## Nothing is locked
Green-field project: no users, no shipped versions, nothing locked in. Do not add
backward-compatibility, migration notes, deprecation shims, or "supersedes the old
X" history — when something changes, change it in place as if it had always been
that way. Only record a decision (DDR/ADR) when a future agent could plausibly
re-make it *differently*; never to preserve history for its own sake.
