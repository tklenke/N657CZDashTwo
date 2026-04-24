# Wire Cross-Reference

::: draft
**DRAFT** — Not yet reviewed.
:::

Complete wire list for N657CZ, generated from the electrical schematic (revision 4). Each wire is identified by its label at both termination points.

For the wire labeling convention, see [[Wire Marking Standard|electrical-wire-marking]].

> **NOTE:** The Gauge column reflects the design gauge from the schematic. Where the schematic could not determine the circuit current, gauge is shown as —. The Notes column records any discrepancy between schematic-specified and installed gauge. Pin numbers in the source schematic are schematic symbol pins, not physical connector pins — for physical connector pin assignments, see the relevant component's pinouts page.

<!-- Source: docs/references/electrical/wire_bom.csv rev 4 (2026-04-23). When the schematic is revised and a new wire_bom.csv is generated, regenerate this table from the updated CSV. -->

## A — Avionics

| Wire Label | From | To | Gauge (AWG) | Color | Length (in) | Notes |
|------------|------|----|:-----------:|-------|------------:|-------|
| `A10A` | G3X Switch | Endurance Bus | — | Blue | 62.4 |  |
| `A10B` | G3X Switch | G3X Bus | — | Blue | 45.8 |  |
| `A11A` | Nav Intrfce (GAD 29) | G3X Bus | 24 | Blue | 59.2 |  |
| `A12A` | ADAHRS (GSU 25) | G3X Bus | 24 | Blue | 60.3 |  |
| `A13A` | EIS (GEA 24) | G3X Bus | 24 | Blue | 134.6 |  |
| `A14A` | PFD 10in (GDU 460) | G3X Bus | 24 | Blue | 38.6 |  |
| `A20A` | VHF Comm1 (GTR 20) | Endurance Bus | 18 | Blue | 70.3 |  |
| `A30A` | Endurance Bus | Audio Pnl w/ USB (GMA 245) | 22 | Blue | 65.8 |  |
| `A40A` | Endurance Bus | Xponder (GTX 45R) | 24 | Blue | 59.0 |  |
| `A50A` | Magnetometer (GMU 11) | Endurance Bus | 24 | Blue | 213.6 |  |
| `A60A` | Backup ASI (G5) | Endurance Bus | 24 | Blue | 53.7 |  |
| `A70A` | Main Bus | VHF Comm2 (GNC 355 Comm) | 20 | Blue | 69.5 |  |
| `A71A` | Endurance Bus | GPS Navigator (GNC 355 Nav) | 24 | Blue | 60.7 |  |
| `A80A` | Main Bus | AutoPilot Panel (GMC 507) | 24 | Blue | 62.9 |  |

## E — Engine Instrument / Engine Control

| Wire Label | From | To | Gauge (AWG) | Color | Length (in) | Notes |
|------------|------|----|:-----------:|-------|------------:|-------|
| `E22A` | Shunt 2 (GEA 24) | Shunt | 24 | Brown | 37.4 |  |
| `E23A` | Shunt 2 (GEA 24) | Shunt | 24 | Brown | 37.4 |  |
| `E31A` | Shunt 2 (GEA 24) | Fuse Link (FLK-1) | 24 | Brown | 38.3 | 20AWG |
| `E32A` | Shunt 2 (GEA 24) | Fuse Link (FLK-1) | 24 | Brown | 39.3 |  |
| `E40A` | Starter Contactor | Inline Fuse (IFH-2) | 6 | Brown | 34.4 | 4AWG > 6in |
| `E40B` | Starter Contactor | Starter (BCS206-149-12) | 6 | Brown | 85.6 | 4AWG |
| `E41A` | Main Bus | E IGN Switch | 20 | Brown | 61.3 |  |
| `E41B` | Electronic Ignition (Plasma III) | E IGN Switch | 20 | Brown | 114.4 | 20AWG |
| `E42A` | Main Bus | E IGN Switch | — | Brown | 61.3 |  |
| `E42B` | M IGN Switch | E IGN Switch | — | Brown | 25.0 |  |
| `E44A` | Starter Contactor | M IGN Switch | 24 | Brown | 118.6 | 4AWG |
| `E45A` | Non-Impulse Magneto | M IGN Switch | 18 | Brown | 123.1 | 20AWG SHIELDED |
| `E991A` | Shield Ground (W1) | M IGN Switch | — | Brown | 24.6 |  |
| `E992A` | Non-Impulse Magneto | Shield Ground (W2) | 18 | Brown | 24.9 |  |

