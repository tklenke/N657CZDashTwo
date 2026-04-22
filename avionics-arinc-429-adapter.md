# ARINC 429 Adapter (GAD 29)

::: draft
**DRAFT** — Not yet reviewed.
:::

## Description

The Garmin GAD 29 is an ARINC 429 (Aeronautical Radio Incorporated) data adapter that interfaces the G3X avionics suite with external IFR navigators. On N657CZ, the GAD 29 connects to the GNC 355 IFR GPS navigator, receiving ARINC 429 navigation data and converting it to the G3X CAN bus. This enables the GDU 460 to display CDI deviation and glideslope guidance from the GNC 355, and allows the autopilot to follow GPS steering commands from the navigator. (GarminG3XInstallationManual_az.pdf, Section 4.1)

The unit is mounted remotely in the avionics bay forward of the instrument panel. It has two connectors on the front face: J291 (9-pin D-sub) and J292 (25-pin D-sub). A status LED on the outer case indicates operating status.

## Specifications

| Item | Value | Source |
|------|-------|--------|
| Unit part number | 011-03236-00 | GarminG3XInstallationManual_az.pdf, Table 4-1 |
| ARINC 429 transmitters | 2 (low speed) | GarminG3XInstallationManual_az.pdf, Section 4.1 |
| ARINC 429 receivers | 4 (low speed) | GarminG3XInstallationManual_az.pdf, Section 4.1 |
| CAN network ports | 1 | GarminG3XInstallationManual_az.pdf, Section 4.1 |
| Current draw | 0.2 A | Engineering report (LRU24) |
| Power source | G3X bus | Engineering report |
| Power wire | A11A, 24 AWG M22759/16 | Engineering report |
| Ground wire | G106A, 24 AWG M22759/16 | Engineering report |
| Mounting hardware | 4× #10-32 pan or hex head screws | GarminG3XInstallationManual_az.pdf, Section 4.5 |

## Connector Pinouts

Pinout data from GarminG3XInstallationManual_az.pdf, Section 23.2.

### J291 — 9-pin D-sub

*Viewed looking at connector on unit.*

| Pin | Function | I/O |
|----:|----------|:---:|
| 1 | CAN HI | I/O |
| 2 | CAN LO | I/O |
| 3 | RESERVED | — |
| 4 | RESERVED | — |
| 5 | RESERVED | — |
| 6 | GROUND | — |
| 7 | AIRCRAFT POWER 1 | In |
| 8 | AIRCRAFT POWER 2 | In |
| 9 | GROUND | — |

### J292 — 25-pin D-sub

*Viewed looking at connector on unit. Pins marked \* have two alternative functions depending on unit variant (GAD 29/29B/29C/29D).*

| Pin | Function | I/O | Alternate Function | Alt I/O |
|----:|----------|:---:|--------------------|:-------:|
| 1 | RESERVED | — | AC REFERENCE HI\* | In |
| 2 | RESERVED | — | AC REFERENCE LO\* | In |
| 3 | RESERVED | — | HDG/CRS VALID\* | Out |
| 4 | ARINC RX 4B | In | | |
| 5 | ARINC RX 3B | In | | |
| 6 | ARINC TX 2B | Out | | |
| 7 | ARINC TX 2B | Out | | |
| 8 | RESERVED | — | HEADING ERROR HI\* | Out |
| 9 | CAN TERM 1 | — | | |
| 10 | ARINC RX 2B | In | | |
| 11 | ARINC RX 1B | In | | |
| 12 | ARINC TX 1B | Out | | |
| 13 | ARINC TX 1B | Out | | |
| 14 | GROUND | — | HEADING ERROR LO\* | In |
| 15 | RESERVED | — | COURSE ERROR HI\* | Out |
| 16 | ARINC RX 4A | In | | |
| 17 | ARINC RX 3A | In | | |
| 18 | ARINC TX 2A | Out | | |
| 19 | ARINC TX 2A | Out | | |
| 20 | GROUND | — | COURSE ERROR LO\* | In |
| 21 | CAN TERM 2 | — | | |
| 22 | ARINC RX 2A | In | | |
| 23 | ARINC RX 1A | In | | |
| 24 | ARINC TX 1A | Out | | |
| 25 | ARINC TX 1A | Out | | |

## Inspection

### Connectors

- Check harness connectors P291 (9-pin) and P292 (25-pin) for full seating and latch security.
- Inspect pins and sockets for corrosion, bent pins, or pushed-back contacts.
- Inspect backshell hardware for security and integrity.

### Mounting

- Verify all four #10-32 mounting screws are present and secure.
- Inspect the mounting surface for cracks or deformation at screw locations.

### Status LED

The GAD 29 has a status LED on the outer case. Verify the LED indicates normal operation on power-up (GarminG3XInstallationManual_az.pdf, Section 31.1.1).

### General

Inspect the unit for physical damage, corrosion, and moisture ingress.

## Procedures

The GAD 29 has no complex removal or installation requirements. Removal and installation does not require special tools.

### Removal

1. Remove power from the G3X bus (SW11 off).
2. Disconnect harness connectors P291 and P292.
3. Remove the four #10-32 mounting screws.
4. Remove the unit.

### Installation

1. Position the unit and install the four #10-32 mounting screws. (GarminG3XInstallationManual_az.pdf, Section 4.5)
2. Connect harness connectors P291 and P292. Verify each connector is fully seated and latched.
3. Restore power and verify the status LED indicates normal operation.
