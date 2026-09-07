# Compound Writing for Divings by Sangam

A context-first, compounding writing system and plugin for developing ideas, drafting, revising, stress-testing, and atomizing content without losing the writer's authentic voice.

Built for **Divings by Sangam** and packaged for **Claude Code**, **OpenAI Codex**, **Google Antigravity**, **Cursor**, **Windsurf**, and open agentic coding environments.

---

## What is Compound Writing?

Most AI writing workflows are amnesiac: you prompt an agent, correct its mistakes, polish the draft, and then start from zero on the next piece.

**Compound Writing** turns every writing session into a compounding asset:
1. **Context Before Craft**: Your persistent identity, syntax rules, editorial constraints, and domain standards live in maintained files (`VOICE.md`, `STYLE.md`, `DOMAIN.md`).
2. **Scaffolding Over Synthetic Prose**: Drafts default to statement headings, tensions, and facts. Sangam writes the sentences, protecting human voice and Substack authorship integrity.
3. **The Compounding Loop (`sw-save`)**: When you make recurring line edits or reject an AI formulation, running `sw-save` codifies that learning permanently so you never give the same feedback twice.
4. **Platform Atomization (`sw-atomize`)**: The Substack essay is the authoritative source; LinkedIn carousels (Gamma) and Koe/Shipper captions are cleanly atomized from it.

---

## Quickstart & Installation

### 1. Claude Code / Claude Desktop
Install directly via the Claude plugin system:
```bash
claude plugin add https://github.com/divingsbysangam/compound-writing
```
Or clone the repository into your project:
```bash
git clone https://github.com/divingsbysangam/compound-writing.git .claude/plugins/compound-writing
```

Once installed, all 35 skills are available as slash commands:
```text
/sw-scribe       # Master router
/sw-interview    # Mine real build memories and numbers
/sw-draft        # Generate structural scaffolds
/sw-ai-check     # Scrub AI residue, banned words, and em dashes
/sw-atomize      # Turn Substack essay into LinkedIn caption & carousel
/sw-save         # Save confirmed lessons into persistent context
```

### 2. Google Antigravity & Gemini CLI
The repository includes native `.agents/skills/` and `.agents/rules/`:
```bash
# Add as a workspace customization or copy to global config
cp -r skills/* ~/.gemini/config/skills/
```
In chat, simply type `sw-interview`, `sw-draft`, or ask: *"Use sw-ai-check on this draft."*

### 3. Cursor & Windsurf
The repository includes root [AGENTS.md](file:///Users/gellasangamesh/Downloads/Manual%20Library/Coding/Non%20SF/compound-writing-divings/AGENTS.md) and `.agents/rules/` which Cursor and Windsurf load automatically.

### 4. OpenAI Codex & ChatGPT
Recognized via `.codex-plugin/plugin.json`.

---

## The Workflow Catalog (35 `sw-*` Commands)

Run `sw-commands` to list all workflows, or `sw-help` for decision routing.

### 🧭 Orchestration
- `sw-scribe` — Front-door router: evaluates what you have and routes to the smallest useful workflow.
- `sw-emergent` — Composes custom multi-stage pipelines for unconventional essays.

### 📁 Writing Home & Compounding
- `sw-setup-project` — Initializes a piece folder with `VOICE.md`, `STYLE.md`, and `drafts/`.
- `sw-onboarding` — Calibrates or refreshes voice rules between Reflective and Technical modes.
- `sw-save` — **The Compounding Engine**: turns feedback or manual rewrite diffs into permanent updates in `VOICE.md` or `STYLE.md`.

### 💡 Ideation & Sourcing
- `sw-brainstorm` — Surfaces raw ideas in Technical/Salesforce or Reflective mode.
- `sw-interview` — Interrogates the author to extract real build memories, physical scenes, and empirical numbers. Never hallucinates.
- `sw-thesis` — Formulates **one falsifiable, arguable claim** that a knowledgeable peer could dispute.
- `sw-promise` — Clarifies reader takeaway and runs the "So What?" chain to the bottom.
- `sw-outline` — Structures material into 4-part short-form or 6-beat long-form arcs.
- `sw-hook` — Generates cold openers (concrete memory, confession, or specific result). Bans throat-clearing.
- `sw-transition` — Builds causal bridges between sections.
- `sw-analogy` — Generates Matt Levine-style physical analogies for dry architecture.
- `sw-simplify` — Strips corporate jargon into plain English without losing technical precision.

### ✍️ Drafting & Revising
- `sw-draft` — **Defaults to a scaffold, not finished prose** (protects Pangram authorship detection).
- `sw-bluf` — Checks the First Paragraph Rule (core tension landed in first 2–3 sentences).
- `sw-dev-edit` — Checks structure, stakes, symptom-before-diagnosis, and self-implication.
- `sw-line-edit` — Polishes syntax, sentence length variance, and connective flow.
- `sw-voice-check` — Audits draft against `VOICE.md` (mandatory contractions, five human signals).
- `sw-ai-check` — **Strict anti-AI purge**: zero em dashes, eliminate banned lexicon, remove structural overcompletion.
- `sw-tracks` — Removes scaffolding notes, bracketed assumptions, and process residue.
- `sw-final-pass` — Executes the 15-point pre-delivery verification checklist.

### 🔍 Pressure-Testing & Personas
- `sw-objections` — Surfaces skeptical developer and architect pushback.
- `sw-asshole` — Attacks weak or under-supported claims uncharitably.
- `sw-hemingway` — Enforces verbal economy, cuts filler (*actually, sitting, by then*), and mandates active voice.
- `sw-hitchcock` — Tests narrative tension and suspense across the beats.
- `sw-reader` — Audits first-time reader cognitive friction and unexplained jumps.
- `sw-mom` — Tests clarity for non-technical readers on reflective pieces.
- `sw-sedaris` — Identifies places for self-implication, humor, or a wry parenthetical aside.
- `sw-sorkin` — Audits dialogue snap and conversational momentum.
- `sw-vonnegut` — Enforces core storytelling fundamentals.
- `sw-panel` — Synthesizes multiple reviewer perspectives simultaneously.
- `sw-debate` — Pits conflicting editorial reviewers against each other.

### 🚀 Platform Extensions
- `sw-atomize` — Transforms approved Substack essay into a **Koe/Shipper LinkedIn caption** (8–14 word bold claim, no closing question, PascalCase hashtags) + **Gamma carousel slide headings**.
- `sw-sf-check` — Cross-references technical and release claims against the official Salesforce Release Notes PDF and verifies dev org boundaries.

---

## Core Invariants

1. **Zero Em Dashes**: Absolute ban. Use hyphens, commas, colons, semicolons, or periods.
2. **Contractions Always**: "Don't", not "do not"; "couldn't", not "could not".
3. **Scaffolding by Default**: Substack drafts default to outlines, beats, tensions, and required facts. Sangam writes the sentences.
4. **Nothing Invented**: All scene details, metrics, and quotes are sourced strictly from memory via `sw-interview`.
5. **Salesforce Truth**: The release notes PDF is the sole source of truth for release claims.

---

## License

MIT © Sangam Gella