## G — Ground

| Wire Label | From | To | Gauge (AWG) | Color | Length (in) | Notes |
|------------|------|----|:-----------:|-------|------------:|-------|
| `G10A` | Firewall Ground | Main Battery (ETX900-VNT) | 2 | Black | 31.4 | 4AWG |
| `G11A` | BATT/ALT DC POWER Switch | Panel Ground | — | Black | 53.5 |  |
| `G21A` | Aux Alt Off/On Switch | Panel Ground | — | Black | 51.5 |  |
| `G22A` | Engine Ground | Alternator (Main) | 6 | Black | 54.8 |  |
| `G23A` | Firewall Ground | Voltage Regulator (LRE1B-14) | 22 | Black | 31.9 | 20AWG |
| `G31A` | Voltage Regulator (PMR1D) | Firewall Ground | — | Black | 42.8 |  |
| `G32A` | Filter Capacitor (S8007-3) | Firewall Ground | — | Black | 41.8 |  |
| `G41A` | Engine Ground | Starter (BCS206-149-12) | 6 | Black | 73.0 |  |
| `G42A` | Starter Contactor | Firewall Ground | 24 | Black | 28.9 | 4AWG |
| `G43A` | Electronic Ignition (Plasma III) | Firewall Ground | 22 | Black | 30.1 |  |
| `G50A` | Brownout Battery (EXT104/EBBS) | Panel Ground | 16 | Black | 31.1 |  |
| `G52A` | E-Bus Alt Feed Switch | Panel Ground | — | Black | 43.9 | 22AWG |
| `G53A` | Relay (SPDT 12V 20A) | Panel Ground | — | Black | 42.9 |  |
| `G54A` | Low Voltage Monitor Module (BC207/AEC9005-101) | Panel Ground | 24 | Black | 52.4 |  |
| `G61A` | Ground Receptacle | Firewall Ground | — | Black | 58.9 | 4AWG |
| `G62A` | Ground Power Switch Breaker (2A) | Panel Ground | — | Black | 59.9 |  |
| `G101A` | Xponder (GTX 45R) | Panel Ground | 24 | Black | 48.0 |  |
| `G102A` | Magnetometer (GMU 11) | Panel Ground | 24 | Black | 219.8 |  |
| `G103A` | Backup ASI (G5) | Panel Ground | 24 | Black | 44.5 |  |
| `G104A` | Panel Ground | Audio Pnl w/ USB (GMA 245) | 22 | Black | 52.4 |  |
| `G105A` | VHF Comm1 (GTR 20) | Panel Ground | 18 | Black | 61.1 |  |
| `G106A` | Battery Contactor (S701-1) | Inline Fuse (IFH-2) | 24 | Black | 38.4 | 4AWG > 6in |
| `G107A` | ADAHRS (GSU 25) | Panel Ground | 24 | Black | 49.5 |  |
| `G108A` | Battery Contactor (S701-1) | BATT/ALT DC POWER Switch | 24 | Black | 126.7 | 22AWG |
| `G109A` | PFD 10in (GDU 460) | Panel Ground | 24 | Black | 49.0 |  |
| `G110A` | Interior Light, Forward | Panel Ground | 24 | Black | 63.4 |  |
| `G111A` | Interior Light, Aft | Panel Ground | 24 | Black | 139.8 |  |
| `G112A` | Lighting Controller | Panel Ground | 22 | Black | 43.8 |  |
| `G113A` | Panel Ground | Landing Light | 22 | Black | 72.3 |  |
| `G114A` | Panel Ground | Taxi Light | 22 | Black | 67.7 |  |
| `G115A` | Nav/Strobe Light, Right (Blaze 1R) | Panel Ground | 18 | Black | 333.0 |  |
| `G116A` | Nav/Strobe Light, Left (Blaze 1G) | Panel Ground | 18 | Black | 325.4 |  |
| `G117A` | USB Charger (GSB 15) | Panel Ground | 22 | Black | 52.8 |  |
| `G121A` | Firewall Ground | Fuel Boost Pump | 18 | Black | 48.5 |  |
| `G122A` | Electric Primer Valve | Firewall Ground | 18 | Black | 50.3 |  |
| `G123A` | Firewall Ground | Canopy Actuator | 18 | Black | 65.1 |  |
| `G124A` | Firewall Ground | Landing Brake Actuator | 18 | Black | 80.5 |  |
| `G125A` | Firewall Ground | Nose Gear Actuator | 16 | Black | 134.0 |  |
| `G126A` | Firewall Ground | Seat Heater | 18 | Black | 93.3 |  |
| `G127A` | Panel Ground | Pitot Probe | 18 | Black | 72.3 |  |
| `G128A` | Voltage Regulator (PMR1D) | Shunt (S870-20) | — | Black | 41.5 |  |
| `G129A` | Pitch Servo (GSA 28) | Panel Ground | 22 | Black | 46.9 |  |
| `G130A` | Panel Fan | Panel Ground | 24 | Black | 58.9 |  |
| `G1010A` | Panel Ground | GPS Navigator (GNC 355 Nav) | 24 | Black | 47.3 |  |
| `G1011A` | Panel Ground | AutoPilot Panel (GMC 507) | 24 | Black | 48.8 |  |
| `G1012A` | Panel Ground | VHF Comm2 (GNC 355 Comm) | 20 | Black | 52.4 |  |

