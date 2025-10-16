# Personal Portfolio — Single-File HTML (index.html)

Summary
- A complete, self-contained single-file HTML web application that serves as a personal portfolio.
- Includes sections for About Me, Projects (with embedded live demos), Skills (with animated proficiency bars), and a Contact form with local persistence.
- Modern design with smooth scrolling, responsive layout, interactive widgets, and accessible UI.

Key Features Implemented
- Self-contained HTML, CSS, and JavaScript in one file (index.html).
- Sticky header with smooth in-page navigation and a responsive menu toggle for small screens.
- About section with an avatar-style decorative element and concise bio.
- Projects section featuring three cards, each with an embedded live demo via iframe srcdoc:
  - Weather Widget: Celsius/Fahrenheit toggle with faux data.
  - Color Mixer: Real-time RGB color mixer with live preview.
  - Counter App: Interactive counter with increment/decrement/reset.
- Skills section with animated proficiency bars that fill when scrolled into view.
- Contact form with client-side validation, simulated submission, and localStorage persistence (no backend required).
- Back-to-top button that appears after scrolling.
- Accessible and semantic markup (aria-labels, roles, live regions).

Setup Instructions
1. Save the file as index.html.
2. Open index.html in any modern web browser (Chrome, Edge, Firefox, Safari).
3. Optionally host on a static site service (see Deployment).

Usage Instructions
- Use the navigation menu to jump between sections: About, Projects, Skills, Contact.
- In the Projects area, interact with each embedded live demo (Weather Widget, Color Mixer, Counter App).
- Scroll to trigger the animated skill bars.
- Fill out the Contact form to simulate sending a message; data will be stored locally in your browser.

Technical Details
- HTML Structure:
  - header: Sticky navigation with responsive menu toggle.
  - main:
    - Section About: Two-column layout with avatar and bio.
    - Section Projects: Card grid with embedded iframes (srcdoc) providing self-contained demos.
    - Section Skills: Grid of skill cards with animated progress bars.
    - Section Contact: Form with validation, inline feedback, and localStorage persistence.
  - footer: Copyright and license note.
  - back-to-top button: Floating control for quick access.
- CSS:
  - Modern design with a dark UI, glassy surfaces, rounded corners, gradient accents, and soft shadows.
  - Responsive grid and typography for readability on mobile devices.
  - Custom properties (CSS variables) for color theming and easy tweaks.
- JavaScript:
  - Navigation: Menu toggle for small screens and scroll spy highlighting of active section.
  - Animations: Progress bars fill via IntersectionObserver when visible.
  - Projects: Self-contained demos implemented using iframe srcdoc content (sandboxed for security).
  - Contact: Client-side validation, a simulated submit with a short delay, success/error messaging, and localStorage persistence.
  - Footer: Dynamic current year.

Deployment Information
- Hosting: Static hosting (GitHub Pages, Netlify, Vercel, etc.).
- GitHub Pages: Create a repository and push index.html; enable GitHub Pages from main branch (root) or /docs as appropriate.

License
- MIT License

Generated Date
- 2025-10-17

Notes
- This is a fully functional, self-contained portfolio suitable for deployment as a standalone page.
- The embedded live demos use srcdoc in iframes to avoid external dependencies while still providing interactive, “live” experiences.