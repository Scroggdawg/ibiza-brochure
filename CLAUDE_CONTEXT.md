# CLAUDE_CONTEXT.md

## Project
Static single-file Ibiza trip brochure for Luke Scroggins / BMF Studios.

## Repository
- Local path: `/Users/scrogdawg/ibiza-brochure-site`
- GitHub repo: `https://github.com/Scroggdawg/ibiza-brochure`
- Production URL: `https://scroggdawg.github.io/ibiza-brochure/`

## App Shape
- The site is a static GitHub Pages brochure.
- Primary source is `index.html`.
- The downloaded local copy is `/Users/scrogdawg/Downloads/ibiza-brochure.html`.
- Venue images are embedded as base64 JPEG data URLs so the brochure remains single-file and resilient.
- The map section uses Leaflet with OpenStreetMap tile URLs. It is not a hand-drawn custom map.

## Current Feature State
- Brochure sections: hero, calendar, trip overview, hotels, restaurants, clubs, day clubs, itinerary, tips, maps, footer.
- Map section sits near the end, after Insider Notes and before the footer.
- Maps included:
  - Full Ibiza island map with all trip anchors.
  - Ibiza Town / Marina / Playa d'en Bossa detail map.
  - Beach picks map.
- Map pins include hotels, airport, nightclubs, day clubs, dinner anchors, and beaches.

## Deployment
- GitHub Pages serves the `main` branch.
- Vercel was previously attempted but blocked by an invalid saved token, so GitHub Pages is the working production host.

## Verification Baseline
- Local preview can be run with:
  `python3 -m http.server 8765 --directory /Users/scrogdawg/ibiza-brochure-site`
- Browser verification should check that:
  - All three map frames render OpenStreetMap tiles.
  - Pins are visible.
  - The map section matches the paper / sea / sun brochure palette.
  - The live GitHub Pages URL updates after push.

## Doctrine Status
This is the first documented session using the doctrine in this repo. Keep this file updated at the end of future sessions.

## Luke's Next Action
Open the live GitHub Pages URL and scroll to the new Island Map section.
