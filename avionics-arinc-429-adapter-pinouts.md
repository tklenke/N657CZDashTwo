# ARINC 429 Adapter Connector Pinouts (GAD 29)

::: pending
**PENDING** — 2026-04-23
:::

Connector pinout data from G3XInstallationManual_RevAZ.pdf, Section 23.2. Harness connectors P291 and P292 mate to unit connectors J291 and J292 respectively.

## J291 — 9-pin D-sub

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

## J292 — 25-pin D-sub

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
