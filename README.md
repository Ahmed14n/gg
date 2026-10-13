# Rentora — Front-end prototype

Rentora is a responsive, English-language front-end concept for a peer-to-peer product rental marketplace. The project uses plain HTML, CSS, and JavaScript and does not require a build step.

## Run locally
1. Keep `index.html`, `styles.css`, `app.js`, and the `assets/` folder together.
2. Confirm the introduction video exists at `assets/rentora-intro.mp4`.
3. Open `index.html` in a modern browser. For the most reliable media and local-storage behavior, serve the folder through a local static server (for example, VS Code Live Server).
4. The introduction must finish before the account screen appears. If autoplay is blocked, choose **Play introduction** and watch it through. If the video cannot load, the site displays an error and does not bypass the introduction.

## Main demo flows
- Mandatory intro video → demo sign up/sign in → marketplace.
- Search, city filter, categories, max daily price, delivery and verified-owner filters, sorting, favorites, and compare up to three sample items.
- Product detail modal with rental rules, handover options, date validation, day-count price estimate, illustrative deposit, and demo payment choice.
- Booking requests saved locally with **Waiting for owner** status.
- Account dashboard for bookings, favorites, private product drafts, condition reports, issue/dispute reports, and sample review information.
- Admin preview with sample overview, listings, reports/disputes, and illustrative analytics.
- Newsletter form acknowledges submission without sending or storing the email.

## Prototype limitations — please read
This is a **front-end-only prototype**. There is no backend, database, cross-device synchronization, real authentication, identity verification, secure admin role, real owner approval, confirmed availability, actual booking confirmation, payment processing, live chat, live notifications, uploaded evidence storage, dispute mediation, or automatic publication of user listings.

- Sign-up/sign-in is a demo flow only. The password is used for browser form validation and is **never saved**.
- Favorites, bookings, private drafts, and report metadata use browser `localStorage` where available. If browser storage is unavailable, interactions continue for the current page session but data will not persist after reload.
- Evidence file inputs only allow local selection; files are not uploaded or stored by this prototype.
- Ratings, reviews, verification labels, product availability, and admin analytics are sample demonstration data.
- Product drafts remain private and do not enter public search results.
- “Online payment” and “Cash on pickup / delivery” are demo display choices only. No money is charged or transferred. A booking request is not a confirmed reservation.

## Integrations required for a production service
A production build needs a backend API and database; secure authentication and authorization; identity and owner verification workflows; listing moderation; real availability and booking state management; payment provider integration and refund/deposit policy; secure image and evidence uploads; notifications and messaging; and a real reporting/dispute process. Privacy, consumer protection, rental terms, tax, and local legal requirements should be reviewed before launch.

## Name availability
**Rentora is a provisional project name.** Trademark/legal, domain-name, and social-handle availability have not been verified. Perform appropriate legal and digital availability checks before public launch.

## Files
- `index.html` — semantic page structure and mandatory intro/auth/store screens
- `styles.css` — responsive visual system and layouts
- `app.js` — demo data, interactions, local persistence, and modals
- `assets/rentora-intro.mp4` — supplied intro video
