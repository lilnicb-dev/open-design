---
name: laya-decisions
description: "Route low-stakes text into advisory choice labels using the optional local Laya classifier, with benchmark and human-review gates."
triggers:
  - "local text classification"
  - "batch triage"
  - "laya model"
od:
  mode: utility
  category: creative-direction
  upstream: "https://github.com/NandhaKishorM/laya"
---

# Laya — advisory text classification

Use Laya for optional, low-stakes triage such as grouping messages or comment themes. Official Python package:

```bash
python -m pip install laya
```

The `laya.Router()` call may download pretrained checkpoints on first use. Obtain permission for any model download, evaluate accuracy using labeled examples for this domain, and leave ambiguous or consequential cases to the stronger agent or human reviewer.

The sibling `nettys-lead-pipeline/tools/laya_triage.py` connector is an **explicit-file, advisory-only** example; never auto-reject prospects, skip established research/approval gates, send emails, or mutate lead ledgers from a classifier score.

Upstream: https://github.com/NandhaKishorM/laya (Apache-2.0). This entry is a catalog pointer, not a bundled model or installed runtime.
