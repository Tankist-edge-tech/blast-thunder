<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a0000,50:ff4500,100:1a0000&height=220&section=header&text=BlastThunder&fontSize=75&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Autonomous%20Reality%20Engine&descAlignY=58&descSize=22&descColor=ffb347" alt="BlastThunder"/>
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
