---
name: ss638-electrician
description: >
  Expert knowledge of SS 638:2018+C1:2020+A1:2022 — Singapore's Code of Practice for
  Electrical Installations (formerly CP 5). Use this skill whenever the user asks about
  electrical installation design, wiring, earthing, protection, cable sizing, RCDs,
  inspection, testing, special locations (bathrooms, pools, PV, EV charging), or
  compliance with Singapore electrical standards. Trigger for any question involving
  circuit design, overcurrent protection, disconnection times, bonding, socket-outlet
  RCD rules, voltage drop, Singapore electrical regulations, EMA requirements, or
  any clause-level query about SS 638. Also trigger for questions comparing SS 638 to
  BS 7671 or IEC standards.
---

# SS 638 Electrician Skill

You are an expert on **SS 638:2018+C1:2020+A1:2022** — *Code of Practice for Electrical Installations* — Singapore's primary standard for the design, erection, and verification of electrical installations. You answer with clause-level precision, cite specific section numbers, and flag Singapore-specific deviations from BS 7671 (the UK standard this is based on).

---

## Document Structure

SS 638 uses a decimal numbering system (Part → Chapter → Section → Clause):
- **Part 1** – Scope, Object and Fundamental Principles (Ch 11–13)
- **Part 2** – Definitions
- **Part 3** – Assessment of General Characteristics (Ch 30–36)
- **Part 4** – Protection for Safety (Ch 41–43)
- **Part 5** – Selection and Erection of Equipment (Ch 51–56)
- **Part 6** – Inspection and Testing (Ch 61–63)
- **Part 7** – Special Installations/Locations (Sections 701L–740L)
- **Appendices 1–16** and **Annexes A(L), B(L)**

Clauses marked **(L)** are Singapore-local modifications to BS 7671.

---

## Key Singapore Deviations from BS 7671

1. **TN-S only** — IT and TN-CS (PEN conductor) systems are prohibited in Singapore. Only TN-S and TT systems permitted (cl. 411.4L, 411.5).
2. **Skilled person definition** — Defined as a person licensed as an electrical worker under the *Electricity (Electrical Workers) Regulations* (Part 2 definitions).
3. **Section 114.1L** — Compliance with SS 638 may be a statutory requirement under Acts listed in Appendix 2(L) (Electricity Act, etc.).
4. **RCD requirements are more stringent** — Domestic installations: ALL socket-outlet and lighting circuits must have ≤30 mA RCD (cl. 411.3.3L).
5. **No caravans, marinas, IT systems, PEN conductors** — those BS 7671 sections deleted as not applicable in Singapore.
6. **Medical locations** moved to informative Annex A(L) (not normative).
7. **Cable colours** — New cable colour code in Appendix 7(L) and Annex B(L).
8. **Voltage drop** — Appendix 12(L) is normative for consumers' installations.

---

## Part 4: Protection for Safety (Key Rules)

### Chapter 41 — Protection Against Electric Shock

**Permitted protective measures (cl. 410.3.3L):**
1. Automatic disconnection of supply (ADS) — most common
2. Double or reinforced insulation (Section 412)
3. Electrical separation — single item only (Section 413)
4. SELV / PELV (Section 414)

**ADS (Section 411) — TN-S system (cl. 411.4L):**
- Exposed-conductive-parts connected to protective conductor
- Max disconnection times (Table 41.1) for final circuits ≤32 A:
  - 230 V (U₀): **0.4 s** (a.c.)
  - >400 V: **0.1 s** (a.c.)
  - Distribution circuits: max 5 s permitted (cl. 411.3.2.3L)
- Earth fault loop impedance condition: Zs × Ia ≤ U₀

**ADS — TT system (cl. 411.5):**
- Each exposed-conductive-part connected to earth electrode independent of supply
- Disconnection by RCD (preferred) or overcurrent device
- RCD condition: Ra × I∆n ≤ 50 V (cl. 411.5.3L)
- Overcurrent condition: Zs × Ia ≤ U₀ (cl. 411.5.4L)
- Distribution circuits: max 1 s (cl. 411.3.2.4L)

**RCD additional protection (cl. 411.3.3L) — SINGAPORE SPECIFIC:**
- ≤30 mA RCD required for:
  - Socket-outlets ≤32 A for ordinary persons / general use
  - Portable equipment ≤32 A for outdoor use
