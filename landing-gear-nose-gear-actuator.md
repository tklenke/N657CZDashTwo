# Nose Gear Actuator

::: draft
**DRAFT** — Not yet reviewed.
:::

## Description

N657CZ uses a Wilhelmson EZ Nose Lift electric linear actuator to extend and retract the nose gear. The actuator is mounted in the nose compartment between the NG-30 mounting plates. An internal ball screw driven by an electric motor extends and retracts the nose gear strut via a lower extension shaft attached to the NG-3/NG-4 fitting on the strut.

The cockpit control is SW10, a momentary (ON)-OFF-(ON) switch (S700-1-7, 20A rated) on the instrument panel. Holding the switch toward extend drives the gear down; holding it toward retract drives the gear up. The actuator stops automatically at each end of travel via internal limit switches.

The Marc Zeitlin EZNoselift Clamp System (Revision 5, February 2024) is installed. The clamp addresses a known failure mode of the original Wilhelmson design: the side-clamp bolts that secure the actuator to the mounting plates are loaded in tension and can loosen over time due to vibration, eventually allowing the pins to walk out and the actuator to separate from the mounting plates. The Zeitlin clamp encircles the upper actuator tube and transfers load to shear pins rather than the original bolts, eliminating the tensile loading. (EZNoselift_Clamp_Install_R5.pdf)

## Specifications

| Item | Value | Source |
|------|-------|--------|
| Actuator type | Linear (ball screw, electric motor) | Engineering report |
| Nominal current | 9.9 A | Engineering report |
| Control switch | SW10, S700-1-7, (ON)-OFF-(ON) momentary | Engineering report |
| Switch rating | 20 A | Engineering report |
| Control wiring | 18 AWG M22759/16 | Engineering report |
| Actuator part number | @@TOM: confirm with Wilhelmson documentation | — |

**Zeitlin clamp hardware (as installed):**

| Qty | Part | Location |
|-----|------|----------|
| 2 | Clamp halves (aluminum) | Upper actuator tube |
| 4 | AN4-21A bolts | Clamp halves |
| 8 | AN960-416L washers | Under bolt heads and nuts |
| 4 | MS21042-4 nuts | Clamp bolts |
| 2 | Shear pins | Through clamp and actuator tube |
| 2 | AN5-12A (or AN5H-12A) bolts | Through shear pins into actuator |
| 2 | Nordlock NL8sp washers | Under shear pin bolts |

(EZNoselift_Clamp_Install_R5.pdf)

## Inspection

### Clamp Hardware

Inspect the Zeitlin clamp at each condition inspection. (EZNoselift_Clamp_Install_R5.pdf)

- Verify both shear pins are present and seated fully in the clamp square holes and actuator tube round holes.
- Check all four AN4-21A clamp bolts and nuts for security. Required torque: 50 in-lb. (EZNoselift_Clamp_Install_R5.pdf)
- Check both AN5-12A shear pin bolts for security. Required torque: 90 in-lb. (EZNoselift_Clamp_Install_R5.pdf)
- Verify Nordlock washers are present under the shear pin bolt heads.
- Check for fretting, corrosion, or wear at the clamp-to-tube contact surfaces.

### Actuating Mechanism

Inspect per AC 43.13 ch09_p005 for wear, looseness in joints, and smooth operation. (AC 43.13, ch09_p005)

- Check the lower extension shaft attachment bolt (AN4 through NG-3/NG-4) for security.
- Check the actuator mounting in the NG-30 plates — verify the actuator rotates freely on the shear pins with no binding. If binding is present, remove and investigate before returning to service.
- Inspect the extension shaft for bending, nicks, or corrosion.
- Check the P1 electrical connector for security and corrosion.
- Inspect wiring for chafing or damage.

### Limit Switches

@@TOM: Describe limit switch locations and adjustment procedure. (Wilhelmson documentation unavailable — verify with manufacturer before adjusting.)

The down limit switch must stop actuator travel before the internal clutch engages. Improper adjustment results in the motor running against the clutch at end of stroke. Signs of misadjustment include the actuator running longer than expected before stopping and unusual clutch noise.

### Lubrication

Apply a light coating of grease to the outer diameter of the shear pins during any removal and reinstallation. (EZNoselift_Clamp_Install_R5.pdf)

@@TOM: Lubrication specification and interval for the ball screw mechanism. (Wilhelmson documentation unavailable.) Use only grease approved by the actuator manufacturer; do not mix grease types. (AC 43.13, ch09_p003)

> **NOTE:** During winter operation, excess grease on the ball screw can congeal and increase loads on the actuator motor, leading to slow or failed operation. Keep lubrication moderate and verify smooth operation after cold-weather storage. (AC 43.13, ch09_p003)

## Procedures

### Functional Test (Aircraft on Jacks)

Perform this test after any work on the actuator, limit switches, or clamp hardware, and as part of the annual condition inspection. Aircraft must be on jacks with main gear clear of the ground. See [[Jacking and Leveling|ground-handling-jacking-and-leveling]] in Section 5.

1. Position the aircraft on jacks per [[Jacking and Leveling|ground-handling-jacking-and-leveling]].
2. Verify the nose gear is in the extended (down) position.
3. Hold SW10 toward retract. Observe the nose gear retract smoothly. The actuator should stop automatically at the full-up position.
4. Listen for any clicking or grinding sounds during retraction. A clicking sound from inside the extension tube indicates the AN5-12A shear pin bolts are contacting the ball screw. If heard, stop immediately and do not operate the system until the interference is resolved. (EZNoselift_Clamp_Install_R5.pdf)
5. Hold SW10 toward extend. Observe the nose gear extend smoothly and lock down.
6. Verify the nose gear is secure in the down-and-locked position before lowering the aircraft off jacks.

### Manual Extension

A manual extension rod runs from the instrument panel to the actuator. The IP end of the rod is fitted with a 1/4" drive socket.

1. Locate the manual extension rod socket on the instrument panel.
2. Insert a 1/4" drive socket wrench into the socket.
3. Turn the rod to extend or retract the nose gear. @@TOM: Confirm clockwise/counterclockwise direction for extend and retract.

### Removal and Installation

@@TOM: Document removal and installation procedure. (Wilhelmson documentation unavailable. Reference EZNoselift_Clamp_Install_R5.pdf for clamp disassembly and reinstallation — see steps 1–15 for the full clamp reinstallation sequence.)
