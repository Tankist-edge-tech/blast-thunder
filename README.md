<p align="center">
  <img src="assets/logo.png" alt="Ouro Logo" width="1024" height="1024"/>
</p>

<p align="center">
<svg xmlns="http://www.w3.org/2000/svg" width="850" height="220" viewBox="0 0 850 220">
  <defs>
    <linearGradient id="edgyGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#000000" stop-opacity="0"/>
      <stop offset="15%" stop-color="#000000" stop-opacity="0"/>
      <stop offset="25%" stop-color="#FF00FF" stop-opacity="1"/>
      <stop offset="35%" stop-color="#FF0033" stop-opacity="1"/>
      <stop offset="45%" stop-color="#FFFFFF" stop-opacity="1"/>
      <stop offset="55%" stop-color="#00FFFF" stop-opacity="1"/>
      <stop offset="65%" stop-color="#FF00FF" stop-opacity="1"/>
      <stop offset="75%" stop-color="#000000" stop-opacity="0"/>
      <stop offset="100%" stop-color="#000000" stop-opacity="0"/>
      <animateTransform attributeName="gradientTransform" type="translate" values="-1 0; 1 0" dur="4s" repeatCount="indefinite"/>
      <animateTransform attributeName="gradientTransform" type="rotate" additive="sum" values="0 0.5 0.5; 90 0.5 0.5; 0 0.5 0.5" keyTimes="0; 0.5; 1" dur="12s" repeatCount="indefinite" calcMode="spline" keySplines="0.42 0 0.58 1; 0.42 0 0.58 1"/>
    </linearGradient>
    <linearGradient id="subtitleGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00FFFF" stop-opacity="0"/>
      <stop offset="40%" stop-color="#FFFFFF" stop-opacity="0"/>
      <stop offset="50%" stop-color="#FFFFFF" stop-opacity="1"/>
      <stop offset="60%" stop-color="#00FFFF" stop-opacity="0"/>
      <stop offset="100%" stop-color="#00FFFF" stop-opacity="0"/>
      <animateTransform attributeName="gradientTransform" type="translate" values="-1 0; 1 0" dur="9s" repeatCount="indefinite"/>
      <animateTransform attributeName="gradientTransform" type="rotate" additive="sum" values="0 0.5 0.5; 90 0.5 0.5; 0 0.5 0.5" keyTimes="0; 0.5; 1" dur="12s" repeatCount="indefinite" calcMode="spline" keySplines="0.42 0 0.58 1; 0.42 0 0.58 1"/>
    </linearGradient>
    <filter id="fluidGlitch" x="-15%" y="-15%" width="130%" height="130%">
      <feTurbulence type="fractalNoise" baseFrequency="0.02 0.03" numOctaves="3" seed="42" result="fluidNoise"/>
      <feDisplacementMap in="SourceGraphic" in2="fluidNoise" scale="14" xChannelSelector="R" yChannelSelector="G" result="fluidDisplaced"/>
      <feTurbulence type="fractalNoise" baseFrequency="0.1 0.2" numOctaves="1" seed="5" result="glitchNoise"/>
      <feDisplacementMap in="fluidDisplaced" in2="glitchNoise" scale="4" xChannelSelector="R" yChannelSelector="G"/>
    </filter>
  </defs>
  <g filter="url(#fluidGlitch)">
    <text x="50%" y="90" text-anchor="middle" font-family="Consolas, Monaco, 'Courier New', monospace" font-size="40" font-weight="700" letter-spacing="2" fill="none" stroke="url(#edgyGradient)" stroke-width="0.8">BLAST THUNDER
      <animateTransform attributeName="transform" type="translate" additive="sum" values="0 0; 4 1; 0 4; -4 1; 0 0" keyTimes="0; 0.25; 0.5; 0.75; 1" dur="6s" repeatCount="indefinite" calcMode="spline" keySplines="0.42 0 0.58 1; 0.42 0 0.58 1; 0.42 0 0.58 1; 0.42 0 0.58 1"/>
    </text>
  </g>
  <g filter="url(#fluidGlitch)">
    <text x="50%" y="140" text-anchor="middle" font-family="Consolas, Monaco, 'Courier New', monospace" font-size="14" font-weight="600" letter-spacing="6" fill="none" stroke="url(#subtitleGradient)" stroke-width="0.8">Autonomous Reality Engine
      <animateTransform attributeName="transform" type="translate" additive="sum" values="0 0; 2 -2; 0 2; -2 -1; 0 0" keyTimes="0; 0.25; 0.5; 0.75; 1" dur="7s" repeatCount="indefinite" calcMode="spline" keySplines="0.42 0 0.58 1; 0.42 0 0.58 1; 0.42 0 0.58 1; 0.42 0 0.58 1"/>
    </text>
  </g>
</svg>
</p>

> **⚖️ License Notice:** This is a **source-available** research project licensed under **PolyForm Noncommercial 1.0.0**, not a permissive open-source license. Personal, educational, and research use only. **Commercial use is strictly prohibited without a separate paid license.** See [`LICENSE`](./LICENSE) for full terms, or contact **@Tankist-edge-tech** for commercial licensing inquiries.

---

**BlastThunder** is a research project exploring a new approach to real-time physics in combined-arms combat simulation. It's not a traditional video game or a standard simulator — it's a proof-of-concept for what we call an **Autonomous Reality Engine**: a physics core that discovers how the world behaves, rather than being told.

The **Dagor Engine** is currently used as temporary visual scaffolding to render the demonstration scene while the core research happens underneath.

---

## The Idea

Most simulators rely on physics that a human designed in advance — hardcoded formulas, pre-baked animations, static damage tables. It looks convincing, but it's fundamentally scripted.

**BlastThunder explores the opposite approach:** instead of hand-writing the physics, an AI-driven core observes raw interaction data and learns the governing equations on its own — discovering, rather than simulating, how armor deforms, how craters form, how a shockwave propagates.

The goal is destruction and material behavior that emerges from real physical principles the system found for itself, at a computational cost light enough to run in real time.

---

## Long-Term Vision

The current prototype (Dagor Engine, standard game-dev tooling) is a means to an end. The long-term research goal is a fully independent, from-scratch **Reality Engine** — including its own tooling and language — that no longer depends on any third-party engine, physics library, or renderer.

---

## Project Status

Early-stage research / pre-alpha. Architecture and internal methods are still evolving and are intentionally not detailed publicly at this stage.

---

## High-Level Stack

*   **Visualization:** Dagor Engine (temporary)
*   **Research Domain:** Physics-informed machine learning, symbolic/equation discovery
*   **Languages:** C++, Python, Daslang

---

## ⚖️ License

Licensed under **PolyForm Noncommercial License 1.0.0**. Free for personal, educational, and research use. **Commercial use of this code or architecture is strictly prohibited** without a separate agreement. Full terms in [`LICENSE`](./LICENSE).

---

## 👥 Contributions

This is currently a closed-development project. **External contributions and pull requests are not accepted at this time.** The repository is shared for visibility only.

---
Developed and maintained by **@Tankist-edge-tech** 