- **Domestic installations: ALL socket-outlet AND lighting circuits protected by ≤30 mA RCD**
- Exception: fire alarms, battery chargers, public address, medical equipment — must be labelled "SOCKET-OUTLET NOT PROTECTED BY RCD" (white on red)

**SELV / PELV (Section 414):**
- SELV: electrically separated from earth and other systems; nominal voltage ≤50 V a.c. / ≤120 V d.c.
- PELV: not separated from earth, but otherwise meets SELV requirements
- FELV (cl. 411.7): ELV system that doesn't fully meet SELV/PELV — requires supplementary protective provisions

**Supplementary equipotential bonding (cl. 415.2):**
- Applied when disconnection time cannot be achieved
- Resistance R between simultaneously accessible parts: R ≤ 50/Ia

**Protective bonding (cl. 411.3.1.2L):**
Main bonding conductors must connect to main earthing terminal:
- Water installation pipes
- Gas installation pipes
- Other pipework and ducting
- Central heating and air conditioning
- Exposed metallic structural parts of the building

---

## Part 5: Selection and Erection of Equipment

### Chapter 52 — Wiring Systems

Key wiring method considerations:
- Nature of location, structure, accessibility, voltage
- Electromechanical stresses, EMI, external influences
- **Cables concealed in walls/partitions** — must comply with depth/protection requirements (cl. 521.6 area)
- Ambient temperature correction, grouping derating apply to current-carrying capacity (Appendix 4(L))

### Chapter 53 — Protection, Isolation, Switching

- Single-pole fuse/switch/CB: line conductor only (cl. 132.14.1)
- No switch or fuse in earthed neutral conductor except linked switch that breaks all line conductors (cl. 132.14.2)
- Isolation must disconnect all live conductors; means must be accessible (cl. 537)
- Emergency switching must be readily accessible and operable (cl. 132.9)

### Chapter 54 — Earthing and Protective Conductors

Minimum CPC cross-sectional area (Table 54.7):
| Line conductor S (mm²) | Min CPC (mm²) |
|---|---|
| S ≤ 16 | S (same) |
| 16 < S ≤ 35 | 16 |
| S > 35 | S/2 |

Main protective bonding conductor: min 6 mm² copper (or per Table 54.8).

### Chapter 55 — Other Equipment
- Low voltage generating sets, luminaires, street furniture
- Section 557: Auxiliary circuits

### Chapter 56 — Safety Services
- Emergency escape lighting (reference SS 563)
- Fire protection applications (reference BS 8519)
- Supply source must maintain operation during emergencies

---

## Part 6: Inspection and Testing

### Chapter 61 — Initial Verification (before energisation)
Visual inspection items include:
- Connection of conductors, correct identification
- Presence and position of labels and warning notices
- Adequacy of conductors for current-carrying capacity and voltage drop
- Correct selection of protective devices

Tests (in order):
1. Continuity of protective conductors and main/supplementary bonding
2. Continuity of ring final circuit conductors
3. Insulation resistance (min 1 MΩ between live conductors and earth; 0.5 MΩ for SELV/PELV)
4. Polarity
5. Earth electrode resistance (for TT systems)
6. Earth fault loop impedance (Zs)
7. Prospective fault current
8. Functional testing (RCDs, etc.)

### Chapter 62 — Periodic Inspection and Testing
Frequency determined by type of installation and risk assessment.

### Chapter 63 — Certification and Reporting (cl. 63L)
Prescribed forms under local Singapore regulations (EMA forms); not the BS 7671 model forms.

---

## Part 7: Special Installations and Locations

### Section 701L — Bath/Shower Locations
Zones defined around bath/shower (Zones 0, 1, 2):
- **Zone 0** (inside bath/shower basin): Only SELV ≤12 V a.c. / 30 V d.c. Equipment IPX7 minimum
- **Zone 1** (above bath/shower, up to 2.25 m): SELV or equipment rated min IPX4; no socket-outlets
- **Zone 2** (extends 0.6 m from Zone 1): Socket-outlets and switches not permitted; RCD ≤30 mA required for all circuits in zones 1 and 2
- Supplementary equipotential bonding required for all metallic parts (pipes, taps, waste, heating, etc.)
- Shaver supply units (BS EN 61558-2-5) permitted in Zone 2 and outside

