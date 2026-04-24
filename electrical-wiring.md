# Wiring

::: draft
**DRAFT** — Not yet reviewed.
:::

Physical wiring installation standards for N657CZ. For wire labeling and identification, see [[Wire Marking Standard|electrical-wire-marking]].

## Wire Specification

All wiring on N657CZ uses MIL-W-22759/16 (ETFE/Tefzel insulation, 150 °C rated, tin-coated stranded copper conductor). This wire is qualified for open-harness construction per MIL-W-5088L Appendix A. Do not substitute wire that is not rated for open airframe use. (AC 43.13-1B §11-77)

## Routing

Route wire bundles in accessible areas protected from personnel traffic, cargo, and maintenance activity. Bundles must not be positioned where they could be used as handholds or where removal of other equipment could damage them. (AC 43.13-1B §11-115)

### Separation from Flammable Fluids

Route wiring above fuel, oil, and hydraulic lines. (AC 43.13-1B §11-126)

| Condition | Minimum separation |
|-----------|-------------------|
| Preferred — route above fluid lines | 6 inches |
| When 6-inch spacing is not practicable | 2 inches |
| When positively clamped adjacent to fluid line | 1/2 inch |

When wiring must run parallel to a fluid line with less than 6-inch clearance, it must be clamped to the same structural member as the fluid line to prevent relative motion. Do not use fluid-line clamps as wire bundle support — install dedicated wire clamps.

### Separation from Heat Sources

Route wiring away from exhaust stacks, heating ducts, resistors, and other high-temperature equipment. In unavoidable hot areas, use high-temperature insulation (fiberglass or PTFE). Do not route wire with soft plastic insulation through high-temperature areas. (AC 43.13-1B §11-124, §11-96z)

### Separation from Flight Controls

Maintain at least 1/2-inch clearance between wiring and mechanical flight controls when a light hand pressure is applied to the wires or controls in the direction of the controls. Where this clearance cannot be maintained, provide additional structural support. Clamps used near movable controls must use steel hardware. (AC 43.13-1B §11-125, §11-96dd)

### Chafe Protection

Where wiring cannot be clamped clear of structure, install grommets or chafe strips. Wiring must maintain at least 3/8-inch clearance from structure at bulkhead penetrations. (AC 43.13-1B §11-115)

Where wire bundles pass through bulkheads, install a grommet if the bundle clearance to the cutout edge is less than 3/8 inch. The grommet may be cut at 45° for installation if cemented in place with the slot at the top. (AC 43.13-1B §11-146d)

## Bundling and Ties

Comb wires within a group so they lie parallel; this minimizes insulation abrasion within the bundle. (AC 43.13-1B §11-116)

Apply ties or lacing at the following intervals: (AC 43.13-1B §11-96i, §11-136)

| Location | Tie interval |
|----------|-------------|
| Main harness runs | Every 24 inches or at each structural support |
| Service loops (instrument panel harnesses) | 4–6 inches |
| Chafe-protection sleeving | Every 6–8 inches |

Use braided lacing tape (MIL-T-43435) or plastic cable straps meeting MS17821/MS17822 for ties. Cable straps may not be used in high-vibration areas, wheel wells, or areas adjacent to flap/control hinges. Do not use straps as primary support on vertical runs where slack migration could cause chafing. (AC 43.13-1B §11-158, §11-146)

### Slack and Bend Radius

Install wiring with enough slack that bundles are not under tension. Leave sufficient slack at connectors and terminal lugs to permit two reterminations without replacing the wire. (AC 43.13-1B §11-118)

Wire deflection between supports must not exceed 1/2 inch unless the bundle cannot contact any chafe surface. (AC 43.13-1B §11-118)

| Wire type | Minimum bend radius |
|-----------|-------------------|
| Wire group or bundle | 10× largest wire OD |
| At breakouts and direction reversals (supported) | 6× wire OD |
| RF/coaxial cables | 6× cable OD |
| Service loop harnesses | 3× harness diameter |

Do not apply sharp bends to hot-stamped wire labels. (AC 43.13-1B §11-117)

### Drip Loops

