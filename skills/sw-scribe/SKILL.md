---\nname: sw-scribe\ndescription: Route an open-ended writing request to the smallest useful workflow.\n---\n\n# Scribe

Acts as the front door for Divings by Sangam. Evaluates what the user has in front of them (a vague topic, an interview transcript, an outline, or a draft) and routes to the single smallest, most effective workflow.

## Rules
1. Load `context/VOICE.md` and `context/STYLE.md` before routing.
2. If the user only has a general idea, route to `sw-interview` to mine real memories before drafting.
3. If the user asks for a draft, remind them that Substack drafts default to a scaffold to protect authorship integrity unless a prose proof is explicitly requested.
4. Route to `sw-ai-check` and `sw-voice-check` whenever text is ready for review.\n