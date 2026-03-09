# Phase Diagrams & Critical Phenomena

## Domain 17: Phase Transitions
### Source: Phase diagram list.pdf

---

## Overview

Critical phenomena visual guide: nucleation vs. spinodal, quench histories, coexistence bands (70+ regime terms).

---

## 17.1 Regime Archetypes

### Coexistence Regions
- Two-phase patches
- Three-phase junctions
- Miscibility gaps
- Spinodal zones

### Phase Topologies
- Critical points
- Triple points
- Binodal/spinodal curves
- Phase domes

---

## 17.2 Pattern Morphologies

| Mechanism | Pattern |
|-----------|---------|
| **Nucleation-Dominated** | Isolated droplets, growth fronts, impingement polygons, Ostwald ripening |
| **Spinodal** | Interpenetrating labyrinthine domains, bicontinuous networks, no isolated droplets |
| **Arrested** | Glassy frozen phases, pinned fronts, patchy coexistence |

---

## 17.3 Transition Controls

### Quench Depth
| Depth | Result |
|-------|--------|
| Shallow | Nucleation islands |
| Deep | Spinodal decomposition |
| Fast | Frozen disorder |

### Coarsening
| Variable | Effect |
|----------|--------|
| Time ↑ | Domain growth |
| Mobility ↑ | Smooth interfaces |
| Arrested | Glassy states |

### External Fields
- Alignment bias
- Striped/chevron domains
- Drifted boundaries

---

## 17.4 Procedural Recipes

### Coexistence Band
```
Define band across canvas
Allow multiphase inside
Enforce purity outside
```

### History Embedding
```
Fine texture = young/quenched
Coarse = old/annealed
Ghost lines persist
```

### Defect-First
```
Place seams before filling regions
Form triple junctions deliberately
Scars feel inevitable
```

---

## AI Prompting Keywords

```
phase diagram, critical point, triple point
binodal, spinodal, nucleation
coarsening, Ostwald ripening, quench
phase separation, coexistence, miscibility gap
```

---

*Generated for Soft Matter Physics Taxonomy - Domain 17*