## L — Lighting

| Wire Label | From | To | Gauge (AWG) | Color | Length (in) | Notes |
|------------|------|----|:-----------:|-------|------------:|-------|
| `L10A` | Main Bus | LANDING LIGHT TAXI Switch | 18 | White | 65.4 |  |
| `L10B` | Landing Light | LANDING LIGHT TAXI Switch | 18 | White | 78.6 |  |
| `L10C` | Taxi Light | LANDING LIGHT TAXI Switch | 18 | White | 76.0 |  |
| `L20A` | Main Bus | NAV+STRB Switch | 16 | White | 64.4 |  |
| `L20B` | Nav/Strobe Light, Right (Blaze 1R) | Firewall Ground | 16 | White | 247.9 |  |
| `L20C` | Nav/Strobe Light, Left (Blaze 1G) | Firewall Ground | 16 | White | 242.1 |  |
| `L21A` | Nav/Strobe Light, Right (Blaze 1R) | Nav/Strobe Light, Left (Blaze 1G) | 14 | White | 361.6 |  |
| `L30A` | Main Bus | NAV+STRB Switch | 16 | White | 64.4 |  |
| `L30B` | Nav/Strobe Light, Right (Blaze 1R) | NAV+STRB Switch | 16 | White | 322.1 |  |
| `L30C` | Nav/Strobe Light, Left (Blaze 1G) | NAV+STRB Switch | 16 | White | 321.5 |  |
| `L40A` | USB Charger (GSB 15) | Main Bus | 22 | White | 77.5 |  |
| `L50A` | Battery Bus | Lighting Controller | 22 | White | 123.4 |  |
| `L52A` | Lighting Controller | Interior Light Dimmer | 22 | White | 25.8 |  |
| `L53A` | Lighting Controller | Interior Light Dimmer | 22 | White | 25.8 |  |
| `L54A` | Interior Light, Aft | Lighting Controller | 20 | White | 124.0 |  |
| `L55A` | Interior Light, Forward | Lighting Controller | 20 | White | 54.0 |  |
| `L99A` | LANDING LIGHT TAXI Switch | LANDING LIGHT TAXI Switch | — | White | 24.0 |  |

## M — Miscellaneous Electrical

