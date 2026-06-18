# SS 638 Part 4 Chapter 41 — Protection Against Electric Shock (Detail)

## Table 41.1 — Maximum Disconnection Times

| System | 50V < U₀ ≤ 120V (a.c./d.c.) | 120V < U₀ ≤ 230V (a.c./d.c.) | 230V < U₀ ≤ 400V (a.c./d.c.) | U₀ > 400V (a.c./d.c.) |
|---|---|---|---|---|
| TN-S | 0.8 s / (note) | 0.4 s / 5 s | 0.2 s / 0.4 s | 0.1 s / 0.1 s |
| TT | 0.3 s / (note) | 0.2 s / 0.4 s | 0.07 s / 0.2 s | 0.04 s / 0.1 s |

Note: For d.c. with TN-S at 50–120V, disconnection not required for electric shock protection.
U₀ = nominal a.c. rms or d.c. line voltage to earth.

---

## Table 41.2 — Max Zs for Fuses at 0.4 s, U₀ = 230 V (TN-S, final circuits ≤32 A)

**gG/gM fuses to IEC 60269-2 (systems E and G):**
| Rating (A) | 6 | 10 | 16 | 20 | 25 | 32 |
|---|---|---|---|---|---|---|
| Zs (Ω) | 8.21 | 4.89 | 2.56 | 1.77 | 1.35 | 1.04 |

**Fuses to SS 167:**
| Rating (A) | 3 | 13 |
|---|---|---|
| Zs (Ω) | 16.4 | 2.42 |

---

## Table 41.3L — Max Zs for Circuit-Breakers at 0.4 s / 5 s, U₀ = 230 V

**Type B (IEC 60898-1):** Formula = 46/In
| Rating (A) | 6 | 10 | 16 | 20 | 25 | 32 | 40 | 50 | 63 |
|---|---|---|---|---|---|---|---|---|---|
| Zs (Ω) | 7.67 | 4.60 | 2.87 | 2.30 | 1.84 | 1.44 | 1.15 | 0.92 | 0.73 |

**Type C (IEC 60898-1):** Formula = 23/In
| Rating (A) | 6 | 10 | 16 | 20 | 25 | 32 | 40 | 50 | 63 |
|---|---|---|---|---|---|---|---|---|---|
| Zs (Ω) | 3.83 | 2.30 | 1.44 | 1.15 | 0.92 | 0.72 | 0.57 | 0.46 | 0.36 |

**Type D (IEC 60898-1):** Formula = 11.5/In
| Rating (A) | 6 | 10 | 16 | 20 | 25 | 32 | 40 | 50 | 63 |
|---|---|---|---|---|---|---|---|---|---|
| Zs (Ω) | 1.92 | 1.15 | 0.72 | 0.57 | 0.46 | 0.36 | 0.29 | 0.23 | 0.18 |

> All Zs values at operating temperature. Adjust for conductor temperature if testing at different temp — see Appendix 14(L).

---

## Table 41.5 — Max Zs for Non-Delayed RCDs (SS 97 / SS 480), U₀ = 230 V

| Rated residual operating current (mA) | Max Zs (Ω) |
|---|---|
| 30 | 1667* |
| 100 | 500* |
| 300 | 167 |
| 500 | 100 |

*Earth electrode resistance should be ≤200 Ω for reliable performance (cl. 542.2.4).

---

## Table 41.4 — Max Zs for Fuses at 5 s, U₀ = 230 V (Distribution circuits, TN-S)

**gG/gM fuses to IEC 60269-2:**
| Rating (A) | 6 | 10 | 16 | 20 | 25 | 32 | 40 | 50 | 63 | 80 | 100 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Zs (Ω) | 12.8 | 7.19 | 4.18 | 2.95 | 2.30 | 1.84 | 1.35 | 1.04 | 0.82 | 0.57 | 0.46 |

**Fuses to SS 167:**
| Rating (A) | 3 | 13 |
|---|---|---|
| Zs (Ω) | 23.2 | 3.83 |

---

## Protective Measure: SELV and PELV (Section 414)

**SELV (Separated Extra-Low Voltage):**
- Electrically separated from earth AND from other circuits
- Nominal voltage: ≤50 V a.c. / ≤120 V d.c.
- Sources (cl. 414.3L): safety isolating transformer (IEC 61558-2-6), motor-generator with isolation, electrochemical source (battery), electronic power supply certified to appropriate standard

**PELV (Protective Extra-Low Voltage):**
- Same voltage limits as SELV
- NOT electrically separated from earth; connected to earth or PE

**FELV (Functional ELV — cl. 411.7):**
- ELV used for functional reasons but NOT fully meeting SELV/PELV criteria
- Requires supplementary protective provisions:
  - Basic protection: basic insulation rated for primary circuit voltage, OR barriers/enclosures
  - Fault protection: exposed-conductive-parts connected to primary circuit PE conductor
  - Source must have at least simple separation between windings

**SELV/PELV circuit requirements (cl. 414.4):**
- Socket-outlets / connectors must not be intermateable with other voltage systems
- SELV circuits: no protective conductor, no connection to earth
- PELV circuits: protective conductor and/or connection to earth
- Wiring must be physically separated from other circuits OR insulated for higher voltage

---

## Reduced Low Voltage Systems (cl. 411.8)

Nominal voltage: ≤110 V a.c. line-to-line  
- Single-phase: 55 V to earthed midpoint
- Three-phase: 63.5 V to earthed neutral

Used where ELV impractical but shock risk reduction needed (e.g. construction sites, portable tools outdoors).

Max disconnection time: 5 s  
Fault protection: overcurrent device or RCD; all exposed-conductive-parts earthed.

---

## Additional Protection Notes

**RCD discrimination (cl. 531.2.9L):**
Where RCDs are in series, selectivity shall be achieved. Upstream RCD should have time delay or higher rated current (S-type or G-type). At least 3:1 ratio in rated current recommended.

**Equipotential bonding — supplementary (cl. 415.2):**
Required when disconnection time cannot be met. Resistance between simultaneously accessible parts:
- R ≤ 50 V / Ia (for a.c. systems)
- R ≤ 120 V / Ia (for d.c. systems)
