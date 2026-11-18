# Navarro House renovation

Plans, costs and progress for our house renovation. Prices are in Philippine pesos (₱).
Last updated: 18 November 2026.

> **For family:** open the website **https://tatayotter.github.io/navarro-house/** and tap any link.
> The 3D model and plans open right in your phone or computer browser.

## What's happening now
| Part | Status |
|---|---|
| Steel stair (Phase 3) | Final design done (v3.3). Steel bought. Welder hired, starting soon. |
| Front gate | Design settled (roll-up car shutter + small door). Waiting on final measurements. |
| Master bedroom | Plan and costing done (about ₱167k with buffer). |
| Living room | Design and cost estimate done (₱228k–370k). |
| Electrical wiring | Whole-house plan drafted: 20 ceiling lights + 5 pendants, 32 outlets, 12 smart switch plates. Booster pump and roof room window aircon have their own circuits. Materials about ₱113k–179k (online estimate). Waiting for the electrician to check. |
| 3D model | Whole house in 3D with airflow, electrical layer and phone view. Kitchen re-arranged (bar counter, fridge by the T&B). |
| Rooftop | Roof room enlarged to take in the old deck area: no deck, no hallway; door at the top of the steel stair. Walls decided: container-van style steel outside, insulation, Hardiflex inside; tiled floor, gypsum ceiling, about ₱205k–345k with buffer (online estimate), see `rooms/rooftop-room.md`. Engineer to check slab load and wall anchoring. |

## Where the prices come from
- **Local receipts and quotes:** steel stair materials already bought (₱18,589, store receipt), welder labour (₱7,000), architect's stair quote (₱64,850, for comparison).
- **Online estimates (no local quote yet):** stair items still to buy (≈₱7,695), front gate, master bedroom, living room, plumbing and septic.

## Plans and documents

### Whole house
- [Floor plans](house/floor-plans-v1.html) (interactive)
- [3D model with airflow](house/airflow-3d-v1.html) (interactive, rotate with your finger or mouse)
- [Electrical layout](house/electrical-layout-v1.html) (where lights, switches and outlets go)
- [Electrical materials](house/electrical-materials.md) (material list and cost)

### Steel stair (Phase 3)
- [Project brief: design, costs, status](stairs/stair-project-brief.md)
- [Full plan PDF v3.3](stairs/Stair_Works_Phase3_Plan_v3.3.pdf)
- [Shopping list (14 Nov)](stairs/shopping-list-14nov.md)

### Front gate
- [Gate plan (draft)](gate/gate-plan-draft.md)
- [Gate drawing (draft)](gate/gate-elevation-draft.png)


## How the website is built (for whoever updates it)
- The website is for viewing only. The homepage is `index.html`; every plan page shares one look from `_layouts/plan.html`.
- **New or changed plan page:** copy `_templates/plan-template.md` into the right folder (`rooms/`, `stairs/`, `gate/`, `house/`), fill in the header (title, status, cost, price_source, updated) and write the body in plain Markdown. GitHub Pages turns `rooms/kitchen.md` into `rooms/kitchen.html`. Then add a card for it on `index.html`.
- Tag every price **Local** (receipt or local quote) or **Online** (online estimate). Set `price_source` to `local`, `online` or `mixed`.
- Keep the city name, street address, GPS coordinates and any claude.ai links off every page.
- **End of every session:** list what changed, copy updated files in, update the homepage status and "Last updated" date, push, and check the site shows the new version.

## How to get updates
- On [GitHub](https://github.com/tatayotter/navarro-house), click **Watch** (top right) → **All activity** to get an email (needs a free GitHub account) whenever something changes.
- The [History](https://github.com/tatayotter/navarro-house/commits/main) page shows every update with a short note of what changed.
