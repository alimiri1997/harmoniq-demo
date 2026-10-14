# Harmoniq — Interactive Multi-Event Product Demo

English-language, static HTML prototype of the Harmoniq event-engagement concept.

## Included demo flows
- Organiser: create, edit, select and change event status
- Attendee: join an event by its code and switch events
- Independent event lighting, live polls, trivia, announcements, sponsorship and rewards
- Venue display with event selection
- Demonstration analytics

### Sample event codes
- `NIGHT26` — Midnight Festival
- `BEATS26` — City Beats Live

## Publish with GitHub Pages
1. Create a GitHub repository, e.g. `harmoniq-demo`.
2. Upload the *contents* of this folder into the **root of the `main` branch**.
   `index.html` must be directly in the repository root, not inside another folder.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, set **Source: Deploy from a branch**.
5. Choose **Branch: main** and **Folder: /(root)**, then save.
6. Once GitHub finishes publishing, open the site URL in **Settings → Pages**.
   A typical project-site URL is `https://YOUR-USERNAME.github.io/harmoniq-demo/`.

No installation, build or server-side runtime is required.

## Important limitations
- This is a *product demo*, NOT a shared multi-user pilot.
- It stores events, polls and settings in each browser's `localStorage`.
- `BroadcastChannel` and storage events can synchronize same-origin tabs in the
  same browser profile, but **not phones or computers on different devices**.
- Publishing on GitHub Pages makes the page reachable from different devices,
  but it does **not** create a common database or realtime service.
- The displayed figures, sponsor and offer are demonstrative, not actual live metrics.
- There is no organiser login or production-grade authentication.
- GitHub Pages is publicly reachable. Do not put real user data or confidential material here.

To support a real 30–100 participant pilot, add authentication/roles,
server-side event storage and a realtime backend (e.g. WebSocket + database),
plus testing and operational safeguards.

## Ownership
Prepared for evaluation of Harmoniq. No public software license is granted by
this repository package. Confirm the owner's authorization before publishing.