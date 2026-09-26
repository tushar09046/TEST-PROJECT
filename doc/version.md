# Version History — ClickCraft Project

This document logs all major updates, releases, bug fixes, and feature additions for the **ClickCraft** project.

---

## [v1.1.0] — 2026-09-26

### Added
- **AI Agent Documentation**: Added `doc/ai_agent_instructions.md` outlining project guidelines, architecture, CSS design tokens, and git workflow.
- **Version History**: Added `doc/version.md` to track release history and changelogs.
- **Workspace Rules**: Added `.agents/rules/project_documentation.md` rule to enforce documentation standards for future AI sessions.
- **Git Ignore & Asset Tracking**: Added `.gitignore` configuration and `.gitkeep` for tracking the `assests/` directory on remote.

---

## [v1.0.0] — 2026-09-26

### Added
- **ClickCraft Web Application**: Initial launch of the ClickCraft performance marketing and growth consultancy website.
- **Pages**:
  - `index.html`: High-converting landing page with hero banner, service overview, case studies, and lead capture.
  - `about.html`: Team overview, mission statement, and core philosophy.
  - `consultation.html`: Detailed service breakdown and booking form.
  - `contact.html`: Contact form integrated with FormSubmit.co.
- **Design System**:
  - Custom CSS tokens (`--primary: #F85A3E`, `--dark: #0d0d0d`, `--heading: #1a1a2e`).
  - Google Fonts integration (`Inter` and `Cardo`).
  - Responsive glassmorphic navigation bar with mobile toggle overlay.
- **Form Security & Validation**:
  - FormSubmit.co integration for automated email routing.
  - Front-end email validation enforcing business emails and bot protection.