### Section 702 — Swimming Pools and Other Basins
Zone 0, 1, 2 defined similarly with stricter restrictions; IPX5/IPX8 requirements apply.

### Section 703 — Sauna Heaters
High-temperature environment; only wiring to sauna equipment permitted; min IP24; no socket-outlets in sauna room.

### Section 704L — Construction Sites
Reduced voltage systems (110 V, centre-tapped) preferred; 30 mA RCD mandatory.

### Section 705 — Agricultural/Horticultural Premises
- Additional bonding for all metallic parts
- 30 mA RCD for all socket-outlets
- Accounts for livestock contact with floors/structures

### Section 712L — Solar PV Systems
- DC cables: rated for PV duty, min 600 V d.c.; separate from AC wiring
- Isolation on both AC and DC sides required
- Anti-islanding protection (inverter must meet SS/IEC standards)
- DC arc fault detection recommended
- Surge protection (SPD) at AC and DC sides
- PV systems on buildings: Appendix 7(L) wiring colour rules apply

### Section 714 — Outdoor Lighting
IP ratings appropriate for outdoor environment; RCD protection; earthing.

### Section 715 — Extra-Low Voltage Lighting
SELV or PELV systems; insulation and segregation requirements.

### Section 722L — Electric Vehicle Charging
- Mode 2, 3, 4 charging equipment
- 30 mA RCD required
- Socket-outlets for EV charging not for general use
- Dedicated circuit recommended
- PME (TN-C-S) NOT permitted in Singapore; TN-S or TT only

### Section 729 — Operating and Maintenance Gangways
Clearances, lighting, emergency escape requirements for HV/LV switchrooms.

### Section 740L — Festive Lighting / Trade Fairs
Temporary installations; 30 mA RCD mandatory; IP44 minimum for outdoor equipment.

---

## Cable Sizing and Voltage Drop (Appendices 4(L) and 12(L))

**Voltage drop limits (Appendix 12(L) — normative):**
- Lighting: 3% of nominal voltage
- Other uses: 5% of nominal voltage
- From origin of installation to final point of use

**Current-carrying capacity:** Use tables in Appendix 4(L); apply:
- Ambient temperature correction factor (Ca)
- Grouping/bunching correction factor (Cg)
- Thermal insulation correction factor (Ci)
- Installation method (reference methods A–F and variants)

**Busbar trunking systems:** Appendix 8(L)

---

## Earthing Systems in Singapore

Only **TN-S** and **TT** systems permitted:
- **TN-S**: Separate N and PE conductors throughout; PE connected to earthed source neutral
- **TT**: Source neutral earthed, installation exposed-conductive-parts earthed via independent electrode

TN-C-S (PME) is **not permitted** in Singapore (deleted from scope).

---

## How to Answer Queries

1. **Cite clause numbers** (e.g., "per cl. 411.3.3L...") — users may need to cross-reference
2. **Flag (L) clauses** as Singapore-specific deviations
3. **For cable sizing**: Walk through: design current → Ib, rated current of protective device → In, tabulated current → It, then apply correction factors to get actual Iz ≥ In ≥ Ib
4. **For earthing/bonding questions**: Identify system type (TN-S or TT), then apply correct disconnection time table
5. **For special locations**: Always check Part 7 for additional/overriding requirements
6. **For inspection/test values**: Quote the pass/fail criteria explicitly

## Reference Files

For deep-dive content on specific topics, load the relevant reference file:
- `references/part4-electric-shock.md` — Full Chapter 41 clauses, disconnection time tables (41.1–41.5), SELV/PELV/FELV
- `references/part5-wiring-earthing.md` — Chapters 52–54: CPC sizing, bonding conductor sizes, voltage drop limits, cable colours, RCD selection, isolation
- `references/appendix4-cable-tables.md` — Cable current-carrying capacity correction factors (Ca, Cg, Ci), installation method reference methods, mV/A/m values
- `references/special-locations.md` — Full Part 7 requirements: bathroom zones, PV, EV charging, construction sites, pools, saunas, festive lighting

> **Note:** Reference files contain extracted/synthesised content from SS 638. Load only the relevant one per query.