| Wire Label | From | To | Gauge (AWG) | Color | Length (in) | Notes |
|------------|------|----|:-----------:|-------|------------:|-------|
| `M10A` | Canopy Switch | Battery Bus | 18 | Yellow | 113.8 |  |
| `M10B` | Canopy Switch | Canopy Actuator | 18 | Yellow | 92.0 |  |
| `M11A` | Canopy Switch | Canopy Actuator | 18 | Yellow | 92.0 |  |
| `M20A` | Main Bus | Fuel Boost Switch | 18 | Yellow | 66.5 |  |
| `M20B` | Fuel Boost Switch | Fuel Boost Pump | 18 | Yellow | 124.6 | 22AWG |
| `M21A` | Electric Primer Valve | Fuel Boost Switch | 18 | Yellow | 126.0 | 22AWG |
| `M30A` | Main Bus | Lnd Brake Switch | 18 | Yellow | 50.2 |  |
| `M30B` | Auto Retract | Lnd Brake Switch | 18 | Yellow | 25.9 |  |
| `M30C` | Landing Brake Actuator | Auto Retract | 18 | Yellow | 70.8 |  |
| `M31A` | Landing Brake Actuator | Lnd Brake Switch | 18 | Yellow | 69.5 |  |
| `M40A` | Main Bus | Nose Gear Switch | 18 | Yellow | 51.2 |  |
| `M40B` | Nose Gear Switch | Nose Gear Actuator | 18 | Yellow | 41.4 |  |
| `M41A` | Nose Gear Switch | Nose Gear Actuator | 18 | Yellow | 41.4 |  |
| `M50A` | Heater Switch | Main Bus | 18 | Yellow | 76.5 |  |
| `M50B` | Heater Switch | Seat Heater | 18 | Yellow | 85.0 |  |
| `M60A` | Main Bus | Pitot Heat | 18 | Yellow | 65.6 |  |
| `M60B` | Pitot Heat | Pitot Probe | 18 | Yellow | 78.8 |  |
| `M71A` | Main Bus | AP SERVOS Switch | 20 | Yellow | 51.2 |  |
| `M71B` | AP Servo Breaker (3A) | AP SERVOS Switch | 20 | Yellow | 43.1 |  |
| `M71C` | Roll Servo (GSA 28) | AP Servo Breaker (3A) | 20 | Yellow | 221.7 |  |
| `M72A` | Main Bus | AP SERVOS Switch | 22 | Yellow | 51.2 |  |
| `M72B` | AP Servo Breaker (3A) | AP SERVOS Switch | 22 | Yellow | 44.1 |  |
| `M72C` | Pitch Servo (GSA 28) | AP Servo Breaker (3A) | 22 | Yellow | 58.9 |  |
| `M80A` | Main Bus | Panel Fan | 24 | Yellow | 60.0 |  |
| `M99A` | Main Bus | Fuel Boost Switch | — | Yellow | 66.5 |  |

## P — DC Power

