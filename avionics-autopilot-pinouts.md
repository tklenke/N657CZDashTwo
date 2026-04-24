# Autopilot Connector Pinouts (GMC 507 / GSA 28)

::: pending
**PENDING** — 2026-04-23
:::

Connector pinout data from G3XInstallationManual_RevAZ.pdf, Sections 23.9 (GMC 507) and 23.13 (GSA 28).

## J7001 — GMC 507 Mode Controller (DE15)

| Pin | Function | I/O |
|----:|----------|:---:|
| 1 | UNIT ID 1 | In |
| 2 | UNIT ID 2 | In |
| 3 | CAN HI | I/O |
| 4 | CAN LO | I/O |
| 5 | RESERVED | — |
| 6 | CAN BUS TERM 2 | — |
| 7 | AIRCRAFT POWER 1 | In |
| 8 | CAN BUS TERM 1 | — |
| 9 | AIRCRAFT POWER 2 | In |
| 10 | TO/GA DISCRETE IN | In |
| 11 | LIGHTING BUS HI | In |
| 12 | RESERVED | — |
| 13 | RESERVED | — |
| 14 | RESERVED | — |
| 15 | POWER GROUND | — |

## J281P / J281R — GSA 28 Servos (DA15)

Pitch servo uses J281P; roll servo uses J281R. Both share the same pinout.

| Pin | Function | I/O |
|----:|----------|:---:|
| 1 | CAN_H | I/O |
| 2 | CAN_L | I/O |
| 3 | CAN_TERM_1 | — |
| 4 | CAN_TERM_2 | — |
| 5 | ID_STRAP_1 | In |
| 6 | ID_STRAP_2 | In |
| 7 | ID_STRAP_3 / RS-232 TX (Roll only) | In |
| 8 | ID_STRAP_4 / RS-232 RX (Roll only) | In |
| 9 | AIRCRAFT GROUND | — |
| 10 | AIRCRAFT POWER | In |
| 11 | TRIM_IN_1 | In |
| 12 | TRIM_IN_2 | In |
| 13 | TRIM_OUT_1 | Out |
| 14 | TRIM_OUT_2 | Out |
| 15 | CWS/DISCONNECT | In |
