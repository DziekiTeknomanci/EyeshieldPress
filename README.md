# Create a README.md based on the provided PDF content

readme = """# 3D-Printed Linear Press

A compact, spring-loaded bench press you can print and assemble with common hardware. It uses 8 mm linear rods and LM8UU bearings for smooth motion and a toggle clamp for consistent pressure. Ideal for light press tasks, jigs, and small fixtures.

> This README is a conversion of the original “Press Documentation” PDF for use in a GitHub repository.

---

## Features
- 3D-printed frame with captive M4 threads
- Smooth guided motion on dual 8 mm shafts
- Optional LM8UU bearings (recommended) or printed bushings
- Adjustable spring preload (2–4 springs)
- Toggle clamp for quick, repeatable clamping
- Mounts to a simple wooden base with a raised step

---

## Bill of Materials (Hardware)

| Component | Qty | Example Link | Notes |
|---|:--:|---|---|
| M4 × 16 mm cap-head socket screws (CHSS) | 10 | [eBay](https://www.ebay.co.uk/itm/365366757336) | 20 mm also works. Cap-head looks neat, other heads are fine. |
| 8 mm linear rod, 150 mm length | 2 | [eBay](https://www.ebay.co.uk/itm/284132709444) | Cheaper in longer lengths—cut to size. (8 mm OD tube may work. Avoid threaded stud.) |
| LM8UU linear bearing | 2 | [eBay](https://www.ebay.co.uk/itm/283560168663) | Optional but highly recommended. |
| Expansion spring, 30–50 mm free length, 6–8 mm OD, 0.5–0.8 mm wire | 2–4 | [eBay](https://www.ebay.co.uk/itm/387764721266) | Two is usually enough; four anchor points allow tuning. |
| Toggle clamp | 1 | [Amazon](https://www.amazon.co.uk/dp/B08F4TG6J5) | Many types will work; large force not required. |

> You can modify the CAD to accommodate different hardware.

---

## Printed Parts & Settings

| Part | Qty | Walls | Solid Top/Bottom Layers | Infill | Notes |
|---|:--:|:--:|:--:|:--:|---|
| Press Bottom | 1 | 3 | 4 / 3 | Gyroid 10% (or Grid 20%) | — |
| Press Top | 1 | 3 | 3 / 4 | Gyroid 10% (or Grid 20%) | — |
| Press Cap | 1 | 3 | 3 / 3 | Gyroid 10% (or Grid 20%) | Tree support recommended for the overhang |
| Printed “Bearing” (optional) | 2 | 4 | 3 / 3 | **None (solid)** | Only if not using LM8UU; print at minimal layer height |

### Material Options
- **PETG** — Recommended for all parts.
- **PLA** — Works, but watch heat buildup; press faces may creep over time.
- **ABS** — Most durable; scale to ~**101%** or compensate for shrinkage in CAD.

### Logos/Text Variants
- *Plain:* Slice the “plain” STL, or in the 3MF set both “objects” to the same filament.
- *Embossed:* Delete the non-named objects in the 3MF; the text will be cut into the first layer.

### Printing With Contrast Colour
The logo/text versions use two bodies at Layer 1 so you can do a manual or automatic filament change for contrast. If you print **Top** and **Cap** together, you only need one change. PLA text on a PETG body is fine. Prefer the provided 3MF files so objects are already separated by filament.

---

## Tools & Consumables
- Soft hammer/mallet *(or steel hammer + wood block)*
- Vice or clamp *(for pressing LM8UU)*
- Lithium or other heavy grease *(light oil works but is sub-optimal)*
- 4×2″ timber off-cut (base & raised step)
- Hacksaw + sandpaper *(if cutting shafts)*
- **Optional:** M4 tap, 7.5 mm drill bit, 8 mm drill bit

---

## Assembly (≈10–20 min)

1. **Cut shafts (if needed).** If your 8 mm rod isn’t pre-cut, cut to **150 mm**. Tolerance is generous (> 10 mm), but make both the same length. Deburr and add a small chamfer with sandpaper. A cordless drill can act as a “lathe” while sanding.
2. **Prep threads.** *Press Top* and *Press Cap* include printed **M4** threads. Screws will self-tap; using an **M4 tap** makes it easier.
3. **Size holes.** Open up the outer holes on *Press Top* with an **8 mm** bit (hand-twisting is fine). Size the matching holes on *Press Bottom* and *Press Cap* to **7.5 mm** so the shafts fit tightly there.
4. **Install shafts (bottom).** Using a soft hammer, drive both shafts into the two large holes on *Press Bottom* until flush with the underside. Stack *Press Top* during this step to help alignment.
5. **Install bearings (top).** Pack **LM8UU** with heavy grease. Press them into the two 25 mm bores on *Press Top*. These are a friction fit—start gently with a mallet, then press fully using a vice or clamp.
6. **Assemble slide.** Carefully slide *Press Top* onto the shafts.
7. **Fit springs (lower).** Hook 2 springs into the lower anchor holes on *Press Top*. Pass the M4 socket screw through the spring loop and into the threaded hole. Do not overtighten. Up to 4 springs can be used.
8. **Fit cap.** Tap *Press Cap* onto the shaft ends. If loose, there is an **M4** hole to secure, but it’s usually not needed.
9. **Fit springs (upper).** Attach the spring tops to *Press Cap* as above.
10. **Mount to base.** Screw the press to a **wooden base**, then add a **raised “step”** 40–50 mm behind the base surface (a 4×2″ off-cut is perfect).
11. **Mount the toggle clamp.** Center the clamp over *Press Top* and adjust height so the press faces just meet. Extra clamp force only loads the press, not the work—there’s no benefit to overtightening and you can’t “over-press” the part unless you damage the tool.

---

## Tips
- Heavier grease inside LM8UU reduces rattle and wear; avoid losing balls from the open ends.
- If press fit tolerances are frustrating for your printer/material, consider lightly sanding bores or tweaking the CAD.
- Printed bushings work in a pinch but LM8UU will last longer and glide smoother.
