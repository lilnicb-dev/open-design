---
name: diagram-design
description: "Generate editorial SVG/HTML diagrams with Cathryn Lavery's original Diagram Design agent skill, preserving project brand style."
triggers:
  - "editorial diagram"
  - "architecture diagram"
  - "process diagram"
od:
  mode: utility
  category: diagrams
  upstream: "https://github.com/cathrynlavery/diagram-design"
---

# Diagram Design — upstream capability

Use for polished flowcharts, timelines, architecture, data flows and branded SVG/HTML diagrams.

This entry is a discoverable **catalog route**, not a copy of the full upstream engine. When the caller's agent environment does not already have `diagram-design` installed, obtain the complete skill from the official repository and install into the **existing project or agent environment**, not a new GitHub repository:

```bash
npx skills add cathrynlavery/diagram-design
```

First inspect the project's active brand guidelines. Then use the installed upstream skill to produce a self-contained HTML/SVG artifact. For anything rendered into a video, export a static/animated asset for the established video-tool timeline. Do not claim a diagram is verified without inspecting its labels, relationships and output file.

Upstream: https://github.com/cathrynlavery/diagram-design (MIT). This catalog entry does not install anything automatically or imply runtime availability.
