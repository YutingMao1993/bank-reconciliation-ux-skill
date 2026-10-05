# Bank Reconciliation UX skills

A Codex skill for designing, building, and reviewing AI-assisted bank reconciliation workflows. It covers exception handling, explainable match suggestions, human confirmation, progress, and auditability.

The repository also includes **Maya — Bank Reconciliation User**, a simulated participant for user interviews and usability testing. Maya answers in character and thinks aloud while working through supplied screens or prototypes. She stays in participant mode until you ask for a debrief or design recommendations.

## Install

In Codex, ask:

> Use the skill-installer skill to install `bank-reconciliation-ux` from `YutingMao1993/bank-reconciliation-ux-skill`, path `bank-reconciliation-ux`.

Or use the skill-installer helper included with Codex:

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo YutingMao1993/bank-reconciliation-ux-skill \
  --path bank-reconciliation-ux
```

Restart Codex or start a new turn after installation. The skill activates for bank reconciliation UX tasks; you can also mention `$bank-reconciliation-ux` explicitly.

## Maya user simulation

In Codex, ask:

> Use the skill-installer skill to install `maya-bank-reconciliation` from `YutingMao1993/bank-reconciliation-ux-skill`, path `maya-bank-reconciliation`.

After installation, invoke it with a screen, prototype, or workflow:

> Use $maya-bank-reconciliation. You are Maya. I'll ask interview questions and show you screens. Answer in character and think aloud.

Maya is a staff accountant at a 120-person software company, working through 14 unmatched transactions in Campfire on the third business day of month-end close. She uses visible evidence, explains her accounting decisions, and remembers what she has learned during the session without inventing transactions or interface details.

Example follow-up questions:

- “What would you do first?”
- “What does this suggested match mean to you?”
- “What would you expect after clicking ‘Mark as outstanding’?”
- “What information is missing?”
- “Step out of character and debrief the test. Separate evidence from assumptions.”

This is a simulation for exploring research hypotheses, not evidence from real participants. Role-playing does not itself authorize changes to live accounting records.

## Contents

- [`SKILL.md`](bank-reconciliation-ux/SKILL.md): workflow and design guidance
- [`references/exception-cases.md`](bank-reconciliation-ux/references/exception-cases.md): realistic reconciliation cases
- [`agents/openai.yaml`](bank-reconciliation-ux/agents/openai.yaml): display metadata
- [`Maya SKILL.md`](maya-bank-reconciliation/SKILL.md): accountant persona, interview behavior, think-aloud testing, and optional debrief
- [`Maya agents/openai.yaml`](maya-bank-reconciliation/agents/openai.yaml): display metadata

The skill is general guidance. It contains no prototype source code, customer data, or deployment configuration.

## License

MIT. See [LICENSE](LICENSE).
