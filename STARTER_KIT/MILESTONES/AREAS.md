# Areas

One current file per product area. Each row points at the last file that touched that area. The file may live in the governing milestone or under `archive/`.

This is not a history. The predecessor named on that milestone's release entry is the one hop back.

If the only copy of a binding decision lives in an archived milestone, this map must point at that file.

A still-in-force list may name a file in this map instead of restating an exclusion. The row names the file. A milestone number is not the row.

## Troubleshooting

Start at the governing milestone, including its release entries.

Name the area involved. Open only the file this map names for that area.

If that file does not explain the failure, read that milestone's release entry, then the one predecessor it names.

Stop. Do not walk the chain. Do not read `archive/RELEASE_LOG.md`.

Go further only when a contradiction is found, a Human Truth conflicts with implementation reality, a milestone explicitly requires review, or the user asks. Even then, open only the named folder.

## Map

Add one row per area. Leave the map empty until a milestone touches an area.

| Area | Last file |
| --- | --- |
