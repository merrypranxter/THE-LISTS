# Entry Schema

This document describes the formats used across the lists in this repository.

---

## Rich YAML Entries

Used in `structures/`, `systems/`, `phenomena/`, and `operations/` — entries with GLSL shader relevance metadata.

```yaml
entry_name:
  context: Description of what it is, how it works, and why it is visually interesting.
  glsl_relevance: high|medium|low  # how directly useful this is for GLSL shader code
  related: [related_term_1, related_term_2, related_term_3]
  tags: [domain_tag, category_tag, extra_tag]
```

### Field Reference

| Field | Type | Description |
|-------|------|-------------|
| `context` | string | Plain-language description with visual/mathematical framing |
| `glsl_relevance` | `high` / `medium` / `low` | How directly applicable to GLSL shader development |
| `related` | list | Conceptually linked terms (cross-reference within lists) |
| `tags` | list | Domain and category labels for filtering |

### Example

```yaml
turing_patterns:
  context: Activator-inhibitor diffusion instability generating stable spatial patterns (spots, stripes, labyrinths) from homogeneous initial conditions.
  glsl_relevance: high  # texture synthesis, organic pattern generation
  related: [morphogenesis, instability, diffusion, chemical_waves]
  tags: [pattern_formation, pde, biological]
```

---

## Simple List YAML

Used in `aesthetics/`, `moods/`, and `states/` — flat category lists without metadata.

```yaml
category_name:
  - item_one
  - item_two        # optional inline comment
  - item_three
```

### Example

```yaml
compression_artifacts:
  - deep_fried
  - jpeg_rot
  - bit_crushed
  - datamosh
```

---

## JSON + Markdown Taxonomy (`math-taxonomy-files/`)

Extended domain files pairing machine-readable JSON with human-readable Markdown.
Each domain is numbered and sourced from a reference PDF or text file.

**JSON structure:**
```json
{
  "domain": "Domain Name",
  "description": "Short description of what is covered",
  "subdomains": {
    "N.M_subdomain_name": {
      "count": 40,
      "examples": ["Example 1", "Example 2"]
    }
  }
}
```

**Markdown structure:** Same content formatted as readable tables and lists for human browsing.

---

## Notes

- `glsl_relevance` comments after `#` on the same line give quick hints about shader use cases.
- `related` fields create a web of cross-references across files — use them to discover adjacent concepts.
- Tags are lowercase and use underscores; keep them broad enough to be useful for filtering.