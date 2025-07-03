# CaRaFagio Examples

## Basic Symbol Combinations

### Portrait in Rembrandt Style
```
Input: Ω1+Λ1+Θ7+Ζ3+Ν1+Ε2+Η5
Translation: Rule of thirds + Chiaroscuro + Warm/cool temperature + Glazing + Alla prima + Melancholic + Rembrandt

Model Outputs:
- SD1.5: "(portrait:1.2), rembrandt lighting, chiaroscuro, warm tones, (melancholic mood:1.1), masterpiece, best quality"
- FLUX: "A melancholic portrait in Rembrandt's style with dramatic chiaroscuro lighting and warm golden tones"
- Pony: "score_9, score_8_up, portrait, rembrandt_style, chiaroscuro, warm_colors, melancholic_expression"
```

### Cyberpunk Cityscape
```
Input: Ϟ2+Ω4+Λ2+Θ8+Ε1+ϴ3
Translation: Cyberpunk aesthetic + Leading lines + Tenebrism + High saturation + Sublime emotion + 3-point perspective

Model Outputs:
- SD1.5: "(cyberpunk city:1.3), neon lights, dark atmosphere, (dramatic perspective:1.2), high saturation"
- FLUX: "A sublime cyberpunk cityscape with dramatic three-point perspective, neon-lit darkness contrasting vivid saturated colors"
```

### Ukiyo-e Landscape
```
Input: Ϙ1+Ω2+Θ6+Ζ5+Λ6+Κ⧑
Translation: Ukiyo-e tradition + Golden ratio + Monochromatic + Pointillism technique + Ambient light + Romantic period influence

Model Outputs:
- SD1.5: "(ukiyo-e style:1.3), woodblock print, monochromatic blue, mount fuji, floating world"
- FLUX: "Traditional Japanese ukiyo-e landscape with golden ratio composition in monochromatic blue tones"
```

## Using Macros

### Epic Fantasy Scene
```
Macro: EPIC_FANTASY
Expands to: VANGOGH_STYLE+DARK_GOTHIC+α4+ψ4
Full expansion: Ω4+Θ3+Ζ2+Ν2+Ψ3+Ε3+Η8+Λ2+Θ7+Ε7+Σheavy+low_key+α4+ψ4

Result: Van Gogh's swirling style with dark gothic atmosphere on FLUX with CFG 4
```

### Street Art Portrait
```
Macro: STREET_REALISM
Expands to: BANKSY_STYLE+PHOTOREALISTIC+κ2+Ϡ1
Full expansion: Ω3+Λ2+Θ6+ΖA+Ν4+ΨB+ΗF+Ω1+Λ4+Θ9+Ζ3+◉50+◎f5.6+κ2+Ϡ1

Result: Banksy's stencil style with photorealistic rendering, openpose control, and LoRA adaptation
```

## Complex Workflows

### Multi-Stage Upscale
```
Input: ω8+ω4
Translation: Cascade workflow + Upscale workflow
Process: Generate at low res with SD3.5 → Pass to SDXL → ESRGAN 4x upscale

CaRaFagio Chain: α3+Ω2+Λ6→α2+υ2→ESRGAN×4
```

### Regional Prompt with LoRA
```
Input: ω7+Ϡ1+MACRO:MONET_STYLE
Translation: Regional workflow + LoRA adaptation + Monet style preset

Implementation:
- Region 1: Ω2+Λ8+Θ2 (Golden ratio + Soft light + Analogous colors)
- Region 2: Ζ4+Ν2+Ψ1 (Scumbling + Broken color + Impressionism)
- LoRA: r=16, α=0.8, style transfer mode
```

## Model-Specific Examples

### For Pony Diffusion
```
Input: α7+Ε6+Ψ8+Ω1
Auto-generated: "score_9, score_8_up, score_7_up, joyful, pop_art, rule_of_thirds, bright_colors, source_anime"
```

### For FLUX Dev
```
Input: α4+Λ1+Η4+Ε5
Auto-generated: "A dramatic scene in Caravaggio's distinctive chiaroscuro style, with intense contrast between light and shadow creating emotional tension"
```

### For SD 3.5
```
Input: α3+Ω2+Θ3+Ζ1
Auto-generated: "Golden spiral composition with triadic color harmony, painted with sfumato technique for atmospheric depth"
Note: No negative prompt (not supported in SD3.5)
```

## Combining Technical and Artistic

### Fast Quality Portrait
```
Input: λ1+α2+Ω1+Λ4+MACRO:REMBRANDT_STYLE
Translation: LCM speed + SDXL + Rule of thirds + Key lighting + Rembrandt preset
Settings: 4-8 steps, CFG 1, LCM sampler
Time: ~2 seconds for 1024x1024
```

### Maximum Quality Landscape
```
Input: µ3+α5+CHAIN_LANDSCAPE+steps50
Translation: High quality sampler + HunyuanDiT + Landscape chain + 50 steps
Settings: DPM++ 2M Karras, CFG 4.5, 50 steps
Time: ~60 seconds for 1024x1024
```

## Tips for Creating CaRaFagio Chains

1. **Start with composition (Ω)** - This sets your fundamental structure
2. **Add lighting (Λ)** - This creates mood and dimension  
3. **Choose color theory (Θ)** - This sets emotional tone
4. **Select technique (Ζ)** - This defines execution style
5. **Include emotion (Ε)** - This gives the piece soul
6. **Reference masters/periods (Η/Κ)** - This provides stylistic grounding

## Common Patterns

### Portrait Formula
`Ω1+Λ4+Λ5+Θ[6-7]+Ν5+Ε[2,4,8]`
(Rule of thirds + Key/Fill light + Mono/Warm colors + Feathering + Melancholic/Serene/Elegant)

### Landscape Formula  
`Ω2+Λ6+Θ2+ϴ4+Ζ4+Ε[1,4]`
(Golden ratio + Ambient light + Analogous colors + Atmospheric perspective + Scumbling + Sublime/Serene)

### Action Scene Formula
`Ω3+Λ7+Θ1+ϴ7+Π+Ε[3,5]`
(Diagonal composition + Direct light + Complementary colors + Forced perspective + Movement + Passionate/Dramatic)

Remember: CaRaFagio is meant to be fluid. These examples are starting points - experiment with your own combinations!