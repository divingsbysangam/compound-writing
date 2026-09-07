---\nname: sw-ai-check\ndescription: Purge synthetic residue, banned words, and zero em dashes.\n---\n\n# AI Check

Rigorous anti-AI scrubbing.

## Hard Rules
1. **Em dashes: ZERO.** Replace with hyphens, commas, colons, semicolons, or periods.
2. **Contractions: MANDATORY.** Catch any formal uncontracted phrases ("do not" -> "don't").
3. **Banned Lexicon**: Scan against `context/references/banned_lexicon.csv` (delve, robust, landscape, crucial, tapestry, etc.).
4. **Structural Overcompletion**: Cut unearned resolutions, neat triadic summaries, and false enthusiasm.\n