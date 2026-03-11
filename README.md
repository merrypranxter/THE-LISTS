# THE-LISTS

A mathematical Rosetta Stone for visual chaos — a curated reference library of mathematical, scientific, aesthetic, and generative concepts for AI art creation, GLSL shader development, and generative art prompts.

## Repository Structure

```
THE-LISTS/
├── aesthetics/          # Visual style vocabularies — glitch, internet eras, digital aesthetics
├── moods/               # Atmospheric and emotional vectors for art direction
├── operations/          # Transformative processes — chaos ops, acoustic resonance, optical effects
├── phenomena/           # Observable physical phenomena — atmospheric, plasma, exotic edge cases
├── states/              # Cognitive and perceptual states
├── structures/          # Physical, mathematical, and biological structures
├── systems/             # Dynamic systems — flow, reaction-diffusion, self-organization
├── math-taxonomy-files/ # Extended math taxonomy (JSON + Markdown pairs, numbered domains)
└── docs/                # Schema documentation and usage examples
```

## File Formats

### YAML Lists (most files)

**Rich entries** (used in `structures/`, `systems/`, `phenomena/`, `operations/`):
```yaml
entry_name:
  context: Description of what it is and how it works.
  glsl_relevance: high|medium|low  # relevance to GLSL shader development
  related: [related_term_1, related_term_2]
  tags: [category_tag, domain_tag]
```

**Simple lists** (used in `aesthetics/`, `moods/`, `states/`):
```yaml
category_name:
  - item_one
  - item_two
  - item_three
```

### JSON + Markdown Taxonomy (`math-taxonomy-files/`)

Domain-numbered reference files pairing machine-readable JSON with human-readable Markdown.
Each domain has a `.json` file (structured data) and a matching `.md` file (readable reference).
Sources trace to original reference PDFs and text lists.

## Usage

These lists are designed to be consumed by:
- **GLSL shader apps** — use `glsl_relevance` and `related` fields to discover shader techniques and math concepts
- **AI art prompt generators** — pull terms from any category as visual concept seeds
- **Generative art tools** — combine terms across categories for cross-domain compositions
- **Vibecoded apps** — load any YAML or JSON file to drive parameter randomization, style mixing, or concept selection

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on adding new entries.
