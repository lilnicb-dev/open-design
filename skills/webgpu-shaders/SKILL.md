---
name: webgpu-shaders
description: "Design optional WebGPU backgrounds and interactive shader effects using the official shaders library; include fallbacks and performance checks."
triggers:
  - "webgpu shader"
  - "premium animated website background"
  - "shaders.com effects"
od:
  mode: prototype
  category: 3d-shaders
  upstream: "https://github.com/shader-effects-inc/shaders"
---

# Shaders — official WebGPU component library

Use for tasteful animated gradients, glass, cursor effects and interactive web backgrounds when visuals materially improve a page. This is an opt-in catalog route, not an automatic change to any production site.

In the **existing website or web application project**, inspect its framework and lockfile before using the official package:

```bash
npm install shaders
```

For React, the documented entry is `shaders/react` with `Shader` and component children. Preserve a non-WebGPU fallback, reduced-motion behavior, mobile performance and readable text contrast. Run build and page-level tests before merging; do not modify live website visuals or add remote scripts merely because this skill exists.

Upstream: https://github.com/shader-effects-inc/shaders (MIT). Actual installation and WebGPU behavior require a compatible runtime.
