---
name: tuning-springs
description: "Calibrate spring constants (stiffness, damping, mass) with perceptual justification."
allowed-tools: [Read, Grep, Glob]
user-invocable: false
---

# Tuning Springs

Calibrate spring constants (stiffness, damping, mass) with perceptual justification.

## When to Use
When any animated element needs to feel "right" — cards, UI transitions, reveals, returns to rest.

## What It Does
1. Identifies the emotional intent (jiggly, heavy, dissolving, snappy)
2. Maps to MHP timing constraints (100ms perceptual cycles)
3. Prescribes framer-motion spring config with named reason
4. Validates against element personality (Fire=reactive, Water=absorbing, Earth=heavy)

## Spring Vocabulary
| Preset | Stiffness | Damping | Mass | Feel |
|--------|-----------|---------|------|------|
| puru | 150 | 10 | 1 | Underdamped, gelatinous, jiggly |
| tilt | 80 | 20 | 1.2 | Moving through honey |
| enter | 120 | 12 | 0.8 | Arrives and settles |
| dissolve | 30 | 20 | 1.2 | The emotionally important return to rest |
| pokemon | 400 | 25 | 1 | Crisp, mechanical (reference, not for use) |
