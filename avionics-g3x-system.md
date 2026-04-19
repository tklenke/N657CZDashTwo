# G3X System Overview

## Description

The Garmin G3X Touch is an integrated avionics suite providing primary flight display, engine monitoring, GPS navigation, communication, and autopilot functions. All G3X line-replaceable units (LRUs) draw power from the dedicated G3X bus. See [[Bus Architecture|electrical-bus-architecture]] in Section 16 for bus and circuit protection details.

Most LRUs are located in the avionics bay forward of the instrument panel (IP). Exceptions: the GEA 24 mounts on the forward face of the firewall, the GMU 11 mounts in the right strake, and the GSA 28 autopilot servos mount in the right fuselage (pitch servo) and under the cowling on the strake (roll servo).

## System Components

- [[ADAHRS (GSU 25C)|avionics-adahrs]] — air data, attitude, and heading reference system
- [[Antenna System|avionics-antennas]] — embedded copper foil and external antennas
- [[Audio Panel (GMA 245R)|avionics-audio-panel]] — audio switching and intercom
- [[Autopilot|avionics-autopilot]] — GMC 507 mode controller and GSA 28 servos (×2)
- [[Engine Data Acquisition (GEA 24)|avionics-engine-data-acquisition]] — engine and systems monitoring
- [[G5 Backup Instrument|avionics-g5-backup-instrument]] — standby attitude and airspeed display (×2)
- [[GDU 460 PFD|avionics-gdu-460-pfd]] — primary flight display touchscreen
- [[GPS and Navigation (GNC 355)|avionics-gps-and-navigation]] — IFR GPS navigator
- [[Magnetometer (GMU 11)|avionics-magnetometer]] — remote magnetometer for heading reference
- [[Transponder and ADS-B (GTX 45R)|avionics-transponder-adsb]] — Mode S transponder with ADS-B In/Out
- [[VHF Communication (GTR 20)|avionics-vhf-communication]] — VHF comm radios (×2)

## System Interconnect Diagram

The diagram below shows the data bus and electrical interconnections between G3X LRUs.

<img src="/assets/diagrams/sec17-g3x-system-interconnect.svg" style="width:100%" alt="G3X System Interconnect">

## Operation

The GDU 460 is the central display and configuration interface for the suite. The GSU 25C provides air data (airspeed, altitude, vertical speed) and attitude and heading reference to the GDU 460. The GMU 11 supplies magnetometer data to the GSU 25C for heading reference. The GEA 24 acquires engine and system sensor data and forwards it to the GDU 460 for display.

The GPS 20A provides WAAS GPS position data to the GDU 460 and GNC 355. The GTX 45R transponder sends and receives ADS-B traffic and weather data, displayed on the GDU 460. The autopilot (GMC 507 and GSA 28 servos) receives flight director guidance from the GDU 460.

The G5 backup instruments operate on separate power from the main G3X bus. @@TOM: Confirm G5 power source — main bus or dedicated circuit?

## Inspection

System-level inspection is performed as part of the annual condition inspection. Individual component checks are on each component's page. At the system level, verify:

- All LRUs power on without fault or alert messages on the GDU 460
- GDU 460 self-test completes without alerts
- GSU 25C AHRS aligns within normal time on power-up @@TOM: alignment time limit — check G3X installation manual if needed
- Engine data is present and plausible on the GDU 460 after engine start
- No persistent system messages remain after normal power-on sequence
