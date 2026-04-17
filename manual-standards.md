# Manual Standards

This page is the authoritative reference for how this manual is organized and why. It records structural decisions about the manual's scope, section organization, and content placement rules. When a future editor needs to decide where content belongs or how to structure a new page, the answer should be here.

For decisions specific to individual sections, see [[Section Notes|section-notes]].

---

## Manual Scope

This is a maintenance manual only. Fabrication and Pilot Operating Handbook (POH) content are out of scope. Build procedures are not needed for a completed aircraft, and POH content belongs in the POH.

---

## Version and Revision Information

Version and revision metadata is not embedded in page content. It is provided automatically by the wiki.

Every page displays a print footer showing the date the page was last edited. This date is derived from the git commit that recorded the most recent change to that page. A printed copy can be verified against the current online version using the last-edited date in the footer.

See [[Record of Revisions|record-of-revisions]] for how to interpret revision history and use the built-in recent changes view.

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
