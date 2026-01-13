# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a GitHub Pages repository (shak2000.github.io) for hosting a personal website. The repository follows GitHub Pages conventions where content is served directly from the main branch.

## GitHub Pages Specifics

- The site is hosted at: https://shak2000.github.io
- Files pushed to the main branch are automatically deployed
- The entry point should be `index.html` at the root directory
- GitHub Pages supports Jekyll by default (can be disabled with `.nojekyll` file)
- Custom domains can be configured via CNAME file

## Development Workflow

Since this is a GitHub Pages site, changes are deployed by pushing to the main branch. Test locally before pushing:

For static HTML/CSS/JS:
- Use any local web server (e.g., `python3 -m http.server 8000` or `npx serve`)
- Open http://localhost:8000 in a browser

For Jekyll sites (if using):
- Install: `gem install bundler jekyll`
- Run locally: `bundle exec jekyll serve`
- View at: http://localhost:4000

## Repository Structure

This is a static HTML/CSS portfolio site:
- `index.html` - Main portfolio page with profile info, experience, skills, and projects
- `tableau.html` - Separate page showcasing Tableau data visualization projects
- `styles.css` - Light theme styling with responsive design
- Profile avatar is loaded directly from GitHub: `https://github.com/shak2000.png`

## Content Updates

When updating the portfolio content:
- Personal info, bio, and links are in the profile header section of `index.html`
- Professional experience is in the `.experience` section
- Technical skills are organized by category in the `.skills` section
- Projects section includes links to GitHub repos and the Tableau projects page
- Tableau visualizations are embedded in `tableau.html` using iframes
- The site uses Font Awesome icons (CDN) for visual elements

## Styling

The site uses CSS custom properties (variables) defined in `:root` for consistent theming:
- Dark mode GitHub color scheme (--bg-primary, --bg-secondary, etc.)
- Fully responsive design with breakpoints at 1024px, 768px, and 480px
- Hover effects on links, badges, and repository cards
