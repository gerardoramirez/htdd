# Source

This folder is a copy of the HTDD Starter Kit.

Files at the kit root are this project's working copy. Fill them in here. A new copy starts at [INIT.md](INIT.md). Agents start at [AGENTS.md](AGENTS.md), which sends them to `INIT.md` while [PROJECT.yaml](PROJECT.yaml) is still unset.

[METHOD/](METHOD/) is reserved for copies of HTDD methodology. Do not write product work there. When `FOUNDATIONS/`, `METHODOLOGY/`, the canonical `HUMAN_TRUTHS/` registry, or the methodology `DISCOVERIES/` log are ready, copy those trees into the matching children of `METHOD/`. See [README.md](README.md#updating).

- Methodology: https://github.com/gerardoramirez/htdd
- Starter kit in that repository: `STARTER_KIT/`

Copied: YYYY-MM-DD

Optional commit or tag:

The hash of the methodology repository at the time of the copy. In a clone of that repository, run `git rev-parse --short HEAD`. On GitHub, copy the hash of the commit you copied.

Files this copy expects outside this folder:

- The product README contains one sentence naming this path. If a merge removes that sentence, put it back. This copy does not own any other file at the repository root.

If the starter kit later changes, merge by hand. A fresh copy must not overwrite work already written at the kit root. Refreshing `METHOD/` is safe if that folder still contains only method files.
