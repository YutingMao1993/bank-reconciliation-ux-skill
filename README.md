# Bank Reconciliation UX skill

A Codex skill for designing, building, and reviewing AI-assisted bank reconciliation workflows. It covers exception handling, explainable match suggestions, human confirmation, progress, and auditability.

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

## Contents

- [`SKILL.md`](bank-reconciliation-ux/SKILL.md): workflow and design guidance
- [`references/exception-cases.md`](bank-reconciliation-ux/references/exception-cases.md): realistic reconciliation cases
- [`agents/openai.yaml`](bank-reconciliation-ux/agents/openai.yaml): display metadata

The skill is general guidance. It contains no prototype source code, customer data, or deployment configuration.

## License

MIT. See [LICENSE](LICENSE).
