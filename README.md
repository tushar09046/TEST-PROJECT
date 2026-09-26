# ClickCraft — Performance Marketing & Growth Consultancy

A modern, responsive multi-page marketing website for **ClickCraft**, a performance marketing and growth consultancy helping brands scale with data-driven strategies, paid media, and conversion optimization.

---

## Live Pages

| Page | File | Description |
|------|------|-------------|
| **Home** | `index.html` | Hero section with animated blob, feature grid, stats bar, vision CTA, contact form |
| **About Us** | `about.html` | Brand story, highlight quote, stats bar, core values grid, team section, CTA banner |
| **Consultation** | `consultation.html` | Services overview, 4-step consultation agenda, booking form with dropdowns, FAQ grid |
| **Contact** | `contact.html` | Contact info cards, message form, HQ details, partnerships info |

---

## Design System

### Color Palette

| Variable | Hex | Name | Usage |
|----------|-----|------|-------|
| `--primary` | `#F85A3E` | Tomato | Buttons, links, CTAs, active states |
| `--primary-light` | `#FF7733` | Atomic Tangerine | Hover highlights, footer accent |
| `--primary-dark` | `#E63B2E` | Cinnabar | Button hover/pressed states |
| `--dark` | `#0d0d0d` | Near Black | Footer background |
| `--heading` | `#1a1a2e` | Dark Navy | All heading text |
| `--body` | `#555555` | Grey | Body paragraph text |
| `--light-bg` | `#E1E6E1` | Alabaster Grey | Alternate section backgrounds |
| `--border` | `#d4d9d4` | Light Grey | Card borders, dividers |

### Typography

| Font | Weight | Usage |
|------|--------|-------|
| **Inter** | 300-800 | Body text, navigation, buttons, UI elements |
| **Cardo** | 400, 700, Italic | Serif accents, highlight quotes, special headings |

Loaded via Google Fonts CDN.

---

## Tech Stack

- **HTML5** — Semantic markup with SEO meta tags
- **CSS3** — CSS custom properties (variables), Flexbox, Grid, media queries
- **Vanilla JavaScript** — Scroll-reveal animations, mobile nav, form validation
- **Google Fonts** — Inter + Cardo
- **FormSubmit.co** — Serverless form submission to email

No build tools, frameworks, or dependencies required. Open any `.html` file directly in a browser.

---

## Project Structure

```
C:\TEST PROJECT\
|-- index.html              # Home page
|-- about.html              # About Us page
|-- consultation.html       # Consultation / Services page
|-- contact.html            # Contact Us page
|-- README.md               # This file
|
|-- resource/
|   |-- Tushar automates.jpg            # Brand logo & favicon image
|   |-- Screenshot 2026-09-15 201749.png
|
|-- assests/                # Assets directory (reserved)
```

---

## Form Integration — FormSubmit.co

All forms submit to **hello@clickcraft.com** via FormSubmit.co (https://formsubmit.co/).

### Configuration

Each form includes these hidden fields:

| Field | Value | Purpose |
|-------|-------|---------|
| `_honey` | (empty, hidden) | Honeypot trap — bots fill this, humans don't |
| `_captcha` | `false` | Disables FormSubmit's default CAPTCHA page |
| `_subject` | `New Contact Form Submission - ClickCraft` | Email subject line |
| `_template` | `table` | Formats email as a clean HTML table |
| `_next` | (empty) | Redirect URL after submission (customizable) |

### Business Email Validation

Forms block free email providers and only accept business domain emails.

Blocked domains include: Gmail, Yahoo, Hotmail, Outlook, AOL, iCloud, ProtonMail, Zoho, Yandex, GMX, Rediffmail, and 20+ disposable/temporary email services.

Users attempting to submit with a blocked domain see an inline error:
"Please use your business email address. Free email providers (Gmail, Yahoo, etc.) are not accepted."

---

## Bot Protection

1. **Honeypot field** — Hidden `_honey` input that bots auto-fill, causing FormSubmit to reject the submission
2. **Business email filter** — Blocks throwaway/disposable email services commonly used by spam bots
3. **HTML5 validation** — Required fields with `type="email"` and `type="url"` enforce browser-level format checks

---

## Features

- **Fully Responsive** — Mobile-first with hamburger menu on all pages
- **Scroll-Reveal Animations** — Content fades in on scroll via IntersectionObserver
- **Animated Hero Blob** — CSS keyframe morph animation on the home page
- **Consistent Navbar & Footer** — Identical structure, logo, and links across all pages
- **Branded Favicon** — Custom favicon from `resource/Tushar automates.jpg`
- **SEO Optimized** — Proper title, meta description, semantic HTML, heading hierarchy
- **No Dependencies** — Pure HTML/CSS/JS, zero npm packages or build steps

---

## Getting Started

1. Clone or download this project folder
2. Open `index.html` in any modern browser (Chrome, Edge, Firefox, Safari)
3. Navigate between pages using the top navigation bar

No server, no build step, no installation required.

### Optional: Local Server

For a more production-like experience:

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000
```

Then visit http://localhost:8000 in your browser.

---

## Customization

### Change Brand Colors

Edit the `:root` CSS variables in the `<style>` block of each HTML file:

```css
:root {
  --primary: #F85A3E;       /* Main brand color */
  --primary-light: #FF7733; /* Lighter accent */
  --primary-dark: #E63B2E;  /* Darker accent */
  --light-bg: #E1E6E1;      /* Section backgrounds */
}
```

### Change Form Recipient

Update the `action` attribute on each `<form>` tag:

```html
<form action="https://formsubmit.co/your-email@domain.com" method="POST">
```

### Change Logo

Replace `resource/Tushar automates.jpg` with your new logo file and update references in all 4 HTML files.

---

## License

(c) 2026 ClickCraft. All rights reserved.
