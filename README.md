# nusome GFS

A one-page scrolling website for the GFS fresh fruit chain. A 3D map of the whole chain stays fixed behind the page; scrolling flies the camera from the big picture into each operation, one after the other. Built as a single `index.html` with three.js; open it in a browser.

## The map is laid out in the order of the chain
- **Farm row (north, west → east):** orchard → bin cold room → packhouse → pallet cold store with its loading dock → transport yard → empty container depot.
- **City (middle):** blocks between the streets, the GFS Marketing operations office, local traffic.
- **Port (east):** weighbridge → export clearance → port gate → reefer stack with power and monitoring → quay cranes and the vessel.
- **Sea:** the loaded vessel crossing.
- **Destination (far east):** quay crane discharge → import customs and phytosanitary inspection → release gate → client warehouse dock (arrival QC) and cold room → client office (proof of delivery) → empty return depot.

## Buildings with openings
Every building has solid back and side walls, and an open front and east wall (pillars with large openings), so the work inside is visible from the street. When the page zooms into a building its roof lifts off and fades away.

## The steps
**Origin:** Picking · Bins into the cold room · Washing, grading and packing · Stored at +4 °C
**GFS Marketing:** Planning, booking and documents (the operations office in the city)
**Transport:** Empty container prepared (wash, inspection, PTI passed, set point) · The truck is dispatched · Loading the back of the truck (fruit pallets, temperature recorder, seal) · Transport to the port
**Port of loading:** Verified Gross Mass (VGM) · South African export clearance (SARS, PPECB, phytosanitary certificate) · Gate-in, stack and reefer power with monitoring · Loaded on the vessel
**Sea:** Crossing the sea
**Destination operations:** Container discharged at destination port · Import customs and phytosanitary clearance · Container released and delivered to client · Unloading and quality inspection · Pallets placed into the client's cold room
**Completion:** Empty container returned to depot · Shipment completed and proof of delivery recorded

The steps, their texts and camera shots are the `STEPS` list at the top of the script in `index.html`. The side dots, the top menu, arrow keys and Page Up/Down jump between steps.

## Publishing
Every push to `main` publishes the site with GitHub Pages (`.github/workflows/pages.yml`). Turn Pages on once under Settings → Pages → Source: **GitHub Actions**.
