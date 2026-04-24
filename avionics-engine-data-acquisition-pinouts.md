# Engine Data Acquisition Connector Pinouts (GEA 24)

::: pending
**PENDING** — 2026-04-23
:::

Connector pinout data from G3XInstallationManual_RevAZ.pdf, Section 23.4.

## J241 — DE9

| Pin | Function | I/O |
|----:|----------|:---:|
| 1 | CAN HI | I/O |
| 2 | CAN LO | I/O |
| 3 | RESERVED | — |
| 4 | RS-232 RX | In |
| 5 | RS-232 TX | Out |
| 6 | GROUND | — |
| 7 | AIRCRAFT POWER 1 | In |
| 8 | AIRCRAFT POWER 2 | In |
| 9 | GROUND | — |

## J242 — DB25

| Pin | Function | I/O |
|----:|----------|:---:|
| 1 | RESERVED | — |
| 2 | CHT6 LO / CHT 2 RESISTIVE LO / TEMP 4 LO | In |
| 3 | EGT6 LO / TEMP 6 LO | In |
| 4 | CHT5 LO / CHT 1 RESISTIVE LO / TEMP 3 LO | In |
| 5 | EGT5 LO / TEMP 5 LO | In |
| 6 | CHT4 LO | In |
| 7 | EGT4 LO | In |
| 8 | CHT3 LO | In |
| 9 | EGT3 LO | In |
| 10 | CHT2 LO | In |
| 11 | EGT2 LO | In |
| 12 | CHT1 LO | In |
| 13 | EGT1 LO | In |
| 14 | CHT6 HI / CHT 2 RESISTIVE HI / TEMP 4 HI | In |
| 15 | EGT6 HI / TEMP 6 HI | In |
| 16 | CHT5 HI / CHT 1 RESISTIVE HI / TEMP 3 HI | In |
| 17 | EGT5 HI / TEMP 5 HI | In |
| 18 | CHT4 HI | In |
| 19 | EGT4 HI | In |
| 20 | CHT3 HI | In |
| 21 | EGT3 HI | In |
| 22 | CHT2 HI | In |
| 23 | EGT2 HI | In |
| 24 | CHT1 HI | In |
| 25 | EGT1 HI | In |

## J243 — DB37

| Pin | Function | I/O |
|----:|----------|:---:|
| 1 | FUEL PRESS GND | — |
| 2 | FUEL PRESS | In |
| 3 | FUEL PRESS XDCR +12V | Out |
| 4 | FUEL PRESS XDCR +5V | Out |
| 5 | RPM XDCR GND 2 | — |
| 6 | RPM 2 | In |
| 7 | RPM XDCR GND 1 | — |
| 8 | RPM 1 | In |
| 9 | RPM XDCR +12V 1 | Out |
| 10 | RPM XDCR +12V 2 | Out |
| 11 | RESERVED / SPARE | — |
| 12 | MANIFOLD PRESS GND | — |
| 13 | MANIFOLD PRESS | In |
| 14 | MANIFOLD PRESS XDCR +12V | Out |
| 15 | MANIFOLD PRESS XDCR +5V | Out |
| 16 | OIL PRESS GND | — |
| 17 | OIL PRESS HI | In |
| 18 | OIL PRESS XDCR +12V | Out |
| 19 | OIL PRESS XDCR +5V | Out |
| 20 | FUEL XDCR GND 1 | — |
| 21 | FUEL RETURN | In |
| 22 | FUEL XDCR GND 2 | — |
| 23 | FUEL FLOW | In |
| 24 | FUEL XDCR +12V 1 | Out |
| 25 | FUEL XDCR +12V 2 | Out |
| 26 | GP +5V 1 | Out |
| 27 | GP GND 1 | — |
| 28 | GP 7 / TEMP 2 LO | In |
| 29 | GP 7 / TEMP 2 HI | In |
| 30 | GP 6 / TEMP 1 LO | In |
| 31 | GP 6 / TEMP 1 HI | In |
| 32 | OIL TEMP LO | In |
| 33 | OIL TEMP HI | In |
| 34 | SHUNT 2 LO | In |
| 35 | SHUNT 2 HI | In |
| 36 | SHUNT 1 LO | In |
| 37 | SHUNT 1 HI | In |

## J244 — DB50

| Pin | Function | I/O |
|----:|----------|:---:|
| 1 | SYSTEM ID 1A* | In |
| 2 | SYSTEM ID 1B / GND | — |
| 3 | RESERVED | — |
| 4 | RESERVED | — |
| 5 | FUEL QTY +5V 1 | Out |
| 6 | FUEL QTY 1 | In |
| 7 | FUEL QTY 1 GND | — |
| 8 | FUEL QTY +5V 2 | Out |
| 9 | FUEL QTY 2 | In |
| 10 | FUEL QTY 2 GND | — |
| 11 | GP 3 / FUEL QTY 3 HI / +5V 3 | Out |
| 12 | GP 3 / FUEL QTY 3 | In |
| 13 | GP 3 / FUEL QTY 3 LO / GND | — |
| 14 | GP 4 / FUEL QTY 4 HI / +5V 4 | Out |
| 15 | GP 4 / FUEL QTY 4 | In |
| 16 | GP 4 / FUEL QTY 4 LO / GND | — |
| 17 | FADEC CAN2 HI | I/O |
| 18 | GP 1 HI / +5V | Out |
| 19 | GP 1 | In |
| 20 | GP 1 LO / GND | — |
| 21 | GP 2 HI / +5V | Out |
| 22 | GP 2 | In |
| 23 | GP 2 LO / GND | — |
| 24 | GP +5V 2 | Out |
| 25 | VOLTS 1 | In |
| 26 | GP GND 2 | — |
| 27 | GP +5V 3 | Out |
| 28 | VOLTS 2 | In |
| 29 | GP GND 3 | — |
| 30 | GP HI / +5V | Out |
| 31 | GP 5 | In |
| 32 | GP 5 LO / GND | — |
| 33 | FADEC CAN2 LO | I/O |
| 34 | FUEL XDCR +12V 3 | Out |
| 35 | FUEL XDCR +12V 4 | Out |
| 36 | FUEL FLOW (shared J243-23) | In |
| 37 | FUEL RETURN (shared J243-21) | In |
| 38 | FUEL XDCR GND 3 | — |
| 39 | FUEL XDCR GND 4 | — |
| 40 | DISCRETE IN 1 | In |
| 41 | DISCRETE IN 2 | In |
| 42 | DISCRETE IN 3 | In |
| 43 | DISCRETE IN 4 | In |
| 44 | DISCRETE OUT 1 / MASTER WARNING | In |
| 45 | DISCRETE OUT 2 / MASTER CAUTION | In |
| 46 | SHUNT 2 HI (shared J243-35) | In |
| 47 | SHUNT 2 LO (shared J243-34) | In |
| 48 | FADEC CAN3 HI (GEA 24B only) | In |
| 49 | FADEC CAN3 LO (GEA 24B only) | In |
| 50 | GP +12V | Out |
