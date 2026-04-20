# ARINC 429 Adapter (GAD 29)

::: approved
**APPROVED** — 2026-04-19
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
