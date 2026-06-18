# SS 638 Part 5 — Wiring, Earthing, and Protective Conductors (Detail)

## Chapter 54 — Earthing Arrangements and Protective Conductors

### Earthing Conductors (cl. 542.3L)

Buried earthing conductor minimum sizes (Table 54.1):

| Protection status | Protected against mech. damage | Not protected against mech. damage |
|---|---|---|
| Protected against corrosion (sheathed) | 2.5 mm² Cu / 10 mm² steel | 16 mm² Cu / 16 mm² coated steel |
| Not protected against corrosion | 25 mm² Cu / 50 mm² steel | 25 mm² Cu / 50 mm² steel |

### Recognised Earth Electrode Types (cl. 542.2.3L)
- Earth rods or pipes
- Earth tapes or wires
- Earth plates
- Underground structural metalwork in foundations
- Welded metal reinforcement of concrete (not pre-stressed)
- Lead sheaths/metal coverings of cables (with consent)

**Prohibited:** Metallic pipes for gas/flammable liquids; water utility supply mains (cl. 542.2.6)

### Protective Conductor (CPC) Sizing

**Rule-of-thumb method — Table 54.7:**
| Line conductor S (mm²) | Min CPC (same material) | Min CPC (different material) |
|---|---|---|
| S ≤ 16 | S mm² | (k₁/k₂) × S |
| 16 < S ≤ 35 | 16 mm² | (k₁/k₂) × 16 |
| S > 35 | S/2 mm² | (k₁/k₂) × (S/2) |

**Adiabatic formula (cl. 543.1.3):**
S = √(I²t) / k

Where:
- S = conductor cross-section in mm²
- I = fault current (A rms)
- t = disconnection time (s) — valid for t ≤ 5 s
- k = material/insulation factor from Tables 54.2–54.6

**k values (Table 54.3 — CPC incorporated in cable or bunched, initial temp 70°C):**
| Material | 70°C thermoplastic | 90°C thermoplastic | 90°C thermosetting |
|---|---|---|---|
| Copper | 115 / 103* | 108 / 86* | 143 |
| Aluminium | 76 / 68* | 66 / 57* | 94 |
*Above 300 mm²

**Minimum standalone CPC (cl. 543.1.1L):**
- If mechanically protected: ≥2.5 mm² copper equivalent
- If NOT mechanically protected: ≥4 mm² copper equivalent

**CPC ≤10 mm² must be copper (cl. 543.2.4L)**

**CPC ≤6 mm² must be covered with insulation throughout (cl. 543.3.201L); use green-yellow sleeving at joints/terminations**

### Main Protective Bonding Conductors (cl. 544.1)

**Minimum size (cl. 544.1.1L):**
- Not less than half the cross-section of the installation's earthing conductor
- Minimum: 6 mm² copper
- Maximum: 25 mm² copper (or equivalent conductance in other materials)

**Connection point (cl. 544.1.2):**
- As near as practicable to point of service entry into premises
- Within 600 mm of meter outlet union or at point of building entry (if meter external)

### Supplementary Bonding Conductors (cl. 544.2)

| Connection type | With mech. protection | Without mech. protection |
|---|---|---|
| Exposed-to-exposed (cl. 544.2.1) | ≥ smaller CPC of the two | ≥ 4 mm² |
| Exposed-to-extraneous (cl. 544.2.2) | ≥ ½ × CPC of exposed-c.p. | ≥ 4 mm² |
| Extraneous-to-extraneous (cl. 544.2.3L) | ≥ 2.5 mm² | ≥ 4 mm² |

---

## Chapter 52 — Wiring Systems

### Cable Concealed in Walls/Partitions (cl. 522.6L)

Cables concealed in walls at depth <50 mm must be:
- Enclosed in earthed metallic conduit or trunking, OR
- Protected by a 30 mA RCD, OR
- Incorporate an earthed metallic screen, OR
- Run horizontally within 150 mm of the top of the wall, or vertically within 150 mm of the corner/angle

### Current-Carrying Capacity (cl. 523)

Apply correction factors to tabulated values (Appendix 4(L)):
- **Ca**: Ambient temperature correction (base reference: 30°C for cables in air; 20°C for buried)
- **Cg**: Grouping/bunching correction (multiple circuits together)
- **Ci**: Thermal insulation factor (fully enclosed = 0.5 for thermoplastic cable)
- **Cc**: Semi-enclosed (BS 3036) fuse factor = 0.725 when using rewirable fuses

