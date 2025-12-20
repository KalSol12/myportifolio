# Portfolio Website - AI Coding Guidelines

## Project Overview
This is a static multi-page portfolio website for Kaleab Tenkir, built with vanilla HTML, CSS, and minimal JavaScript. The site consists of 5 pages: Home (index.html), About (aboutme.html), Projects (project.html), Skills (skill.html), and Contact (contact.html).

## Architecture & Structure
- **Multi-page static site**: Each section is a separate HTML file with shared header/footer
- **Modular CSS**: `style.css` for global styles, page-specific CSS files (e.g., `about.css`) for unique sections
- **Assets organization**: Images in `images/`, documents in `assets/`

## Key Patterns & Conventions

### HTML Structure
- Use consistent header with logo and navigation across all pages
- Main content wrapped in `<section>` with descriptive IDs (e.g., `id="about"`)
- Footer with copyright on all pages for consistency
- Container class for responsive layout: `<div class="container">` (90% width, max 1200px)

### Styling Approach
- **Fonts**: 
  - Body: 'Roboto' (weights 400,500,700)
  - Headings: 'Montserrat' (weights 500,700)
- **Color Palette**:
  - Primary: #00bcd4 (cyan for accents)
  - Secondary: #ffe600 (yellow for highlights)
  - Text: #333 (dark), #d6d2d2 (light on dark backgrounds)
  - Backgrounds: White/light gradients, dark radial gradients for sections
- **Responsive**: Use flexbox for layouts, media queries for mobile
- **Effects**: Box shadows, transitions (0.3s), sticky header

### JavaScript Usage
- Minimal inline scripts only (e.g., typing effect in index.html, form validation in contact.html)
- No external JS libraries - keep vanilla JS for simple interactions

### File Naming & Organization
- HTML: lowercase, descriptive (aboutme.html, not about.html)
- CSS: matches HTML name (about.css for aboutme.html)
- Images: descriptive names, stored in `images/`
- Assets: PDFs/docs in `assets/`

### Navigation & Links
- Internal links: relative paths (e.g., `href="aboutme.html"`)
- External: target="_blank" for social/GitHub links
- Download links: `download` attribute for CV

### Content Guidelines
- Profile image: `images/photo_2025-10-15_23-58-56.jpg` (circular, 200x200px)
- Social links: GitHub, LinkedIn, Twitter with Font Awesome icons
- CV download: `assets/kaleab_Temkir_fita.pdf`
- Project descriptions: Detailed, highlighting technologies, challenges, outcomes
- Skills: Categorized (Frontend, Backend), with visual progress indicators
- About: Include education, achievements, certifications

### Professional Elements
- Consistent footer across all pages
- Form validation on contact page
- Alt texts for accessibility
- Semantic HTML with proper headings and sections

## Development Workflow
- No build tools required - edit HTML/CSS directly
- Test in browser: Open index.html locally
- Responsive testing: Resize window or use dev tools
- Font Awesome icons: Use classes like `fab fa-github`

## Common Patterns
- Hero sections with text left, image right layout
- Skills displayed as cards with icons or progress bars
- Projects grid with detailed descriptions and links
- Contact form with client-side validation
- Dark theme sections with light text for contrast

When adding new sections, create matching HTML and CSS files, update navigation in all pages, include footer.