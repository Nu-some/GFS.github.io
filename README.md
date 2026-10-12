# nusome GFS

A one-page scrolling website for the GFS fresh fruit chain. A 3D map of the whole chain stays fixed behind the page; scrolling flies the camera from the big picture into each operation, one after the other. Built as a single `index.html` with three.js; open it in a browser.

## The map is laid out in the order of the chain
- **Farm row (north, west → east):** orchard → bin cold room → packhouse → pallet cold store with its loading dock → transport yard → empty container depot.
- **City (middle):** blocks between the streets, GFS HQ on the avenue, local traffic.
- **Port (east):** weighbridge → port gate → reefer stack → quay cranes and the vessel.
- **Sea:** the loaded vessel crossing.
- **Destination (far east):** quay crane discharge → customs scanner and inspection shed → client warehouse cold room → empty return depot.

## Buildings with openings
Every building has solid back and side walls, and an open front and east wall (pillars with large openings), so the work inside is visible from the street. When the page zooms into a building its roof lifts off and fades away.

## The steps
1. Picking · 2. Bins into the cold room · 3. Washing, grading and packing · 4. Stored at +4 °C · 5. The empty container is prepared (wash + PTI) · 6. The truck is dispatched · 7. Loading the back of the truck · 8. Through the city · 9. The truck is weighed (VGM) · 10. Off-loaded into the stack · 11. Loaded on the vessel · 12. Crossing the sea · 13. The container is discharged · 14. Customs clearance · 15. Pallets into the cold room · 16. The empty container is picked up

The steps, their texts and camera shots are the `STEPS` list at the top of the script in `index.html`. The side dots, the top menu, arrow keys and Page Up/Down jump between steps.

## Publishing
Every push to `main` publishes the site with GitHub Pages (`.github/workflows/pages.yml`). Turn Pages on once under Settings → Pages → Source: **GitHub Actions**.
