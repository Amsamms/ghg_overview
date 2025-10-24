# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a research documentation project focused on Greenhouse Gas (GHG) emissions and carbon footprinting. The repository contains research materials in multiple formats (markdown, PDF, Word, audio recordings) and an interactive web-based guide.

## Repository Structure

- **Source Documentation**: `Greenhouse Gas Emissions Explained_ A Guide.md` (95KB markdown file - primary source document)
- **Web Interface**: `index.html` - Single-page application (SPA) presenting the research content interactively
- **Audio Resources**: Audio recordings in English and Arabic (`.m4a` files) containing research presentations

## Web Application Architecture

The `index.html` file is a standalone single-page application with the following architecture:

### Technology Stack
- **UI Framework**: Tailwind CSS (via CDN)
- **Visualization**: Chart.js (via CDN)
- **Typography**: Google Fonts (Inter)
- **Structure**: Tabbed navigation SPA with fixed top nav

### Design Decisions
- **Color Palette**: Warm Neutrals (White, Gray-50, Gray-700, Emerald-600)
- **Navigation**: Tabbed interface chosen for non-linear exploration of complex topics (science, policy, economics, calculations, case studies)
- **No SVG graphics or Mermaid JS used** (important constraint)

### Visualization Types Used
1. **Line/Bar Charts**: Rising CO2/temperature trends (time-series data)
2. **Interactive Lists**: Global frameworks (IPCC, ISO) - click to show/hide
3. **Diagram (HTML/CSS/Flexbox)**: Scopes 1/2/3 hierarchy visualization
4. **Horizontal Bar Chart**: Sector emissions comparison (handles long labels)
5. **Donut Chart**: Refinery emissions proportions (part-to-whole)

## Working with This Project

### Viewing the Web Application
Open `index.html` directly in a browser - no build process or server required.

### Modifying Content
- Primary research content is in the markdown file
- Web application content and structure is in `index.html`
- All styling uses Tailwind CSS utility classes
- All charts use Chart.js configuration objects embedded in the HTML

### Key Constraints
- Maintain the tabbed SPA structure for content navigation
- Do not introduce SVG graphics or Mermaid JS
- Keep the self-contained nature (all dependencies via CDN)
- Preserve the warm neutral color palette for consistency
