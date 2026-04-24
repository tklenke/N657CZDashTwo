# Bus Architecture and Schematics

::: draft
**DRAFT** — Not yet reviewed.
:::

N657CZ uses a four-bus electrical architecture: Battery Bus, Endurance Bus, Main Bus, and G3X Bus. Each bus serves a distinct role in the load-shedding philosophy that governs the aircraft's electrical system design.

## Battery Bus (FH1)

The Battery Bus is always hot — it is connected directly to the battery and is not switched by the master switch. Its purpose is to power a small set of items that must remain active regardless of master switch position.

The key design decision is placing the electronic ignition (Plasma III) on the Battery Bus. The electronic ignition behaves identically to the magneto from the cockpit: when the ignition switch is ON, that system is armed and ready. By powering the electronic ignition from the always-hot Battery Bus, the entire electrical system can be shut down with no adverse effect on engine ignition. This eliminates the need to track ignition power separately from the master switch.

| Item | Reference |
|------|-----------|
| Electronic Ignition | LRU6 (Plasma III) |
| Dome Lights | LRU81 |
| Canopy Actuator | LRU14 |
| Endurance Bus Feed | via relay R2 |

The Battery Bus also provides the feed path to the Endurance Bus through a relay, allowing essential equipment to operate on battery-only power when the master contactor is open.

## Endurance Bus (FH2)

The Endurance Bus carries the minimum set of equipment needed to navigate safely to landing on battery power alone after an alternator failure or other electrical emergency. The design goal is that a fully charged battery can power the Endurance Bus for a duration equal to or greater than the aircraft's fuel endurance — so battery capacity, not fuel, is never the limiting factor.

When the Endurance Bus is in use in battery-only mode, the pilot switches off all Main Bus loads. At that point, only the items below remain powered. Once a landing clearance is received, the master can be re-closed to use any remaining battery energy for accessory loads.

| Item | Reference |
|------|-----------|
| G3X Bus (feeds GDU 460, GEA 24, GAD 29, GSU 25C) | FH6 feed |
| VHF Comm 1 | LRU21 (GTR 20) |
| Audio Panel | LRU22 (GMA 245) |
| Transponder / ADS-B | LRU28 (GTX 45R) |
| Backup Instrument | LRU26 (G5) |
| Magnetometer | LRU25 (GMU 11) |
| GNC 355 Nav (GPS/Nav only) | LRU10-N |

> **NOTE:** The GNC 355 Nav function is on the Endurance Bus; the GNC 355 Comm 2 function is on the Main Bus and is not available in battery-only operation.

## Main Bus (FH3)

The Main Bus carries all equipment not assigned to the Battery or Endurance Bus — items that can be deferred until final approach if operating on battery power alone. Normal operations use the full complement of Main Bus loads; shedding begins only when the alternator fails and battery conservation is needed.

| Item | Reference |
|------|-----------|
| Non-Impulse Magneto (switch circuit) | LRU7 |
| GNC 355 Comm 2 | LRU10-C |
| Autopilot Control Panel | LRU11 (GMC 507) |
| Autopilot Servos | LRU18, LRU19 (GSA 28 ×2) |
| Nav / Strobe Lights | LRU85, LRU89 |
| Landing Light | L7 |
| Taxi Light | L9 |
| USB Charger | LRU60 (GSB 15) |
| Seat Heater | LRU20 |
| Landing Brake Actuator | LRU15 |
| Nose Gear Actuator | LRU16 |
| Nose Gear Auto-Retract | LRU4 |

## G3X Bus (FH6)

The G3X Bus is a switched fuse block that distributes power to the core G3X LRUs. It is fed from the Endurance Bus, so the G3X suite (PFD, engine monitor, ARINC adapter, and ADAHRS) remains operational in battery-only mode.

| Item | Reference |
|------|-----------|
| Primary Flight Display | LRU33 (GDU 460) |
| Engine Data Acquisition | LRU32 (GEA 24) |
| ARINC 429 Adapter | LRU24 (GAD 29) |
| ADAHRS | LRU27 (GSU 25C) |

The VHF Comm 1 (GTR 20), Audio Panel (GMA 245), Transponder (GTX 45R), G5, GMU 11, and GNC 355 Nav are powered directly from the Endurance Bus rather than the G3X Bus, so they remain operational independently of the G3X Bus state.

## Schematics

The electrical schematic is divided into four sheets. Each sheet can be printed independently.

| Sheet | Description |
|-------|-------------|
| [[Top-Level|electrical-schematic-top]] | Overall power distribution: bus architecture, alternators, batteries, master contactor, and bus feed paths |
| [[Avionics|electrical-schematic-avionics]] | Power and ground wiring for the G3X avionics suite and associated LRUs |
| [[Alarm and Lighting|electrical-schematic-alarm-lighting]] | Interior and exterior lighting, warning indicators, and related controls |
| [[Mechanical Systems|electrical-schematic-mechanical]] | Actuators, fuel system, ignition, and other mechanical system loads |
