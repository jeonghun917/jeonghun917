# Jeonghun Mun

I built a control plane in the first place because of shitty agent memory and constant session changes.
140 PRs later, the part that worked was the simplest one, so I shipped it on its own:

### [readfirst](https://github.com/jeonghun917/readfirst): what to read and check before you change a file

One file next to the code holds the rules, traps and checks only your team knows. `npx readfirst read <file>`
hands them to you or your coding agent right before an edit (a Claude Code hook, MCP for Cursor and Codex, or Cursor
rules exported from the same map), and a GitHub Action fails the PR when the map falls behind the code.
`readfirst find` shows what already exists before an agent writes it again; `readfirst audit` shows what the map no
longer sees. MIT, no dependencies, no model calls.
Making maps for open source projects turned up real bugs, reported to saleor, wagtail, Tandoor and mealie.
[Site](https://readfirst-cloud.vercel.app) · [npm](https://www.npmjs.com/package/readfirst) · [Marketplace](https://github.com/marketplace/actions/readfirst-map-check)

### [Welsmere](https://www.welsmere.app): a British-English speaking coach for Korean and Japanese learners

Learners talk by voice: role-plays of everyday and work situations, goal-based lessons, a daily UK course for living
in Britain, IELTS mock tests, and spaced review of their own sentences. Every talk ends in a result sheet with
corrected sentences, expressions to try, phoneme-level pronunciation feedback with their intonation drawn against the
coach's British voice, and a rough CEFR or IELTS level. Live, with paying users.

### [TTS Blind Eval Studio](https://github.com/jeonghun917/tts-blind-eval-studio): blind listening tests for text-to-speech

A small CPU-only tool for comparing TTS candidates without knowing which model made which clip. Candidate names stay
hidden until the reveal, labels and order are randomised from a seed, and the prompts and rating rubric are locked to a
versioned protocol so they can't drift between evaluations. No model weights, datasets, API keys or GPU needed.

Current work includes:

- AI Development Control Plane — continuity, bounded execution, validation, review, and promotion
- Ars Mentis / VELA — persistent AI continuity
- Pharos Orbis — provenance-grounded information systems
- C3 — speech and interaction systems
- Ars Bellum — simulation and game systems

Public notes:
- [AI Development Control Plane](https://github.com/jeonghun917/ai-development-control-plane): why readfirst exists, and the 140 PRs before it

Most production repositories are private.
