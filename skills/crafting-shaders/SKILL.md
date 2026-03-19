# Crafting Shaders

R3F shader recipes per Wuxing element. From CSS prototype to WebGL production.

## When to Use
When a card or UI element needs material fidelity beyond CSS blend modes.

## Element Recipes
- **Wood**: Vertex displacement along UV paths + green Fresnel rim
- **Fire**: drei `<Sparkles>` + heat distortion shader on art layer
- **Earth**: `MeshPhysicalMaterial({ transmission: 0.8, thickness: 2, ior: 1.5 })` — Urushi amber
- **Metal**: `anisotropy: 1` + faceted clearcoat normal map
- **Water**: Fresnel + noise displacement + rotating UVs (water orb technique)

## Two-Surface Architecture
- CSS Effects Lab = fast iteration, exploration
- R3F Shader Lab = production fidelity, shipping
