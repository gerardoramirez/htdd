# Project Structure

Every HTDD project begins with the same architecture.

Not because folders matter.

Because consistency allows the methodology to scale.

The destination is a convention, not a requirement. Recommended: `docs/htdd/`. Also valid: `docs/`, `htdd/`, `design/htdd/`, or any path the team already uses for product writing. After the copy, one sentence in the product README should name the path.

```text
<destination>/
  README.md
  SOURCE.md
  AGENTS.md
  PROJECT_BOOTSTRAP.md
  HUMAN_TRUTH_DISCOVERY.md
  HUMAN_TRUTHS/
  PRODUCT_PRINCIPLES.md
  ETHICAL_AI_PRINCIPLES.md
  EXPERIENCE_BOARDS/
  DISCOVERIES/
  MILESTONES/
    README.md
    CURRENT.md
    RELEASE_LOG.md
    AREAS.md
    001_EXAMPLE_MILESTONE/
      MILESTONE_SUMMARY.md
      BOARD_SNAPSHOT.md
      implementation_artifacts/
    archive/
      README.md
      RELEASE_LOG.md
  CHECKLISTS/
  LESSONS_LEARNED.md
  METHOD/
    FOUNDATIONS/
    METHODOLOGY/
    HUMAN_TRUTHS/
    DISCOVERIES/
```

Files at the destination root are the project's living files. They come from a one-time copy of `STARTER_KIT/`.

Point `CURRENT.md` at a milestone only after that folder has `MILESTONE_SUMMARY.md` and a short still-in-force list. The list names the exclusions this product binds. A later milestone restates the exclusions that remain from its predecessor, or names the predecessor file in `AREAS.md`. A sentence that only names the predecessor is not that list. A first milestone names the exclusions it binds. Do not copy another product's exclusions into the list. `001_EXAMPLE_MILESTONE` is a template until a project copies it and writes that list.

`METHOD/` is a reserved snapshot. No product writing. When `FOUNDATIONS/`, `METHODOLOGY/`, the canonical `HUMAN_TRUTHS/` registry, or the methodology `DISCOVERIES/` log are ready, copy those trees from the HTDD repository into the matching children of `METHOD/`. Do not copy them into the destination root.

How to copy and update: [STARTER_KIT/README.md](../STARTER_KIT/README.md).
