# Nose Gear

## Description

The nose gear is a retractable, electrically actuated tricycle gear assembly mounted in the nose compartment forward of the F-22 bulkhead. The system consists of a Wilhelmson EZ Nose Lift electric actuator, a builder-fabricated fiberglass strut, a wheel and fork assembly, and a pair of spring-loaded doors that open on extension and close automatically on retraction.

> **NOTE:** N657CZ is at risk of tipping backward whenever the nose gear is extended and the front seat is unoccupied. See [[Nose Gear Tipping Hazard|landing-gear-nose-gear-tipping]] before performing any work with the nose gear extended.

## System Components

- [[Nose Gear Actuator|landing-gear-nose-gear-actuator]] — Wilhelmson EZ Nose Lift electric linear actuator with Zeitlin clamp modification. Controls extension and retraction.
- **Nose gear strut** — Builder-fabricated fiberglass strut. Connects the actuator extension shaft to the wheel fork.
- **Upper pivot** — Pivot fitting at the fuselage attachment point. @@TOM: document fitting type and hardware.
- **Lower pivot** — Pivot fitting connecting the strut to the wheel fork. @@TOM: document fitting type and hardware.
- **Wheel and fork assembly** — Nose wheel, tire, axle, and fork. @@TOM: document wheel and tire specifications.
- **Nose gear doors** — Two doors that close the gear well when the gear is retracted. Spring-loaded closed; opened by gear leg travel during extension.

## Operation

The cockpit control is SW10, a momentary (ON)-OFF-(ON) switch on the instrument panel. Holding the switch toward extend drives the actuator to push the strut down; holding it toward retract drives the actuator to pull the strut up. The actuator stops automatically at each end of travel via internal limit switches.

**Extension sequence:** SW10 held to extend → actuator extends → strut and gear leg descend → gear leg or cam pushes nose gear doors open → gear reaches full extension → actuator stops.

**Retraction sequence:** SW10 held to retract → actuator retracts → strut and gear leg rise → tension springs pull nose gear doors closed → gear reaches full retraction → actuator stops.

**Manual extension:** A manual extension rod runs from the instrument panel to the actuator. Insert a 1/4" drive socket wrench into the socket on the IP end and turn to extend or retract the gear manually. @@TOM: confirm clockwise/counterclockwise direction for extend and retract. See [[Nose Gear Actuator|landing-gear-nose-gear-actuator]] for full manual extension procedure.

## Nose Gear Doors

The nose gear doors are spring-loaded closed using tension springs (screen door type) attached between each door and a fixed structural point inside the nose compartment. When the gear extends, the gear leg or a cam pushes the doors open against the spring force. When the gear retracts, the springs pull the doors closed.

@@TOM: Verify door spring specifications and attachment details for N657CZ. Builder notes indicate springs are typically 5/16"–3/8" diameter, approximately 6" unstretched length, 0.045–0.050" wire gauge, approximately 3–7 lb/in spring rate. Hardware sources include Century Spring, Lee Spring, or equivalent screen door extension springs.

If a door spring fails, the door may remain open in flight, resulting in increased drag. This is not a flight hazard but should be corrected before the next flight.

> **NOTE:** Safety wire the spring attachment points to prevent a broken spring from becoming a loose object in the nose compartment.

## Inspection

### System Function Test

Perform at each condition inspection with the aircraft on jacks. See [[Jacking and Leveling|ground-handling-jacking-and-leveling]] in Section 5 and the functional test procedure on the [[Nose Gear Actuator|landing-gear-nose-gear-actuator]] page.

Verify:
- Gear extends and retracts smoothly with no unusual noise.
- Nose gear doors open fully on extension and close fully on retraction.
- Gear locks down securely before lowering aircraft off jacks. (AC 43.13, ch09_p005)

### Strut and Pivots

Inspect per AC 43.13 ch09_p005 for wear, looseness, and condition. (AC 43.13, ch09_p005)

- Inspect the fiberglass strut for cracks, delamination, or impact damage. Pay particular attention to the attachment area at the upper pivot where loads concentrate.
- Check the upper pivot fitting hardware for security and wear.
- Check the lower pivot fitting and fork for security, wear, and alignment.
- Inspect the strut for bending. A bent strut must be replaced.

### Nose Gear Doors

- Inspect both door springs for fatigue and condition. Pay particular attention to the end loops (90° bends), which are the typical failure point.
- Verify spring attachment points on the doors and structure are secure and undamaged.
- Verify safety wire is present at spring attachment points.
- Verify both doors close fully and are flush with the fuselage contour when the gear is retracted.
- Inspect door hinge hardware for security and wear.

### Wheel and Fork Assembly

@@TOM: Document wheel, tire, and bearing inspection criteria and intervals.

## Troubleshooting

| Symptom | Likely Cause | Action |
|---------|-------------|--------|
| Doors do not close fully on retraction | Weak or broken spring; spring anchor shifted | Inspect springs and attachment points; adjust or replace spring |
| Door closes but gap remains | Hinge geometry misaligned | Adjust hinge or anchor point position |
| Actuator does not stop at end of travel | Limit switch misadjusted | See [[Nose Gear Actuator|landing-gear-nose-gear-actuator]] — limit switch adjustment |
| Clicking from inside extension tube during operation | AN5-12A bolts contacting ball screw | Stop immediately; see [[Nose Gear Actuator|landing-gear-nose-gear-actuator]] |
| Gear extends/retracts slowly | Excess grease congealed (cold weather); low battery | Check lubrication; verify electrical system charge |