Where wiring enters a connector, terminal block, or junction box from above, form a drip loop — dress the wire downward past the connector entry, then back up — to prevent moisture from running into the connector. Where wiring must enter from below, seal the entry or provide sufficient slack for a drip loop. (AC 43.13-1B §11-118A)

## Clamping

Support wire bundles with MS-21919 cushion clamps lined with nonmetallic material, spaced no more than 24 inches apart. Clamps should fit snugly without pinching wires; the bundle must not slide through the clamp under slight axial pull. (AC 43.13-1B §11-146)

| Requirement | Rule |
|------------|------|
| Maximum clamp spacing | 24 inches |
| Clearance from bulkhead cutout before grommet required | < 3/8 inch |
| Clamp attachment hardware orientation | Hardware above the clamp |

Rest the back of the clamp against structure where practical. Use stand-offs to maintain clearance between wiring and structure — tape and tubing are not acceptable substitutes for stand-offs. (AC 43.13-1B §11-96b)

Do not use plastic clamps or cable ties in locations where failure could result in contact with movable flight controls or chafing of essential wiring. (AC 43.13-1B §11-146)

## Shielding

Shielded wiring is used on circuits susceptible to electromagnetic interference (EMI). Shields are connected to airframe ground at one or both ends, depending on the circuit function. Shield coverage of 85% or greater is recommended. (AC 43.13-1B §11-89, §11-106)

Route shielded data bus and sensitive avionics wiring away from high-current power wiring. EMI coupling increases with length of parallel runs and decreases with separation distance. Where separation cannot be maintained, use shielded cable with adequate coverage. (AC 43.13-1B §11-106)

### Coaxial and RF Cables

Coaxial cables require special handling. Kinking or crushing a coaxial cable can damage it internally with no visible external evidence. (AC 43.13-1B §11-120, §11-121)

- Do not clamp coaxial cable tightly enough to distort its cross section.
- Do not bend coaxial cable tighter than 6× the cable OD.
- Do not use coaxial cable as a handhold or structural support.
- Do not use coaxial cable with a solid center conductor — use stranded center only.
- Use cushion clamps on coaxial cable; metal clamps may distort the cable geometry.

## Connector Installation

Inspect connectors and verify the following at each installation and inspection: (AC 43.13-1B §11-100)

- Connectors are fully mated; coupling ring is at the fully mated indicator line.
- Coupling nut is safetied as required by the component manufacturer.
- Cable clamp backshells (MIL-C-85049) are installed on all applicable MS connectors.
- Silicone tape is wrapped inside MS3057 cable clamp adapters before tightening to maintain grip on the wires.
- Unused receptacles are capped with metal or composite dust caps attached by their normal mating method.
- No evidence of overheating (discoloration), corrosion, or cracking of potting compound.
- Wires exiting connectors are routed so moisture drains away from the connector body.

Where identical connectors are installed in adjacent locations, route and clamp wiring such that connectors cannot be interchanged incorrectly, and clearly identify the wiring. (AC 43.13-1B §11-100i)

## System Separation

Route wires of redundant aircraft systems in separate bundles and through separate connectors to prevent a single fault from disabling multiple systems. Route power feeders from separate sources in separate bundles. Attach ground wires from separate power sources to separate airframe attachment points. (AC 43.13-1B §11-105)

Colored plastic cable ties or lacing tape may be used to identify separated system bundles. Replace with the same color during maintenance. (AC 43.13-1B §11-105)

## Wire Identification

All wire segments are labeled per the [[Wire Marking Standard|electrical-wire-marking]]. Labels must be present at both ends of each segment and readable after installation. Identify wiring at intervals of not more than 15 inches. (AC 43.13-1B §11-96gg)

## References

| Document | Relevance |
|----------|-----------|
| AC 43.13-1B, Chapter 11 — *Aircraft Electrical Systems* | FAA-accepted methods for wiring installation, clamping, routing, shielding, and inspection (AC 43.13, ch11_p001) |
| MIL-W-22759/16 | Wire specification: ETFE insulated, tin-coated stranded copper, 150 °C, open wiring |
| MIL-W-5088L / SAE AS50881A — *Wiring, Aerospace Vehicle* | Wire selection criteria; Appendix A defines open-wiring qualified wire types |
| MS-21919 | Standard cushion clamp specification for wire bundle support |
