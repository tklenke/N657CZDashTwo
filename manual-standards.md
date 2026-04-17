# Manual Standards

[TOC]

This page is the authoritative reference for how this manual is organized and why. It records structural decisions about the manual's scope, section organization, and content placement rules. When a future editor needs to decide where content belongs or how to structure a new page, the answer should be here.

---

## Manual Scope

This is a maintenance manual only. Fabrication and build content is out of scope.

The aircraft is built. The manual is for the owner/maintainer performing ongoing maintenance and inspection. Build procedures are not needed and would create confusion about what applies to a completed aircraft.

---

## Version and Revision Information

Version and revision metadata is not embedded in page content. It is provided automatically by the wiki.

Every page displays a print footer showing the date the page was last edited. This date is derived from the git commit that recorded the most recent change to that page. A printed copy can be verified against the current online version using the last-edited date in the footer.

See [[Record of Revisions|record-of-revisions]] for how to interpret revision history and use the built-in recent changes view.

---

## Section 6: Servicing as Master Index

Section 6 is a master index of all servicing tasks, not a collection of procedures. Each task entry states the service interval and points to the full procedure in its home section.

A maintainer planning a service event needs a single place to see everything that requires attention. Duplicating procedures in Section 6 would create maintenance burden and risk of conflicting information.

Procedures such as oil change live in Section 14 (Power Plant). Section 6 lists "Oil and Filter" with interval and a pointer to Section 14.

**TOC structure:** Two pages in Section 6:
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

Exterior Finish and Fueling may warrant their own pages if the content volume (product notes, cautions, technique guidance) justifies it. Writer decides based on content.

---

## Section 7: Inspection Structure

Three inspection tiers:

- 7.1 Annual Condition Inspection — single comprehensive checklist page
- 7.2 Post-Cross-Country Check — focused on stress and extended-use items
- 7.3 Periodic Check — mid-season; broader than 7.2 but lighter than the annual

Experimental aircraft operate under annual condition inspection only. The 7.2 and 7.3 tiers reflect practical maintenance intervals without implying FAA-mandated tach-time requirements.

The annual condition inspection is kept as a single page (not broken into sub-pages by system) to preserve its utility as a checklist. If it grows unwieldy, reconsider at the next architectural review.

---

## Alternators: Power Plant, Not Electrical

Alternator maintenance procedures live in Section 14 (Power Plant), not Section 16 (Electrical System). Section 16 includes a cross-reference pointer to Section 14.

Alternators are engine-driven mechanical components. Their maintenance (belt tension, brush inspection, output testing) is physically performed at the engine. The electrical section covers distribution and consumption of power after it is generated, not the generation hardware itself.

---

## Panel and Cover Removal Procedures Live in Section 9

Removal and installation procedures for all panels and covers are in Section 9 (Canopy and Panels). Other sections that reference those panels include a cross-reference pointer rather than duplicating the procedure.

Single source of truth for panel procedures. A maintainer working on cabin access or firewall components should not have to reconcile two versions of the same removal steps.

**Examples:**
- Cabin Interior (Section 10) links to Armrests and Firewall Cover Panel in Section 9
- Any section requiring instrument panel access links to IP Access Panel in Section 9

---

## TOC Depth: Component-Specific Procedures Are Not Listed

Type 2 Procedure pages that are specific to a single component are not listed in the TOC. They are accessed through their parent component's Type 1b page.

The TOC reflects the manual's structure at the component and system level. Listing every procedure would make the TOC unwieldy and suggest a flat organization that does not exist. A maintainer navigates to the component page first; from there, procedures are one click away.

**What belongs in the TOC:**
- All Type 1a System pages and Type 1b Component pages
- Section-level index pages (e.g., Servicing, Lubrication, Annual Condition Inspection)

**What does not belong in the TOC:**
- Component-specific procedures, even substantial ones (e.g., Canopy Cleaning, Wing Removal and Installation, Battery Removal, Brake Fluid Change) — these are accessed through their parent component page

---

## List Ordering: Alphabetical by Default

Lists of pages, items, or components are ordered alphabetically by default. This can be overridden when a different order is clearly better (e.g., procedural sequence, logical grouping), but alphabetical is the starting assumption.

Alphabetical ordering is predictable and makes items findable without requiring the reader to understand the author's organizational logic. Arbitrary ordering creates maintenance burden as items are added over time.

---

## Section 2: Safety Precautions Structure

Five pages covering hazards specific to this aircraft:

- Composite Material Hazards
- Electrical Safety
- Fire and Fuel Hazards
- Fluids and Chemicals
- General Shop Safety

Generic shop safety content is excluded. Composite material hazards are included because fiberglass dust and epoxy are present in both repair work and routine inspection of this airframe.

---

## Section 3: Aircraft General Structure

Three pages:

- 3.1 General Layout and Configuration
- 3.2 Aircraft Dimensions and Weight
- 3.3 Systems Overview

Systems Overview gives a maintainer context before diving into individual systems. A high-level summary with cross-references reduces the chance of someone working on a system without understanding how it fits into the whole.

---

## Section 4: Ground Handling Structure

Four pages:

- 4.1 Towing Procedures
- 4.2 Jacking and Leveling
- 4.3 Tiedown and Parking
- 4.4 Storage

Storage is a maintenance task in its own right (fuel stabilizer, pitot cover, control locks, etc.).

---

## Section 17: Instruments Folded into Avionics

Section 15 (Instruments) is eliminated. Instrument content is covered in Section 17 (Avionics).

The aircraft has a full glass panel (GDU 460 PFD, G5 backup, GEA 24 EIS). The traditional instruments/avionics boundary assumes steam gauges. On this aircraft, the displays and the avionics generating the data are the same hardware. Splitting them across two sections would force arbitrary decisions about where content belongs and require cross-referencing for every topic.

---

## Weight and Balance as Standalone Section

Weight and Balance is its own top-level section (Section 4), not a sub-section of Aircraft General.

W&B is a recurring maintenance task with its own procedures, not just background information. It warrants a dedicated section so a maintainer can find it directly.
