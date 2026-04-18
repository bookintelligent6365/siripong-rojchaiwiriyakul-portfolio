# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A static, single-page personal portfolio for **Siripong Rojchaiwiriyakul** — Senior Sales Analyst and founder of **Book Intelligent Academy**. No build tools, frameworks, or dependencies. Open `index.html` directly in a browser to preview.

## Architecture

Two files make up the entire site:

- [index.html](index.html) — All HTML structure and the inline theme-toggle script (dark/light mode via `localStorage` and `data-theme` attribute on `<html>`)
- [style.css](style.css) — All styling, using CSS custom properties defined in `:root` and overridden in `[data-theme="light"]`

Reference spec and content data live in:
- [plan/our_plan.md](plan/our_plan.md) — Canonical source of truth for content (stats, dates, project outcomes, contact links)
- [GEMINI.md](GEMINI.md) — Design conventions and aesthetic rationale

## Design System

All colors must use CSS variables — never hardcode hex values in new rules.

| Variable | Role |
|---|---|
| `--gold` / `--gold-dim` / `--gold-glow` | Primary accent — use sparingly for high-impact elements only |
| `--bg-color`, `--surface`, `--surface-accent` | Background layers (deep to shallow) |
| `--text-primary`, `--text-secondary` | Typography hierarchy |
| `--border`, `--border-gold` | Subtle vs. gold-accented borders |

**Typography:** `Inter` for UI text, `JetBrains Mono` for dates, tags, section labels, and technical context.

**Spacing convention:** Sections use `8rem` vertical padding (`premium-section`). Cards use `3rem` internal padding. Maintain generous negative space — this is the "Executive" feel.

## Theme Toggle

The dark/light toggle is handled entirely in the `<script>` block at the bottom of `index.html`. It sets `data-theme="light"` on `<html>` and persists via `localStorage`. All new CSS rules must support both themes by using variables, not hardcoded colors.

## Deployment

Target: **GitHub Pages**. No build step — push the repo and the site is live from `index.html`.