**Coordination equation (cl. 433.1):**
Ib ≤ In ≤ Iz
I₂ ≤ 1.45 × Iz

Where:
- Ib = design current of circuit
- In = rated current of protective device
- Iz = current-carrying capacity of cable under installed conditions
- I₂ = current ensuring effective operation of protective device (= 1.45 × In for CB; check fuse characteristics)

### Voltage Drop (Appendix 12(L) — Normative)

Maximum from origin of installation to most remote point:
- **Lighting circuits**: 3% of nominal voltage
  - For 230 V single-phase: max 6.9 V drop
  - For 400 V three-phase: max 12 V drop
- **Other circuits (power, heating, etc.)**: 5% of nominal voltage
  - For 230 V: max 11.5 V
  - For 400 V: max 20 V

Voltage drop calculation: ΔV = (mV/A/m) × Ib × L / 1000

Where mV/A/m values are from Appendix 4(L) tables for the relevant cable type, conductor temperature, and installation method.

---

## Chapter 53 — Protection, Isolation, Switching

### Overcurrent Protective Device Co-ordination (cl. 533)

Device must be selected so:
- Rated current ≥ design current of circuit
- Breaking capacity ≥ prospective fault current at the point of installation
- For discrimination: upstream device shall not operate for faults cleared by downstream device

### RCD Types and Applications (cl. 531.2)

| Type | Characteristic | Typical use |
|---|---|---|
| AC | Responds to sinusoidal a.c. residual current | General use |
| A | Responds to a.c. and pulsating d.c. | Circuits with electronic equipment |
| B | Responds to a.c., pulsating d.c., smooth d.c. | VSD/frequency converters |
| S (selective) | Time-delayed | Upstream/main RCD for discrimination |
| G (general) | Short time-delay | Some discrimination applications |

**RCD rating for TN-S (cl. 531.3):**
Zs × I∆n ≤ 50 V

**RCD rating for TT (cl. 531.4):**
Ra × I∆n ≤ 50 V

**Unwanted tripping (cl. 531.2):**
Where high earth leakage current from equipment (e.g. IT equipment, large motors), consider:
- Separate circuits for high-leakage equipment
- Use Type S or higher I∆n RCD (with separate ≤30 mA RCD for general circuits)
- Refer to 314.1L(iv)

### Isolation Requirements (cl. 537.2)

Every circuit shall have means of isolation:
- Shall isolate all live conductors (line AND neutral in single-phase)
- Must be lockable or otherwise secure against inadvertent re-energisation
- Means shall be clearly identified as to which circuit it controls

### Firefighter's Switches (cl. 537.6)

Required for exterior lighting and signs and interior discharge lighting installations at high voltage:
- Located in accessible position agreed with fire authority
- Coloured red; labelled "FIREFIGHTER'S SWITCH"
- Height: not above 2.75 m from ground

---

## Chapter 55 and 56 Highlights

### Generator Sets (cl. 551)
- Automatic changeover: switching must not connect standby generator in parallel with mains unless generator is designed for parallel operation
- Earthing of generator: if used as standby to TN-S system, PE of generator must connect to installation's main earthing terminal

### Safety Services (cl. 560)
- Sources: battery (response time ≤0.5 s for emergency lighting), UPS, motor-generator
- Circuits for safety services must be independent of other circuits
- Emergency escape lighting: see SS 563
- Fire detection and alarms: see SS 645

---

## Identification (Chapter 51, cl. 514)

### Cable Core Colours — New System (Appendix 7(L) — Normative)

**Single-phase AC:**
- Line: Brown
- Neutral: Blue
- Protective: Green-yellow

**Three-phase AC:**
- Line 1 (L1): Brown
- Line 2 (L2): Black
- Line 3 (L3): Grey
- Neutral: Blue
- Protective: Green-yellow

**Old colours (pre-SS 638):** Red (L), Yellow (L2), Blue (L3), Black (N) — Annex B(L) covers transition.

**Warning notice required (cl. 514.14)** where old and new colour systems coexist.

### Documentation (cl. 514.9, 132.13)

Every installation shall have:
- Single-line diagram showing system earthing, protective devices, circuit identification
- Schedule of circuits with current ratings and cable types
- Test results certificate (Chapter 63 / EMA prescribed forms)
