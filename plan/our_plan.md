# Implementation Plan: Siripong Guu - Senior Sales Analyst Portfolio

## Objective
Build a modern, dark-themed, responsive portfolio website for "Siripong Guu" (Senior Sales Analyst) to be hosted on GitHub Pages. The design will utilize the "JetBrains Mono" font to give it a clean, technical, and data-focused aesthetic.

## Key Files & Context
- `index.html`: The main structural file containing the hero section, projects, and contact details.
- `style.css`: The styling file containing the dark theme variables, JetBrains Mono font import, and responsive grid layouts.
- `assets/` (Optional directory for project images or icons, if needed later).

## Implementation Steps

### 1. Project Setup
- Create the necessary files: `index.html` and `style.css` in the local workspace.

### 2. Styling (style.css)
- Import the **JetBrains Mono** font from Google Fonts.
- Define a modern dark theme using CSS variables:
  - Background: `#0d1117` (GitHub Dark Dimmed background)
  - Surface/Cards: `#161b22`
  - Text Primary: `#c9d1d9`
  - Accent Color: A subtle blue or green for links/buttons (e.g., `#58a6ff`).
- Set up a CSS reset and basic typography styling to ensure JetBrains Mono is the default font.
- Create utility classes for layout (flexbox/grid) and spacing.

### 3. HTML Structure (index.html)
- **Hero Section:**
  - Create a centered hero banner displaying the name "Siripong Guu".
  - Add the subtitle: "Senior Sales Analyst".
- **Projects Section:**
  - Build a responsive 3-column CSS grid.
  - Create 3 placeholder project cards. Each card will contain:
    - Project Title (e.g., "Sales Forecasting Model", "Market Basket Analysis", "Interactive Sales Dashboard").
    - A brief description of the tools used and the outcome.
    - A placeholder link to a repository or live dashboard.
- **Contact Section:**
  - Create a footer or dedicated section with contact details.
  - Include links for Email, LinkedIn, and GitHub.

### 4. Deployment to GitHub Pages
- Initialize a local git repository.
- Commit the `index.html` and `style.css` files.
- Push the code to a new public GitHub repository (ideally named `siripong-guu.github.io`).
- Enable GitHub Pages in the repository settings, pointing to the `main` branch.

## Verification & Testing
- Preview `index.html` locally in a web browser.
- Verify that the dark theme colors and JetBrains Mono font render correctly.
- Test the responsiveness: ensure the 3-column project grid collapses gracefully to a single column on mobile devices.
- Verify that all contact links are functional and properly formatted.