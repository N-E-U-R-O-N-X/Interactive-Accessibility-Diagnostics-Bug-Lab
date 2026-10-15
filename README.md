# ⚡ AccessForge: Interactive WCAG 2.1 Inspection Workbench

> **A tactile, single-file Human-Computer Interaction (HCI) laboratory designed to teach and stress-test WCAG 2.1 Level AA accessibility standards through dynamic 3D physics, synthesized audio, direct manipulation, and a gamified bug hunt.**

<p align="center">
  <img src="https://img.shields.io/badge/WCAG-2.1%20Level%20AA-4ECDC4?style=for-the-badge&logo=w3c&logoColor=white" alt="WCAG 2.1 AA" />
  <img src="https://img.shields.io/badge/Architecture-Single%20File%20(No%20Bundler)-FF6B6B?style=for-the-badge" alt="Single File App" />
  <img src="https://img.shields.io/badge/Dependencies-0%20(Pure%20Vanilla)-F5C064?style=for-the-badge" alt="Zero Dependencies" />
  <img src="https://img.shields.io/badge/Audio-Web%20Audio%20API%20Engine-1B2A4A?style=for-the-badge" alt="Web Audio API" />
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" alt="MIT License" />
</p>

---

## 📑 Table of Contents

- [Project Motivation](#-project-motivation)
- [System Architecture & Core Modules](#-system-architecture--core-modules)
  - [Drawer 01: The Keys (Spatial Keyboard & Audio Telemetry)](#drawer-01-the-keys-spatial-keyboard--audio-telemetry)
  - [Drawer 02: The Mixer (Relative Luminance & Contrast Lab)](#drawer-02-the-mixer-relative-luminance--contrast-lab)
  - [Drawer 03: The Lens Room (Vision & Reflow Diagnostics)](#drawer-03-the-lens-room-vision--reflow-diagnostics)
  - [Drawer 04: The Buggy Shop (Gamified 14-Defect Audit)](#drawer-04-the-buggy-shop-gamified-14-defect-audit)
  - [The Thermal Audit Receipt](#the-thermal-audit-receipt)
- [Comprehensive WCAG 2.1 Bug Matrix](#-comprehensive-wcag-21-bug-matrix)
- [Mathematical & Algorithmic Foundations](#-mathematical--algorithmic-foundations)
- [Interaction & Keyboard Navigation Guide](#-interaction--keyboard-navigation-guide)
- [Technical Stack & Design Patterns](#-technical-stack--design-patterns)
- [Local Setup & Getting Started](#-local-setup--getting-started)
- [License](#-license)

---

## 💡 Project Motivation

Digital accessibility guidelines (WCAG) are typically consumed as dense, regulatory checklists. Developers and designers often struggle to translate these abstract normative criteria into tangible design empathy.

**AccessForge** solves this through sensory HCI principles:
* **Direct Manipulation:** Users do not merely read about contrast failures; they manipulate RGB sliders and observe dynamic pass/fail coin flips.
* **Immediate Sensory Feedback:** Every keystroke produces visual depth displacement, live speed telemetry, and synthesizes pentatonic frequencies.
* **Active Contrastive Analysis:** Users alternate directly between intentional accessibility anti-patterns and their semantic, fully accessible remediations.

---

## 🗄️ System Architecture & Core Modules

The application is split into four distinct interactive drawers accessible via an accessible tablist:

```text
┌─────────────────────────────────────────────────────────────────────────────┐
│                            ACCESSFORGE INTERFACE                            │
├─────────────────┬─────────────────┬──────────────────┬──────────────────────┤
│ 01 · THE KEYS   │ 02 · THE MIXER  │ 03 · THE LENS    │ 04 · THE BUGGY SHOP  │
│ 3D Spatial Deck │ Contrast Lab    │ Magnifier Loupe  │ 14-Bug Hunt          │
│ Web Audio Synth │ Mascot 'Dot'    │ Reflow & CVD     │ Side-by-Side Fixes   │
│ Live KPM Feed   │ CVD Color Proof │ Text Stressors   │ Thermal Receipt      │
└─────────────────┴─────────────────┴──────────────────┴──────────────────────┘
