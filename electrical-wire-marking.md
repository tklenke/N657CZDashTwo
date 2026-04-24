# Wire Marking Standard

::: approved
**APPROVED** — 2026-04-23
:::

All wiring on N657CZ uses the EA wire marking standard described on this page. Wire labels appear at both ends of each wire segment and follow a three-part format.

## Label Format

A wire label consists of up to three parts:

| Part | Description | Length | Example |
|------|-------------|--------|---------|
| System Code | Identifies the major system the wire belongs to | 1 character | `L` |
| Circuit ID | Unique circuit number, matching the master schematic net name | 2–4 characters | `10` |
| Segment ID | Sequential letter identifying physical segments within the same net | 1 character (optional) | `A` |

**Full label example:** `L10A`
- `L` — Lighting system
- `10` — Circuit 10 (Landing/Taxi Light Power circuit)
- `A` — First physical segment of that circuit

### Segment ID Usage

A single electrical net often spans multiple physical wire segments separated by switches, fuses, or connectors. Each segment receives the same System Code and Circuit ID, with a different Segment ID letter.

**Example — Landing/Taxi Light circuit (L10):**

| Segment | Label | Wire Run |
|---------|-------|----------|
| Bus to switch | `L10A` | Main Bus → Landing Light Taxi Switch |
| Switch to landing light | `L10B` | Landing Light Taxi Switch → Landing Light |
| Switch to taxi light | `L10C` | Landing Light Taxi Switch → Taxi Light |

If more than 26 segments are needed, extend with two-letter suffixes: AA, AB, AC, etc.

## System Codes

System codes follow MIL-W-5088L Appendix B. Codes used on N657CZ:

| Code | System |
|------|--------|
| A | Avionics |
| D | Data bus (CAN, ARINC 429, RS-232/422 — see [[Wire Marking Standard#Data Bus Wiring|electrical-wire-marking#data-bus-wiring]]) |
| E | Engine Instrument |
| G | Ground |
| L | Lighting |
| M | Miscellaneous Electrical |
| P | DC Power (generation, distribution, battery) |

## Wire Color Conventions

Wire insulation color follows system code where practical. Color coding is a visual aid — it does not replace the wire label.

| System Code | System | Wire Color |
|-------------|--------|------------|
| P | Power (DC) | Red |
| G | Ground | Black |
| L | Lighting | White |
| A | Avionics | Blue |

Multi-conductor bundles may use different colors for individual conductors within the bundle. Always verify connections against the schematic.

## Wire Characteristics

Physical properties of the wire are not encoded in the label. They are recorded in the wiring log and schematic notes:

| Characteristic | Location | Example |
|----------------|----------|---------|
| Wire gauge | Wiring log / schematic notes | 20 AWG |
| Insulation type | Wiring log / installation standard | Teflon/Tefzel (MIL-W-22759) |
| Endpoints | Derived from schematic | Main Bus to ANL Fuse |

## Data Bus Wiring

Data bus wiring uses system code **D**. The Circuit ID encodes bus type and link number. Data bus cables do not follow the single-wire color convention — cable type is determined by the applicable bus standard. No D-prefix wires are currently installed; these circuit IDs are reserved for use when data bus cabling is added.

### Circuit ID Ranges

| Range | Bus Type | Description |
|-------|----------|-------------|
| D001–D009 | CAN bus | Shared bus wiring |
| D010–D099 | ARINC 429 | Point-to-point differential links |
| D100+ | Non-bus | RS-232, RS-422, and discrete data wires |

### CAN Bus (D001–D009)

CAN bus uses a daisy-chain topology. Two circuit IDs are reserved for the differential pair:

- **D001** — CAN_L (low side)
- **D002** — CAN_H (high side)

The Segment ID identifies each physical hop in the chain. Both wires of a CAN pair for the same hop carry the same Segment ID letter.

| Segment | CAN_L Label | CAN_H Label | Wire Run |
|---------|-------------|-------------|----------|
| First hop | `D001A` | `D002A` | LRU 1 → LRU 2 |
| Second hop | `D001B` | `D002B` | LRU 2 → LRU 3 |
| Third hop | `D001C` | `D002C` | LRU 3 → LRU 4 |

Cable type: shielded twisted pair per ISO 11898 or equipment manufacturer specification.

### ARINC 429 (D010–D099)

ARINC 429 is unidirectional and point-to-point. Each link uses two consecutive circuit IDs for its differential pair — even number for the A wire (positive), odd for the B wire (negative). A Segment ID is not normally required since there are no intermediate junctions.

| Link | A Wire | B Wire |
|------|--------|--------|
| Link 1 | `D010` | `D011` |
| Link 2 | `D012` | `D013` |
| Link N | `D010 + (N−1)×2` | `D011 + (N−1)×2` |

The range D010–D099 supports up to 45 point-to-point ARINC 429 links. Cable type: shielded twisted pair per ARINC 429 Part 1 specification.

### Non-Bus Data Wiring (D100+)

RS-232, RS-422, and discrete signal wires are numbered sequentially starting at D100. Each wire receives its own Circuit ID. Related wires in a multi-conductor interface (e.g., TX, RX, and ground of an RS-232 link) are assigned consecutive numbers. Cable type per the equipment interface specification.

## Physical Marking

Mark each wire segment at both termination points. (MIL-STD-681E)

Marking methods:
- Adhesive number tape (e.g., Digi-Key digit tape)
- Heat-shrink sleeve with printed markings

Markings must be visible and readable after installation.

## References

| Document | Relevance |
|----------|-----------|
| MIL-STD-681E — *Identification Coding and Application of Hookup and Lead Wire* | Systems III and IV define functional coding by printed markings and coding of interconnecting wiring |
| MIL-W-5088L — *Wiring, Aerospace Vehicle* | Appendix B defines circuit function letters (system codes) |
| AC 43.13, Chapter 11 — *Aircraft Electrical Systems* | FAA-accepted methods for wiring installation and identification (AC 43.13, ch11_p001) |
