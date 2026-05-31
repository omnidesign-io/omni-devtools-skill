# Omni DevTools Skill

Version: 1.0.0

`omni-devtools` is an AI agent skill for building dev-only, floating design and typography exploration panels on development branches. It enables creators to experiment with style tokens (typography, weights, scaling, glassmorphic card variables) live in the browser, instantly seeing visual impacts across the product surface without writing or compiling code edits.

## When To Use This Skill

Use this skill when:
- Exploring new typographic systems (such as changing Google Fonts, scaling base sizes, or adjusting weights globally).
- Toggling decorative features (like italics, underlines, borders, or glassmorphic settings).
- Tuning visual balances live with stakeholders without waiting for fresh builds.
- Preserving exploration state across refreshes using localized parameters.

Do NOT use this skill for:
- Production branches (these exploration tools are strictly development-only panels and must not compile to client-side production bundles).
- Backend or logical database experimentation.

## Core Pattern Architecture

A complete Omni DevTool follows a three-layered design system:
1. **CSS Variables & Calc Rules**: Defines relative styles mapping typography/scales to computed variables.
2. **Non-Blocking Preloader Script**: Inline script in the page's `<head>` that parses parameters from `localStorage` and applies styling before rendering to avoid CLS/FOUT.
3. **Floating Explorer Panel UI**: Glassmorphic UI container with range sliders, presets, and design history stack.

## Installation

Install this repository as an agent skill by copying or linking `SKILL.md` to the provider-agnostic global directory `~/.agents/skills/omni-devtools/SKILL.md`, or copy `SKILL.md` into a local `omni-devtools` skill directory.

## Release

- Initial public release: 1.0.0
