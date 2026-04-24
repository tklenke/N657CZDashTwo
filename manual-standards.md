# Manual Standards

::: draft
**DRAFT** — Not yet reviewed.
:::

This page is the authoritative reference for how this manual is organized and why. It records structural decisions about the manual's scope, section organization, and content placement rules. When a future editor needs to decide where content belongs or how to structure a new page, the answer should be here.

For decisions specific to individual sections, see [[Section Notes|manual-standards-section-notes]].

For writing and formatting standards, see:
- [[Writing Style|manual-standards-writing-style]] — voice, tense, and language rules
- [[Formatting|manual-standards-formatting]] — page naming, NOTE callouts, citations, cross-references
- [[Page Templates|manual-standards-page-templates]] — standard page structures by page type

---

## Manual Scope

This is a maintenance manual only. Fabrication and Pilot Operating Handbook (POH) content are out of scope. Build procedures are not needed for a completed aircraft, and POH content belongs in the POH.

---

## Version and Revision Information

Version and revision metadata is not embedded in page content. It is provided automatically by the wiki.

Every page displays a print footer showing the date the page was last edited. This date is derived from the git commit that recorded the most recent change to that page. A printed copy can be verified against the current online version using the last-edited date in the footer.

See [[Record of Revisions|record-of-revisions]] for how to interpret revision history and use the built-in recent changes view.

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

## Connector Pinout Sub-Pages

Connector pinout tables for avionics LRUs are on dedicated sub-pages (`[component-slug]-pinouts`) rather than inline on the component page. The component page links to the pinout sub-page from its Specifications section: "For full connector pin assignments, see [[Connector Pinouts|[component-slug]-pinouts]]."

Pinout sub-pages are not listed in the TOC. They are accessed through their parent component page.

**Page structure:**
- H1: "[Component Name] Connector Pinouts ([Model])"
- Intro paragraph: source document and section; connector-to-harness mating relationship
- One `##` section per connector with designation and type (e.g., `## J291 — 9-pin D-sub`)
- Table: Pin | Function | I/O, with pin column right-aligned

Pinout tables for multi-connector LRUs are large and break the flow of the component page. Keeping them on a dedicated sub-page makes both pages more readable.

---

## Section 16: Electrical Schematics on Separate Pages

Each KiCad electrical schematic sheet is published as its own dedicated page. The TOC entry for `electrical-bus-architecture` is labeled "Bus Architecture and Schematics" to indicate where schematics are found.

The four schematic pages (not listed in the TOC — accessed from `electrical-bus-architecture`):

| Page | Covers |
|------|--------|
| `electrical-schematic-top` | Top-level power distribution |
| `electrical-schematic-avionics` | Avionics electrical |
| `electrical-schematic-alarm-lighting` | Alarm and lighting system |
| `electrical-schematic-mechanical` | Mechanical systems |

Separate pages produce clean print output and allow precise cross-linking — any page that references a specific subsystem can link directly to the relevant schematic sheet.

The `electrical-bus-architecture` page is the hub: it describes the bus architecture and links to all four schematic pages.

---

## Section 16: Wire Marking Standard and Wire Cross-Reference

Wire marking is documented on two dedicated pages in Section 16:

- **`electrical-wire-marking`** (Wire Marking Standard) — the complete EA wire marking standard: label format, system codes, wire color conventions, and data bus circuit ID ranges. Source: `docs/references/electrical/ea_wire_marking_standard.md`.

- **`electrical-wire-reference`** (Wire Cross-Reference) — a formatted table of every wire on N657CZ: wire label, from/to endpoints, gauge, color, and length. Source: `docs/references/electrical/wire_bom.csv`.

The `electrical-wiring` page covers physical installation standards (routing, clamping, bundling) and links to `electrical-wire-marking` for labeling. Avionics pages that discuss CAN bus or ARINC 429 wiring link to `electrical-wire-marking` for the D-code circuit ID ranges.
