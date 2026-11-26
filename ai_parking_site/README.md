# Parkwise — AI Car Parking System (SDF prototype)

A browser-based parking management prototype. Plate recognition and payment are simulated; no real camera, gateway, or database is connected.

## Run locally
1. Download/extract the project folder.
2. Open `index.html` in a modern browser. For best results, use VS Code Live Server.
3. Use Dashboard, Vehicle Entry, Manage Lot, and Test Lab from the top navigation.

## Features
- Simulated plate validation and confidence threshold
- Nearest suitable free-bay allocation (EV bays are A03, A06, A09, A12)
- Reservations, active ticket management, and exit/payment simulation
- Occupancy-based tariff multiplier: 1.0 below 40%, 1.25 from 40%, 1.5 from 75%
- Grace period of 10 minutes; fees round up to full hours
- Admin bay fault/restore controls
- 16 executable practical tests in the Test Lab

## Important limitations
This is an academic prototype. State is held in browser memory and resets on refresh. ANPR is simulated using plate-format validation and a confidence slider. Payment is simulated; do not enter real payment information. The app is not a production access-control system.

## Deploy
Upload the files to a GitHub repository and enable GitHub Pages from Settings → Pages, selecting the main branch and root folder. Alternatively, deploy the folder to a static hosting service.
