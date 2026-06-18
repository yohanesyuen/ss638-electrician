# SS 638 Appendix 4(L) — Cable Current-Carrying Capacity and Voltage Drop

> Appendix 4(L) is **informative** (advisory), but the methodology it describes is the industry-standard approach for cable sizing under SS 638.

---

## Cable Sizing Methodology (Section 6)

The sizing procedure determines the required **tabulated current-carrying capacity (It)** from the tables, then selects the cable size with It ≥ required value.

### Key symbols

| Symbol | Meaning |
|---|---|
| Ib | Design current of circuit (A) |
| In | Rated current of protective device (A) |
| It | Tabulated current-carrying capacity (A) — single circuit, 30°C ambient |
| Iz | Actual current-carrying capacity under installed conditions (A) = It × Ca × Cg × Ci |
| I₂ | Operating current of protective device (fusing/tripping current) |
| Ca | Correction factor for ambient temperature |
| Cg | Correction factor for grouping/bunching |
| Ci | Correction factor for thermal insulation |
| Ct | Correction factor for conductor operating temperature (voltage drop only) |

### Coordination rule (cl. 433.1.1)
```
Ib ≤ In ≤ Iz
I₂ ≤ 1.45 × Iz
```

### Step-by-step sizing (for IEC 60898 CB or IEC 60269 fuse)

1. Determine **Ib** (design current)
2. Select **In** ≥ Ib (next standard size up)
3. Determine applicable correction factors: Ca, Cg, Ci
4. Calculate required tabulated value:
   ```
   It ≥ In / (Ca × Cg × Ci)
   ```
5. Look up cable size in appropriate Table 4D/4E/4F/etc. (by installation method reference)
6. Check voltage drop (see below)

**For BS 3036 semi-enclosed (rewirable) fuses only:** add an extra divisor of 0.725:
```
It ≥ In / (0.725 × Ca × Ci)    [single circuit]
It ≥ In / (0.725 × Cg)          [grouped]
```

**Where overload protection NOT required (cl. 433.3):**
```
It ≥ Ib / (Ca × Cg × Ci)
```

---

## Correction Factor Ca — Ambient Temperature (Table 4C1)

Reference ambient temperature = **30°C** (air) / **20°C** (ground-buried cables).

**For 70°C thermoplastic cables (PVC):**

| Ambient Temp (°C) | Ca |
|---|---|
| 25 | 1.03 |
| 30 | 1.00 |
| 35 | 0.94 |
| 40 | 0.87 |
| 45 | 0.79 |
| 50 | 0.71 |
| 55 | 0.61 |
| 60 | 0.50 |

**For 90°C thermosetting cables (XLPE/LSF):**

| Ambient Temp (°C) | Ca |
|---|---|
| 25 | 1.02 |
| 30 | 1.00 |
| 35 | 0.96 |
| 40 | 0.91 |
| 45 | 0.87 |
| 50 | 0.82 |
| 55 | 0.76 |
| 60 | 0.71 |
| 65 | 0.65 |
| 70 | 0.58 |

> Singapore context: Typical indoor ambient = 30–35°C. Cable routes near boilers, plant rooms, or in direct sunlight may reach 45–50°C.

**For BS 3036 semi-enclosed fuses, use Table 4C2** (slightly different values due to 160°C final temp rather than 115°C for 70°C PVC grouped).

---

## Correction Factor Cg — Grouping (Tables 4B1, 4B2)

**Table 4B1: Cables clipped direct, on trays, ladders (touching):**

| No. of circuits/cables | Cg |
|---|---|
| 1 | 1.00 |
| 2 | 0.80 |
| 3 | 0.70 |
| 4 | 0.65 |
| 5 | 0.60 |
| 6 | 0.57 |
| 7 | 0.54 |
| 8 | 0.52 |
| 9 | 0.50 |
| 10–12 | 0.48 |
| 13–16 | 0.45 |
| 17–20 | 0.43 |
| >20 | 0.41 |

**Table 4B2: Enclosed in conduit/trunking/ducting (single layer):**

| No. of circuits | Cg |
|---|---|
| 1 | 1.00 |
| 2 | 0.80 |
| 3 | 0.70 |
| 4 | 0.65 |
| 5 | 0.60 |
| 6 | 0.57 |
| 7–9 | 0.50 |
| 10–12 | 0.45 |
| 13–16 | 0.41 |
| 17–20 | 0.38 |
| >20 | 0.35 |

> **Note:** A circuit that carries ≤30% of its grouped current-carrying capacity may be ignored when counting circuits for grouping (cl. 523.5L).

