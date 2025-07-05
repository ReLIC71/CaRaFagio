# CaRaFagio - Generative Art Knowledge Compression for Claude

## History

CaRaFagio began life as CRF (Claude Reference Format) - a simple plug-in to help Claude troubleshoot ComfyUI workflows. What started as a technical reference for node connections and model parameters evolved into something more ambitious: a comprehensive knowledge compression system covering both the technical and artistic aspects of generative AI.

The name evolved from CRF to CaRaFagio (Compression and Reference Format for Automated Generative Imagery Oracle) as the scope expanded from pure technical documentation to include art history, composition theory, and creative techniques.

## What This Is

CaRaFagio is a highly compressed knowledge base that enables Claude to function as a comprehensive generative art assistant. It uses a custom symbol system to encode:

- Technical specifications for all major AI models (SD1.5, SDXL, FLUX, etc.)
- ComfyUI node architectures and workflow patterns
- Art history spanning 15 master artists and 12 movements
- Composition principles, color theory, and lighting techniques
- Hardware optimization strategies
- Common troubleshooting solutions

Current version: **v108.4** (28.4KB compressed from ~2MB of knowledge)

## Technical Details

### Compression System
- Single Unicode characters represent complex concepts
- Positional grammar: `[TYPE][SUBTYPE][VALUE][CONSTRAINTS]`
- Relationship operators show connections between concepts
- ~98% compression ratio with ~50x faster parsing

### Coverage
- **Models**: SD1.5, SDXL, SD3.5, FLUX, HiDream, Pony, IllustriousXL, OmniGen, Cosmos
- **Platforms**: ComfyUI (primary), A1111, Forge, StabilityMatrix
- **Technical**: LoRA systems, ControlNet, IPA, regional prompting, samplers, schedulers
- **Artistic**: Composition (Ω), Lighting (Λ), Color (Θ), Perspective (ϴ), Emotion (Ε)

## Usage

1. Load `CaRaFagio_v108.4.md` into a conversation with Claude
2. Claude will parse the compressed format automatically
3. Ask technical or artistic questions naturally

### Example Queries
- "My FLUX generations are slow on a 3090"
- "How do I achieve Caravaggio-style lighting in SDXL?"
- "Convert this A1111 workflow to ComfyUI nodes"
- "Why am I getting black images with SD3.5?"

## How It Works

CaRaFagio uses a symbol-based compression where:
- `α1` = SD1.5 architecture specs
- `Ω1` = Rule of thirds composition
- `λ1` = LCM speed optimization
- `ℱ1` = Memory error fixes

Claude interprets these symbols to provide context-aware assistance that combines technical accuracy with artistic knowledge.

## Repository Structure

```
/
├── CaRaFagio_v108.4.md    # Current version - use this
├── legacy/                 # Previous versions for reference
│   ├── carafagio_v2_ultra.md
│   ├── carafagio_v2_ultra_plus.md
│   └── crf_p2_legend.md
├── examples.md             # Usage examples
├── USER_GUIDE.md           # For non-technical users
└── README_TECHNICAL.md     # Implementation details
```

## Contributing

CaRaFagio is designed to be extended. When adding new content:
- Never redefine existing symbols
- Maintain backward compatibility
- Document additions in both the guide and legend
- Keep compression philosophy: maximum information density

## License

See LICENSE.md - essentially: use freely, credit appreciated, don't claim you made it.

## Limitations

- Claude's knowledge cutoff applies to base information
- New models/techniques need manual updates
- Some artistic interpretations are subjective
- Not a replacement for actual art education

## Why This Exists

Because switching between "explain like I'm five" and "give me the technical details" is exhausting. CaRaFagio lets Claude operate at whatever level you need, from debugging CUDA errors to discussing the finer points of chiaroscuro.

---

*"Art's for slackers!"* - Sir Terry Pratchett (GNU)

*The best compression is the one that preserves everything that matters.*