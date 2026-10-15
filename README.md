# Harmoniq — Modular Multi-Event Concept Prototype (October 2026)

A browser-based concept demonstration aligned with the 14 October 2026 Harmoniq feasibility document. This is **not** the operational MVP, a cloud platform or a pilot-ready multi-device service.

## Open

Open `index.html` on GitHub Pages or a local HTTP server. The public project site's expected address is:

https://alimiri1997.github.io/harmoniq-demo/

> The address requires GitHub Pages to be enabled in repository **Settings → Pages → Deploy from branch → main / (root)**.

## Included flows

- Organiser: create, edit, select, pause and close events, with per-event **type**, **visibility** and **enabled modules**.
- Four sample event types: Concert/Festival, Corporate Conference, University Event, Pub/Quiz Night.
- Every event gets a shareable URL and a **scannable QR invitation**.
- Public events appear in the attendee list. Private events are code/link only **within the same browser data store**.
- Event code access with optional attendee participation in event modules.
- Light experience: static colours plus Aurora Wave (16 seconds) and Focus Pulse (12 seconds).
- Live polls: question library, multiple-choice and Yes/No types, vote submissions and basic results.
- Trivia: a simple scored question and venue-display quiz screen.
- Announcements: non-emergency messages.
- Configurable demo sponsor: brand, message, offer, expiry and validation limit; claim code and simulated operator redemption.
- Basic local analytics, optional satisfaction rating, a post-event report and downloadable CSV.
- Concept-only views for venue guidance and AI Discover & Dine; no real AI food suggestions, allergen safety assurances, payments or POS connection.

## Sample events

| Code | Event | Type |
|---|---|---|
| `NIGHT26` | Midnight Festival | Concert |
| `BEATS26` | City Beats Live | Concert/Festival |
| `SUMMIT26` | Harmoniq Business Summit | Corporate |
| `CAMPUS26` | University Welcome Week | University |

To test a Pub Night, create an event with the Pub / Quiz Night template under Organiser → All events.

## Important technical limits

- All state is persisted to the **current browser profile's localStorage**. Same-origin tabs in one browser profile can communicate through storage events and BroadcastChannel. **Independent computers and phones do not share event creation, voting, lighting, redemptions or analytics.** Publishing to GitHub Pages provides a link, not a backend.
- Demo attendee count for Midnight Festival begins at an **illustrative 86**; it is not a measured connected-user figure. Real event metrics, timing, failure rates and capacity have not been validated.
- Public/private visibility in this demo is **not an authentication or security boundary**. Real event access requires backend controls and identity/session management.
- The QR invitation is scannable, but a newly-created local event will not exist on a separate device. The QR code for a reward represents a **demo claim only**.
- Code and creative content in this repository are public. Do not upload production credentials, private attendee data or proprietary documents.
- Lighting is optional and requires device compatibility and safety tests; no emergency evacuation, life-safety or flash control is provided.
- The original document proposes an initial 10–30-device controlled QA before a 30–100-person pilot. This software does not meet those operational acceptance criteria.

## Next engineering step for actual pilot

Deploy role-based organiser authentication, per-event database, secure invite URLs, realtime messaging or WebSockets, participation logging, claims validation and device synchronization. Run privacy/security review, device tests and load testing before describing it as pilot-ready.

## Third party

The embedded QR Code generator is based on Kazuhiko Arase's JavaScript QR implementation (MIT license). See `THIRD_PARTY_NOTICES.md`.