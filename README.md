# RayX — Building What Comes Next

A responsive React + Vite marketing website with cinematic scrollytelling, GSAP ScrollTrigger reveals, Lenis smooth scrolling, RayX product cards, and a technology stack section.

## Run locally

1. Install Node.js (LTS).
2. In this folder, run `npm install`.
3. Run `npm run dev`.
4. Open the local URL printed by Vite.
5. For a production build, run `npm run build`; preview it with `npm run preview`.

## Add project links

Open `src/data/siteData.js` and replace these values with your actual deployed URLs:

- `rayxAI` — RayX AI project
- `rayxExam` — RayX Exam project
- `rayxLabs` — RayX Labs project

Use a full URL beginning with `https://` (or `http://` for local testing). A card opens its project button only when a valid URL is configured.

## Main files

- `index.html` — page metadata and app mount point
- `src/main.jsx` — React entry point
- `src/App.jsx` — page sections, navigation, product cards and animations
- `src/style.css` — responsive styling and visual effects
- `src/data/siteData.js` — editable project URLs and technology stack content
- `vite.config.js` — Vite + React configuration
- `package.json` — scripts and dependencies

## Tech stack shown on the website

Frontend: HTML5, CSS3, JavaScript, TypeScript · UI frameworks: React.js, Next.js · Styling: Tailwind CSS · Backend: Node.js, Express.js · Database: PostgreSQL, SQL · Authentication: Sessions, OAuth, JWT · APIs: REST APIs · Tools: Git, GitHub, VS Code · Testing: Vitest, Playwright · Deployment: Vercel, Cloudflare, Docker · Security: OWASP basics, input validation, secure authentication.

Note: The website displays the requested technology stack as a capabilities overview; this marketing site itself is built with React/Vite and its own listed dependencies. Backend, database, and authentication services are not automatically provisioned by this frontend project. Update the placeholder contact email in `src/App.jsx` before launch.


## Motion update (October 2026)

- Integrated the supplied Three.js GhostCursor shader trail with ember tint and idle fade; it respects reduced-motion preferences.
- Added a 50ms-per-character hero typing reveal and 36ms letter-by-letter vertical clip reveals.
- Added scroll-progress-driven statement wipe, interpolated process timeline/readouts, traced network route, and a molten-form stage.
- Removed the scrolling marquee; added ruled bands, a rate table, and native-details FAQ.
- Integrated the supplied Three.js GhostCursor with a viewport-fixed overlay, ember tint, restrained bloom, and idle fade.


## Extending RayX safely

- Add a product object to the `products` array near the top of `src/App.jsx`. Set `name`, `type`, `desc`, `tags`, `icon`, and `href`. Use an empty or placeholder `href` until the product is deployed; the card will safely show “Project link coming soon” instead of trying to open a broken URL. The card count updates automatically.
- Add technologies by editing `technologyGroups` in `src/data/siteData.js`. The stack cards and layout update from that array automatically.
- Set `contactEmail` in `src/data/siteData.js` to a real email address before launch. `hello@rayx.example` is a placeholder and cannot receive mail.
- The header remains fixed while the site scrolls through its story sections; navigation jumps to each section rather than splitting this cinematic landing page into separate routes.
