# Usage Examples

This document provides examples of how to use the vocabulary in GLSL shaders, AI prompts, and generative art.

## GLSL Shaders

Example of a simple fragment shader using the vocabulary:
```glsl
#version 330 core

out vec4 color;

void main() {
    color = vec4(1.0, 0.5, 0.0, 1.0); // Using "color" vocabulary
}
```

## AI Prompts

Prompt examples to guide AI in generating specific outputs:

1. 
   *"Generate an abstract image inspired by the term 'luminescence'."*

2. 
   *"Create a visual representation of 'chaos' using vibrant colors and irregular shapes."*

## Generative Art

Code snippet for a generative art piece:
```javascript
function setup() {
    createCanvas(400, 400);
    noLoop();
}

function draw() {
    background(255);
    stroke(random(255), random(255), random(255)); // Using random colors
    for (let i = 0; i < 100; i++) {
        line(random(width), random(height), random(width), random(height));
    }
}
```

These examples illustrate how to integrate the vocabulary into different creative coding environments.