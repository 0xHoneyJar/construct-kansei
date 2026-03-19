# Material Physics

Fresnel, IOR, transmission, thin-film interference recipes for digital materials.

## When to Use
When a surface needs to feel like a specific physical material — amber, ceramic, silk, metal.

## The Internal Volume Thesis
Chrome reflects from outside. Amber glows from inside.
`MeshPhysicalMaterial({ transmission: 0.8, thickness: 2, ior: 1.5 })` = Urushi lacquer.

## Key Parameters
| Material | IOR | Transmission | Roughness | Key Property |
|----------|-----|-------------|-----------|-------------|
| Amber/Honey | 1.50 | 0.8 | 0.15 | Internal warm shift |
| Ceramic | 1.50 | 0.0 | 0.4 | Diffuse warm reflection |
| Silk | 1.50 | 0.0 | 0.3 | Anisotropic highlight |
| Water | 1.33 | 0.95 | 0.05 | Caustic refraction |
| Crystal | 2.42 | 0.9 | 0.0 | Prismatic dispersion |

## OKLCH Safety
Chroma MUST be < 0.15 in any blend-mode context. Warm tones (hue 20-90) with chroma > 0.17 clip violently through RGB blend math.
