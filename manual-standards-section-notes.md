# Section Notes

::: approved
**APPROVED** — 2026-04-17
:::

This page records structural decisions about individual sections of the manual — how each section is organized, what it contains, and why. For general editorial and organizational rules that apply across the whole manual, see [[Manual Standards|manual-standards]].

---

## Section 2: Safety Precautions

Five pages covering hazards specific to this aircraft:

- Composite Material Hazards
- Electrical Safety
- Fire and Fuel Hazards
- Fluids and Chemicals
- General Shop Safety

Generic shop safety content is excluded. Composite material hazards are included because fiberglass dust and epoxy are present in both repair work and routine inspection of this airframe.

---

## Section 3: Aircraft General

Three pages:

- General Layout and Configuration
- Aircraft Dimensions and Weight
- Systems Overview

Systems Overview gives a maintainer context before diving into individual systems. A high-level summary with cross-references reduces the chance of someone working on a system without understanding how it fits into the whole.

---

## Section 5: Ground Handling

Four pages:

- Towing Procedures
- Jacking and Leveling
- Tiedown and Parking
- Storage

Storage is a maintenance task in its own right (fuel stabilizer, pitot cover, control locks, etc.).

---

## Section 4: Weight and Balance

Weight and Balance is its own top-level section, not a sub-section of Aircraft General.

W&B is a recurring maintenance task with its own procedures, not just background information. It warrants a dedicated section so a maintainer can find it directly.

---

## Section 6: Servicing

Section 6 is a master index of all servicing tasks, not a collection of procedures. Each task entry states the service interval and points to the full procedure in its home section.

A maintainer planning a service event needs a single place to see everything that requires attention. Duplicating procedures in Section 6 would create maintenance burden and risk of conflicting information.

**Two pages in Section 6:**
- [[Servicing|servicing]] — master index page; all tasks listed below are `##` sections within this page
- [[Lubrication|servicing-lubrication]] — its own page due to volume (comprehensive list of all lubrication points with intervals and pointers)

**Tasks indexed within the Servicing page** (each with interval and pointer to home section):

- Air Filter → Section 14 (Power Plant)
- Avionics Software Updates → Section 17 (Avionics)
- Battery Service → Section 16 (Electrical System)
- Brakes → Section 13 (Landing Gear and Brake System)
- Canopy and Door Seals → Section 9 (Canopy and Panels)
- Control Surface Hinges and Linkages → Section 12 (Flight Controls)
- Cooling System → Section 14 (Power Plant)
- Exterior Finish → standalone page if content volume warrants; home section not yet assigned
- Fuel Filters → Section 15 (Fuel System)
- Fueling → Section 15 (Fuel System) or standalone if content volume warrants
- Interior → Section 10 (Cargo and Cabin Systems)
- Lighting → Section 16 (Electrical System)
- Oil and Filter → Section 14 (Power Plant)
- Pitot/Static System → Section 17 (Avionics)
- Propeller → Section 14 (Power Plant)
- Spark Plugs → Section 14 (Power Plant)
- Tires and Wheels → Section 13 (Landing Gear and Brake System)
- Wing Removal and Installation → Section 8 (Structures)

Exterior Finish and Fueling may warrant their own pages if the content volume justifies it. Writer decides based on content.

---

## Section 7: Inspection

Three inspection tiers:

- 7.1 Annual Condition Inspection — single comprehensive checklist page
- 7.2 Post-Cross-Country Check — focused on stress and extended-use items
- 7.3 Periodic Check — mid-season; broader than 7.2 but lighter than the annual

Experimental aircraft operate under annual condition inspection only. The 7.2 and 7.3 tiers reflect practical maintenance intervals without implying FAA-mandated tach-time requirements.

The annual condition inspection is kept as a single page (not broken into sub-pages by system) to preserve its utility as a checklist. If it grows unwieldy, reconsider at the next architectural review.

---

## Section 9: Panel and Cover Removal Procedures

Removal and installation procedures for all panels and covers are in Section 9 (Canopy and Panels). Other sections that reference those panels include a cross-reference pointer rather than duplicating the procedure.

Single source of truth for panel procedures. A maintainer working on cabin access or firewall components should not have to reconcile two versions of the same removal steps.

**Examples:**
- Cabin Interior (Section 10) links to Armrests and Firewall Cover Panel in Section 9
- Any section requiring instrument panel access links to IP Access Panel in Section 9

---

## Section 14: Alternators Belong Here, Not in Electrical

Alternator maintenance procedures live in Section 14 (Power Plant), not Section 16 (Electrical System). Section 16 includes a cross-reference pointer to Section 14.

Alternators are engine-driven mechanical components. Their maintenance (belt tension, brush inspection, output testing) is physically performed at the engine. The electrical section covers distribution and consumption of power after it is generated, not the generation hardware itself.

---

## Section 17: Avionics (Instruments Folded In)

Section 15 (Instruments) is eliminated. Instrument content is covered in Section 17 (Avionics).

The aircraft has a full glass panel (GDU 460 PFD, G5 backup, GEA 24 EIS). The traditional instruments/avionics boundary assumes steam gauges. On this aircraft, the displays and the avionics generating the data are the same hardware. Splitting them across two sections would force arbitrary decisions about where content belongs and require cross-referencing for every topic.
