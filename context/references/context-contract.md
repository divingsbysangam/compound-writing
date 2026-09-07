# Context Contract

This document governs how all skills, agents, and platform integrations load context for *Divings by Sangam*.

## Priority of Context Sources

When processing writing tasks, load sources in this strict order:

1. **Explicit Prompt Instructions**: The immediate instructions given in the current conversation turn.
2. **`context/VOICE.md`**: Voice, tone, rhythm, mandatory contractions, zero em dashes, and tell cleanup rules.
3. **`context/STYLE.md`**: Structural requirements (4-part short-form, 6-beat long-form, scaffolding default, LinkedIn Koe/Shipper format).
4. **`context/DOMAIN.md`**: Salesforce release notes PDF ground truth, scratch org boundaries, and verified metrics.
5. **`context/examples/`**: Real published essays and past draft diffs.
6. **`context/references/banned_lexicon.csv`**: Lexical tell patterns.

## Rules of Engagement

- **Never invent scenes or numbers**: If scene details or data points are missing, invoke `sw-interview` to ask Sangam.
- **Scaffolding by default**: For Substack essays, output outlines, beats, tensions, and structural scaffolds unless Sangam explicitly requests a full prose draft proof.
- **Compounding updates**: When Sangam makes recurring line edits or corrects phrasing, invoke `sw-save` to update `VOICE.md` or `STYLE.md`.
