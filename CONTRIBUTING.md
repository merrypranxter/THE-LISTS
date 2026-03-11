# Contributing to THE-LISTS

Thank you for your interest in contributing! Here's how to add or improve entries.

---

## Adding a Rich YAML Entry

Rich entries belong in `structures/`, `systems/`, `phenomena/`, or `operations/`.

Each entry requires four fields:

```yaml
your_term_name:
  context: What it is, how it works, and what makes it visually/mathematically interesting.
  glsl_relevance: high|medium|low  # how directly useful for GLSL shader development
  related: [related_term_1, related_term_2]
  tags: [domain_tag, category_tag]
```

**Guidelines:**
- Use `snake_case` for entry names
- Keep `context` to 1–2 sentences focused on visual/mathematical properties
- Set `glsl_relevance` based on direct shader applicability:
  - `high` — standard technique, directly implements in fragment/vertex shaders
  - `medium` — useful concept with some shader application
  - `low` — theoretical; valuable as a concept seed but rarely coded directly
- `related` should reference other terms that already exist in the lists
- `tags` should use lowercase with underscores

---

## Adding a Simple List Entry

Simple list entries belong in `aesthetics/`, `moods/`, or `states/`.

```yaml
category_name:
  - new_item_one
  - new_item_two   # optional inline description
```

---

## Adding to `math-taxonomy-files/`

Each domain in `math-taxonomy-files/` has a paired `.json` and `.md` file.
If adding a new domain, create **both files** with matching names.

---

## Submission Process

1. Create a new branch for your changes
2. Add or modify entries following the format above
3. Submit a pull request describing what you added and why it belongs

Thank you for contributing!
