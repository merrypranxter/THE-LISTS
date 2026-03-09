# Perceptual Engineering & Visual Hacking

## Domain 6: Perceptual Engineering
### Source: Optical illusions notes.pdf

---

## Overview

Complete illusion taxonomy with neural mechanisms, GLSL shader implementations, and AI prompting vectors.

---

## 6.1 Neural Mechanisms & Spatial Vision

### Foveal vs Peripheral Processing

| Region | Range | Characteristics |
|--------|-------|----------------|
| Foveal | 0-2° | High-resolution, color-sensitive (foveal purple → peripheral blue) |
| Peripheral | >5° | Motion-sensitive, low-resolution |

### Top-Down Modulation
- HVAs (higher visual areas) feedback
- Recurrent processing
- Parietal-EVC gradient

### Lateral Inhibition
- **Mechanism**: Retinal ganglion cells, center-surround antagonism
- **Effects**: Edge enhancement, contrast detection

---

## 6.2 Geometric & Brightness Illusions

| Illusion | Mechanism | Parameters |
|----------|-----------|------------|
| **Fraser Spiral** | Twisted cord effect, arc tilt | Checkered background |
| **Café Wall** | Parallel lines appear tilted | Tilt 5-15°, offset 0.3-0.7× brick |
| **Müller-Lyer** | Arrowhead affects length | 20% apparent length difference |
| **Simultaneous Contrast** | Lateral inhibition | ΔL* 30-60, up to 30% shift |
| **Hermann Grid** | ON-center inhibition | Grid 2-8px, spacing 20-60px |
| **Scintillating Grid** | White dots on intersections | Contrast polarity reversal |
| **Munker-White** | Color assimilation | Interleaved stripe shifts |

---

## 6.3 Motion & Figure-Ground Phenomena

### Peripheral Drift
- **Mechanism**: Asymmetric luminance gradients (sawtooth profiles)
- **Rules**: Dark-to-light motion rule
- **Discovery**: Pupil dilation modulation (2025)

### Rotating Snakes (Kitaoka)
- Optimal: 0.5-2 cycles/degree at 8° eccentricity

### Rubin's Vase
- **Type**: Bistable perception
- **Enhancement**: Frontoparietal recruitment (3-5×)
- **Switching Rate**: 2-5 seconds

### Kanizsa Triangle
- **Type**: Modal completion
- **Neural Basis**: V2/V4 boundary completion

---

## 6.4 Moiré & Interference

- **Spatial Beat Frequency**: |S1-S2|/(S1×S2)
- **Applications**: Industrial pose estimation (6-DoF)
- **Removal**: CNN wavelet+spatial domain

---

## 6.5 AI-Generated Illusions & Creative Coding

### Phantasmagoria GAN
- Architecture: Candidate Generator + Illusion Discriminator (VTS+PQ)
- Performance: 70% correct illusion perception

### Diffusion Model Illusions
- Latent space brightness/color shifts
- Visual anagrams (rotation/inversion/frequency filtering)

### Quantum Neural Networks
- QT-DNN with quantum tunneling activation
- Models Necker cube switching

### GLSL Implementation
```glsl
// Asymmetric luminance gradients
// UV coordinate warping
// Real-time peripheral drift shaders
```

### Databending for Glitch-Illusions
- Formats: PNG/JPG/GIF/FLIF
- Methods: Hex editing, Audacity sonification

---

## GLSL Shader Recipes

### Peripheral Drift Shader
```glsl
// Asymmetric luminance gradient
float sawtooth = fract(uv.x * frequency);
float gradient = smoothstep(0.0, 1.0, sawtooth);
vec3 color = mix(darkColor, lightColor, gradient);
```

### Moiré Pattern
```glsl
float pattern1 = sin(uv.x * 50.0);
float pattern2 = sin(uv.x * 52.0);
float moire = pattern1 * pattern2;
```

---

*Generated for Perceptual Engineering Taxonomy - Domain 6*