| Wire Label | From | To | Gauge (AWG) | Color | Length (in) | Notes |
|------------|------|----|:-----------:|-------|------------:|-------|
| `P10A` | Battery Contactor | Main Battery (ETX900-VNT) | 24 | Red | 38.1 | 4AWG |
| `P11A` | Battery Contactor | Battery Contactor | 24 | Red | 24.0 |  |
| `P13A` | Main Bus | Diode | — | Red | 40.9 | 4AWG > 6in |
| `P14A` | Battery Bus | Battery Contactor | 24 | Red | 50.0 | 14 AWG (>6 in) |
| `P20A` | Fuselink | Diode | 20 | Red | 40.0 | 4AWG > 6in |
| `P20B` | Fuselink | ALT FLD Breaker (5A) | 20 | Red | 68.8 | 18AWG |
| `P20D` | BATT/ALT DC POWER Switch | Voltage Regulator (LRE1B-14) | 20 | Red | 124.1 | 20AWG |
| `P22A` | Alt LED | Voltage Regulator (LRE1B-14) | 20 | Red | 25.0 |  |
| `P22B` | Alt LED | Voltage Regulator (LRE1B-14) | 20 | Red | 25.0 |  |
| `P22C` | Inline Fuse (IFH-2) | Voltage Regulator (LRE1B-14) | 20 | Red | 25.0 |  |
| `P22D` | Battery Contactor | Inline Fuse (IFH-2) | 20 | Red | 38.4 | 4AWG > 6in |
| `P23A` | Alternator (Main) | Voltage Regulator (LRE1B-14) | 22 | Red | 96.8 | 20AWG |
| `P24A` | Alternator (Main) | Main Alt Shunt | 24 | Red | 89.9 | 4AWG |
| `P24B` | Main Alt Shunt | ANL Current Limiter (60A) | 24 | Red | 25.1 | 4AWG |
| `P24C` | Starter Contactor | ANL Current Limiter (60A) | 24 | Red | 32.8 | > 6in 4AWG |
| `P30A` | Battery Contactor | Inline Fuse (IFH-2) | 24 | Red | 33.4 | 14 AWG (>6 in) |
| `P30B` | Engine Shunt | Inline Fuse (IFH-2) | 24 | Red | 26.0 | 14AWG |
| `P30C` | Voltage Regulator (PMR1D) | Engine Shunt | 24 | Red | 41.5 |  |
| `P31A` | Voltage Regulator (PMR1D) | Alternator (Alt) | 18 | Red | 54.9 |  |
| `P32A` | Voltage Regulator (PMR1D) | Alternator (Alt) | 18 | Red | 54.9 |  |
| `P33A` | Voltage Regulator (PMR1D) | Aux Alt Off/On Switch | — | Red | 110.8 |  |
| `P34A` | Filter Capacitor | Voltage Regulator (PMR1D) | — | Red | 25.0 |  |
| `P51A` | Battery Bus | Brownout Battery Relay | 16 | Red | 141.3 |  |
| `P51B` | Brownout Battery Relay | Brownout Battery (EXT104/EBBS) | 16 | Red | 35.8 | 14AWG |
| `P52A` | Inline Fuse (IFH-2) | Brownout Battery (EXT104/EBBS) | 16 | Red | 33.3 |  |
| `P52B` | Endurance Bus Relay | Inline Fuse (IFH-2) | 16 | Red | 25.3 |  |
| `P52C` | Endurance Bus Relay | Endurance Bus | 16 | Red | 29.5 | 14AWG |
| `P53A` | Endurance Bus Relay | Endurance Bus Relay | — | Red | 24.0 |  |
| `P53B` | Endurance Bus Relay | E-Bus Alt Feed Switch | — | Red | 57.2 | 22AWG |
| `P54A` | Main Bus | Diode | — | Red | 40.9 | 4AWG > 6in |
| `P54B` | Diode | Endurance Bus | — | Red | 24.6 | 20AWG >6 IN |
| `P55A` | Low Voltage Monitor Module | Endurance Bus | 24 | Red | 65.0 | 20AWG |
| `P56A` | BATT/ALT DC POWER Switch | ALT FLD Breaker (5A) | — | Red | 37.1 | 20AWG 22AWG |
| `P57A` | LV EBUS Warning LED | Low Voltage Monitor Module | 24 | Red | 25.4 | 22AWG |
| `P61B` | Battery Contactor | Ground Power Contactor | 24 | Red | 29.0 | 4AWG |
| `P62A` | Ground Receptacle | Ground Power Contactor | — | Red | 66.6 | 4AWG |
| `P62B` | Diode | Ground Power Contactor | — | Red | 24.8 |  |
| `P62C` | Ground Power Switch Breaker (2A) | Crowbar Overvoltage Module | — | Red | 141.7 |  |
| `P63A` | Crowbar Overvoltage Module | Ground Power Contactor | — | Red | 25.0 |  |
| `P64A` | Crowbar Overvoltage Module | Ground Power Contactor | — | Red | 25.0 |  |
| `P99A` | Diode | Battery Contactor | 6 | Red | 24.0 |  |
| `P99B` | Diode | Battery Contactor | 6 | Red | 24.0 |  |
| `P99C` | Starter Contactor | Starter (BCS206-149-12) | 6 | Red | 85.6 | 4AWG |
