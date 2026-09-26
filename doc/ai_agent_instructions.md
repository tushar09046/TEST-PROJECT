# AI Agent Instructions — ClickCraft Project

This document provides complete instructions, technical details, design systems, and guidelines for AI agents working on the **ClickCraft** repository.

---

## 1. Project Overview
**ClickCraft** is a performance marketing and growth consultancy web application. It features a modern, responsive design built with HTML5, custom CSS (vanilla design system with CSS variables), and JavaScript.

- **Primary Goal**: Help brands scale with data-driven strategies, paid media, and conversion rate optimization.
- **Repository Location**: `c:\TEST PROJECT`
- **Remote GitHub Repository**: `https://github.com/tushar09046/TEST-PROJECT.git`

---

## 2. Technology Stack & Architecture
- **HTML5**: Semantic markup across key pages (`index.html`, `about.html`, `services/consultation.html`, `contact.html`).
- **CSS3 Design System**:
  - CSS Variables defined in `:root` (Warm color palette: `#F85A3E` primary, `#0d0d0d` dark, `#1a1a2e` headings, `#E1E6E1` light bg).
  - Typography: Google Fonts (`Inter` for UI, `Cardo` for serif accent typography).
  - Custom glassmorphism, responsive grid layouts, and micro-interactions.
- **Form Integration**: FormSubmit.co integration with business email validation and anti-spam protection.
- **Assets**: Stored in `resource/` and `assests/` directories.

---

## 3. Directory Structure
```
c:\TEST PROJECT/
├── .agents/
│   └── rules/
│       └── project_documentation.md   # Workspace rules for documentation standards
├── doc/
│   ├── ai_agent_instructions.md       # AI agent guidance & system instructions (this file)
│   └── version.md                     # Complete project version history
├── resource/                          # Images, logos, and screenshots
├── assests/                           # Media assets and resources
├── .gitignore                         # Configured Git exclusion patterns
├── index.html                         # Home page
├── about.html                         # About Us page
├── consultation.html                  # Consultation / Service details page
├── contact.html                       # Contact & Lead submission page
└── README.md                          # Main project readme
```

---

## 4. AI Agent Guidelines & Rules

### A. Design Aesthetics & Consistency
1. **Preserve Color Palette**: Always adhere to the established warm CSS design system (`var(--primary)`, `var(--primary-dark)`, `var(--heading)`, etc.).
2. **Typography Rules**: Use `font-family: 'Inter'` for general body/buttons and `.serif` (`font-family: 'Cardo'`) for headings or pull-quotes.
3. **Responsive Layouts**: Maintain mobile-first responsive styling with standard breakpoints (`768px`, `1024px`).

### B. Form Handling & Security
1. **Validation**: Ensure all form inputs (email, phone, text) have active front-end validation and sanitization.
2. **Business Email Enforcement**: Ensure contact forms validate against generic/free email providers where required.
3. **FormSubmit.co Config**: Maintain proper hidden fields (`_captcha`, `_template`, `_next`) for lead routing.

### C. Git & Version Control Workflow
1. **Never commit sensitive credentials** (such as GitHub PATs or API secrets) into code or configuration files.
2. **Version Documentation**: Update `doc/version.md` whenever introducing new features, bug fixes, or major design changes.
3. **Branching & Commits**: Write concise, descriptive commit messages describing the changes made.

---

## 5. Maintenance & Execution Commands
- **Git Status**: `git status`
- **Git Push**: `git push origin main`
- **Git Fetch**: `git fetch origin`