---

## Correction Factor Ci — Thermal Insulation

| Installation condition | Ci |
|---|---|
| Cable surrounded in thermal insulation — total enclosure, no air gap | **0.5** |
| Cable in contact with thermal insulation on one side (e.g. touching rockwool in wall) | 0.75 |
| No thermal insulation contact | 1.0 |

These apply to cables passing through or installed in contact with thermal insulation materials (mineral wool, foam board, etc.).

---

## Harmonic Current Rating Factor (Table 4 in Appendix 4(L))

For 4-core and 5-core cables carrying 3rd harmonic currents:

| 3rd harmonic content of line current | Size based on line current | Size based on neutral current |
|---|---|---|
| 0–15% | 1.00 | — |
| >15–33% | 0.86 | — |
| >33–45% | — | 0.86 |
| >45% | — | 1.00 |

When neutral current > line current, size cable on neutral current. If neutral current > 135% of line current and sized on neutral, no derating needed on line conductors.

---

## Voltage Drop (Appendix 12(L) — Normative; Section 7 of Appendix 4(L))

### Limits (Appendix 12(L)):
- Lighting circuits: **3%** of nominal voltage
- All other circuits: **5%** of nominal voltage

From origin of installation to the furthest point of utilisation.

### Calculation:
```
Voltage drop (V) = (mV/A/m) × Ib × L / 1000
```

Where:
- mV/A/m = millivolts per ampere per metre from Appendix 4(L) tables (at 70°C or 90°C conductor temp)
- Ib = design current (A)
- L = circuit length (m) — **one-way** for single-phase (cable tables give both-way equivalent); check table footnotes

### Temperature correction of mV/A/m (Ct factor, Section 7.1):

When conductor is not at rated operating temperature, the resistive component of voltage drop changes:
```
Ct = [230 + tp - (Ca²Cg² - Ib²/It²)(tp - 30)] / (230 + tp)
```
Where tp = max conductor operating temperature (70 or 90°C).

For ≤16 mm²: design mV/A/m = Ct × tabulated mV/A/m × cos φ (power factor)
For >16 mm²: design mV/A/m = Ct × cos φ × (mV/A/m)r + sin φ × (mV/A/m)x

> For most practical purposes (≤16 mm², cos φ ≈ 0.8–1.0, temperature near rated), tabulated mV/A/m values can be used directly with a small safety margin.

---

## Installation Methods (Table 4A Reference Methods)

Key reference methods and corresponding current-carrying capacity tables:

| Ref Method | Description | Tables |
|---|---|---|
| A | Enclosed in conduit in thermally insulating wall | 4D1, 4E1 |
| B | Enclosed in conduit on wall or in trunking | 4D1, 4E1 |
| C | Clipped direct to non-metallic surface | 4D2, 4E2 |
| D | In ducts in ground | 4D3, 4E3 |
| E | In free air (single cable, touching surface) | 4D4, 4E4 |
| F | In free air (single cable, spaced from surface) | 4D4, 4E4 |
| 11 | On perforated cable tray (touching) | 4E4 (90°C armoured) |
| 12 | On unperforated cable tray | Use Ref C or E |
| 13 | On cable ladder | 4E4 |

**Most common in Singapore buildings:**
- Method B: conduit on surface / trunking (offices, residential)
- Method C: clipped direct (plant rooms, external routes)
- Method E/F: cable tray in risers, cable management systems

### Cable type to table mapping:
| Cable type | Temp rating | Tables |
|---|---|---|
| PVC insulated, PVC sheathed (BS 6004) | 70°C | 4D series |
| XLPE/thermosetting armoured (BS 5467, BS 6724) | 90°C | 4E series |
| Mineral insulated (MICC) (BS 6207) | 70°C or 105°C | 4J series |
| Flexible cords (BS EN 50525) | 60°C/85°C | 4H, 4F series |
| Busbar trunking | — | Appendix 8(L) |

---

## Practical Sizing Example (from Appendix 4(L) worked example)

**Given:** 3-phase circuit, Ib = 58 A, installed in group of 4 on perforated cable tray (Method 11), ambient 35°C, 90°C thermosetting SWA cable, IEC 60898 CB.

1. Select In = 63 A (≥ 58 A)
2. Ca = 0.96 (35°C, 90°C cable), Cg = 0.77 (4 circuits on tray)
3. Required It = 63 / (0.96 × 0.77) = 85.2 A
4. From Table 4E4A: 16 mm² Cu SWA = 99 A ✓
5. Check voltage drop with mV/A/m from Table 4E4A for 16 mm²
