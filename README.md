# Bank Reconciliation UX skills

A Codex skill for designing, building, and reviewing AI-assisted bank reconciliation workflows. It covers exception handling, explainable match suggestions, human confirmation, progress, and auditability.

The repository also includes **Maya — Bank Reconciliation User Simulation**, an accountant-perspective review skill. Maya walks through a design during month-end close, evaluates her confidence, and then provides prioritized UX recommendations and scores across six dimensions.

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

> Use $maya-bank-reconciliation to review this design as Maya, then give prioritized UX recommendations.

Maya is a staff accountant at a 120-person software company, working through 14 unmatched transactions on the third business day of month-end close. The simulation uses visible evidence, separates understanding from trust, and prioritizes accounting accuracy without unnecessary confirmation steps.

## Contents

- [`SKILL.md`](bank-reconciliation-ux/SKILL.md): workflow and design guidance
- [`references/exception-cases.md`](bank-reconciliation-ux/references/exception-cases.md): realistic reconciliation cases
- [`agents/openai.yaml`](bank-reconciliation-ux/agents/openai.yaml): display metadata
- [`Maya SKILL.md`](maya-bank-reconciliation/SKILL.md): accountant persona, simulation, and critique format
- [`Maya agents/openai.yaml`](maya-bank-reconciliation/agents/openai.yaml): display metadata and invocation prompt

The skill is general guidance. It contains no prototype source code, customer data, or deployment configuration.

## License

MIT. See [LICENSE](LICENSE).
