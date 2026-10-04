# Seat Theory — Ljubljana edition

An independent illustrated guide to choosing where to sit on an LPP city bus. Plain HTML, CSS, JavaScript and original SVG diagrams. No build step, dependencies, tracking, API keys or live bus data.

## Included

- Representative single-section, articulated and compact/midi diagrams. These are explicitly schematic and do not claim exact seat counts, doors or orientation for a vehicle.
- Seven zone analyses: ordinary front, middle, exit-adjacent, rear, wheel-arch seats, plus the joint and priority/accessibility area. The joint appears only on the articulated map.
- Pros, cons, best uses, practical checks and sources for each zone.
- Six preference presets, five 0–4 priority sliders and journey-length adjustments.
- Accessibility overrides for avoiding steps, wheelchair use and stroller use. Bays and priority seating are excluded from scored ordinary seats.
- Transparent weighted preference index with all ratings, preset weights and the formula available on the page.
- Qualitative suitability matrix, window-versus-aisle graphic and conceptual door-proximity diagram.
- Sun-side compass using user-selected bus and solar bearings; no weather or location is inferred.
- Ten journey scenarios, courtesy guidance, source notes, mobile and print styles, keyboard controls and reduced-motion support.

## Evidence

Research was checked on 4 October 2026 using official LPP and City of Ljubljana materials, plus CDC and NHS guidance for motion sickness. Sources are linked on the page. Historical fleet examples explain the illustrated shapes; no current fleet totals or route-to-model assignments are asserted. Older LPP publications are dated or identified as brochures, and visitors are directed to current markings and instructions.

The guide is not affiliated with LPP. Zone ratings and recommendations are editorial heuristics, not measured crowding, noise, vibration, availability, health probabilities or crash-safety results. The scoring index describes preference match only. The actual driver, on-board markings, accessibility needs and conditions take precedence.

## Model

Score = 100 × sum(zone rating × user weight) / (4 × sum(user weights)). Each zone rating and slider is 0–4. Short trips add one weight to exit access; long trips add one to being away from doors. Zero total weight displays no ranking; ties use displayed zone order. Accessibility choices bypass the model. Layout selection changes the illustration, not purported measured vehicle performance.

## Run and publish

Run `python3 -m http.server 8000` from this folder and open `http://localhost:8000`. For GitHub Pages, choose **Settings → Pages → Deploy from a branch → main → /(root)**. All asset paths are relative. Set a custom domain in Pages and your DNS provider if desired.

## Verification

JavaScript syntax, HTML IDs, local assets, recommendation calculations, access overrides, map changes, preset controls and sun-side geometry were checked. Browser visual QA was not available in the authoring environment; inspect desktop/mobile output after publication.
