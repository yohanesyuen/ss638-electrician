# SS 638 Part 7 — Special Installations and Locations (Detail)

---

## Section 701L — Locations Containing a Bath or Shower

### Zone Definitions

**Zone 0:** Interior of the bath tub or shower basin only.
- For showers without a basin: 0.10 m height zone with same horizontal extent as Zone 1.

**Zone 1:** Limited by:
- Floor level to 2.25 m above floor (or to highest fixed shower head if higher)
- Vertically: surface circumscribing the bath/shower basin; OR 1.20 m from centre of fixed wall/ceiling shower outlet (for showers without basin)
- Zone 1 includes the space under the bath tub (unless only accessible with a tool)

**Zone 2:** Limited by:
- Same height as Zone 1
- Extends 0.60 m horizontally beyond the Zone 1 boundary
- (For showers without basin: no Zone 2 — Zone 1 is extended to 1.20 m radius)

### Restrictions by Zone

| Item | Zone 0 | Zone 1 | Zone 2 | Outside (≥3m from Zone 1) |
|---|---|---|---|---|
| Socket-outlets | ✗ | ✗ | ✗ | ✓ (if >3m from Zone 1) |
| SELV socket-outlets | ✗ | ✗ | ✓ (source outside zones) | ✓ |
| Shaver supply unit (IEC 61558-2-5) | ✗ | ✗ | ✓ (if no direct spray) | ✓ |
| Switches (non-SELV) | ✗ | ✗ | ✗ | ✓ |
| SELV switches (≤12V a.c. / ≤30V d.c.) | ✗ | ✓ | ✓ | ✓ |
| Pull cord switches | ✓ | ✓ | ✓ | ✓ |
| IP rating min. | IPX7 | IPX4 | IPX4 | Normal |
| Water jets (cleaning) | — | IPX5 | IPX5 | — |

### Equipment Permitted in Zone 0
Only fixed, permanently connected equipment protected by SELV ≤12 V a.c. / ≤30 V d.c. (source outside all zones), meeting IP rating and zone suitability per manufacturer.

### Equipment Permitted in Zone 1
Fixed and permanently connected only:
- Whirlpool units, electric showers, shower pumps
- SELV/PELV equipment ≤25 V a.c. / ≤60 V d.c.
- Ventilation equipment, towel rails, water heating appliances
- Equipment rated for Zone 1 per manufacturer

### Protection Requirements
- **All circuits in bath/shower location: ≤30 mA RCD required** (cl. 701.411.3.3)
- Supplementary equipotential bonding required connecting all metallic pipes (water, gas, waste, heating, a/c) and metallic structural parts to PE conductors of circuits
- Supplementary bonding may be omitted if: all circuits comply with ADS disconnection times, all have ≤30 mA RCD, and all extraneous-conductive-parts are connected to main equipotential bonding (cl. 701.415.2)

### Luminaires
Parts of a lampholder within 2.5 m of bath/shower cubicle: insulating material or totally enclosed luminaire required. B22 lampholders need protective shield per IEC 60061.

### Electric Bidets (cl. 701.55.2L — Singapore specific)
- 16 A MCB + RCCB (voltage-independent type to SS 97) with **10 mA** rated residual operating current
- 20 A double-pole switch outside toilet
- 16 A weatherproof connection unit IP55 (non-metallic casing) near control box
- Bidet installed **outside** Zones 0, 1, and 2
- Compliant with IEC 60335-2-84

---

## Section 702 — Swimming Pools and Other Basins

### Zone Definitions
- **Zone 0:** Interior of basin including recesses, foot-cleaning basins, water jets/waterfalls
- **Zone 1:** From Zone 0 to 2 m from rim, floor to 2.5 m height; or 1.5 m from diving boards/structures
- **Zone 2:** From Zone 1 boundary to 1.5 m further; same height. **No Zone 2 for fountains.**

### Protection Requirements by Zone

| Zone | Permitted protective measure | Socket-outlets/switches | IP rating |
|---|---|---|---|
| 0 | SELV ≤12 V a.c. / ≤30 V d.c. only (source outside zones 0,1,2) | None | IPX8 |
| 1 | SELV ≤25 V a.c. / ≤60 V d.c. only | None | IPX4 (IPX5 where jets likely) |
| 2 | SELV, or ADS with ≤30 mA RCD, or electrical separation | Permitted with ≤30 mA RCD | IPX2 indoor / IPX4 outdoor (IPX5 where jets) |

All extraneous-conductive-parts in Zones 0, 1, 2: supplementary equipotential bonding required.

No switchgear or controlgear in Zones 0 or 1. No junction boxes in Zones 0 or 1 (SELV junction boxes permitted in Zone 1).

Metallic cable sheaths in Zones 0, 1, 2: connected to supplementary equipotential bonding.

---

## Section 703 — Sauna Heaters

### Requirements
- Only wiring for sauna equipment permitted inside the sauna room
- Minimum IP24 for equipment inside sauna
- No socket-outlets in sauna room
- Cables for sauna heater to withstand high temperatures (min 170°C insulation rating)
- Pull-cord switches permitted; standard light switches not permitted inside sauna
- Thermostat and thermal cutout (per sauna heater standard EN 60335-2-53) required

---

## Section 704L — Temporary Electrical Installations for Construction Sites

Refer to **SS 650-1** for primary requirements. SS 638 Section 704L is largely superseded.

Key points still applicable:
- 30 mA RCD mandatory for all socket-outlet circuits
- Reduced voltage (110 V centre-tapped to earth, 55 V to earth) preferred for portable tools
- Inspection and testing before energising and periodically (minimum monthly recommended)
- Distribution boards: lockable, weatherproof, clearly labelled

---

## Section 705 — Agricultural and Horticultural Premises

### Key Requirements
- 30 mA RCD for all socket-outlets
- Additional supplementary equipotential bonding for all metallic parts, including:
  - Steel frames of buildings
  - Metallic water/feed troughs
  - Metallic fittings and pipes
- IP rating for equipment in livestock areas: minimum IP44 (higher where water jets used)
- Residences/offices connected to agricultural installation: bonding to agricultural installation PE
- High-density livestock rearing: standby power supply for life-support systems (cl. 35 applies)
- Cable types: armoured cables preferred; PVC/rubber sheathed cables to be protected from mechanical damage and rodents

---

## Section 712L — Solar Photovoltaic (PV) Power Supply Systems

### Scope
Applies to all PV power supply systems connected to Singapore buildings/installations, including grid-tied and battery storage systems.

### System Earthing (cl. 712.312.2L)
One live conductor of d.c. side may be earthed only if there is **at least simple separation** between a.c. and d.c. sides (e.g. transformer-type inverter). Transformerless inverters: neither pole of d.c. side earthed unless via specific safety measures.

### Protection Against Electric Shock
- PV equipment on d.c. side: considered energised even when disconnected from a.c. side
- Non-conducting location and earth-free bonding (Section 418L): NOT permitted on d.c. side
- Class II (double insulated) equipment preferred for d.c. side

### RCD Requirements (cl. 712.411.3.2.1.2L)
- Transformerless inverters: **Type B RCD** (IEC 62423) required to protect against d.c. fault currents
- Type B RCD may be omitted if inverter has built-in residual current monitoring with automatic disconnection
- Inverters with built-in transformer: Type B RCD not required

### Overload Protection — DC Side
- PV string/array cables: overload protection may be omitted if cable rating ≥ 1.25 × Isc STC
- PV d.c. main cable: overload protection may be omitted if rating ≥ 1.25 × Isc STC of PV generator

### String Fuse Sizing (cl. 712.512.1.1L)
If N strings in parallel and (N-1) string combined Isc exceeds module max reverse current, each string needs fuse or blocking diode.
Fuse sizing: **1.5 × Isc_MOD < In < 2.4 × Isc_MOD** AND In ≤ IMOD_MAX_OCPR

### Cable Requirements
- All d.c. side cables: rated for d.c. voltage; UV-resistant; single-core sheathed preferred
- Minimise loop areas to reduce lightning-induced voltages
- Cables must withstand wind, temperature, solar radiation (cl. 712.522.8.3L)

### Isolation (cl. 712.537.2.2.5L)
- DC switch-disconnector required at PV inverter d.c. side (external or built-in)
- Must comply with IEC 60947-3, utilisation category **DC21B**
- Combiner boxes: warning label required — "parts may be live after isolation from inverter"

### Grid-Connected Systems (cl. 712.55L) — Singapore Specific
- Anti-islanding protection mandatory: automatic disconnection on loss of supply or voltage/frequency deviation
- PV system must not cause adverse effects (harmonics, power factor, voltage changes) to grid
- Consult SP Group (public supply owner) for connection requirements
- **Warning notices (DUAL SUPPLY)** required at: origin of installation, meter position, DB/consumer unit, all isolation points

### PV Module Requirements (cl. 712.511.1L) — Singapore Specific
- Comply with IEC 61215-1
- Classified per IEC 61730-1 and rated for application
- Building-mounted PV: **minimum Class C module fire class** (per ANSI/UL 790 Spread of Flame and Burning Brand tests)

---

## Section 714 — Outdoor Lighting Installations

### Scope
Roads, parks, car parks, gardens, sports areas, monuments, advertising panels, illuminated signs.
Excludes: utility distribution, festoon lighting, luminaires fixed to building supplied from internal wiring, traffic signals.

### Protection
- Max disconnection time: 5 s for all circuits (applies cl. 411.3.2.3L for TN-S or 411.3.2.4L for TT)
- RCD protection required for all circuits (≤30 mA for general; higher sensitivity acceptable with separate RCDs per 531.2.9L)
- Earthing conductor of street fixture: min copper equivalent = supply neutral conductor, and not less than **6 mm²** (cl. 714.411.203L)

### Access to Enclosures
- Doors below 2.5 m: lockable; basic protection maintained when door open (IPXXB/IP2X minimum)
- Luminaire below 2.8 m: access to light source requires tool

---

## Section 722L — Electric Vehicle Charging Systems

**Refer to TR 25** (Technical Reference 25 — Electric Vehicle Charging System) for full compliance.

### Key Requirements from TR 25 / SS 638 context
- Mode 2: standard socket-outlet with in-cable control box (ICCB); 30 mA RCD required
- Mode 3: dedicated EVSE (Electric Vehicle Supply Equipment); 30 mA RCD required; dedicated circuit recommended
- Mode 4: DC fast charging
- **TN-C-S (PME) NOT permitted in Singapore** — only TN-S or TT
- Socket-outlets for EV charging designated and labelled separately from general socket-outlets
- Current capacity: circuits to be sized for continuous loading (EV charging is continuous duty)
- Earthing: dedicated PE conductor throughout; no shared neutral/earth (no PME)
- Smart metering/load management recommended for multiple EVSE installations

---

## Section 729 — Operating and Maintenance Gangways

### Minimum Gangway Dimensions (cl. 729.513.2)

**With barriers/enclosures (ADS protective measure):**
- Between barriers/enclosures and switch handles (most onerous position): **700 mm**
- Between barriers/enclosures and wall: **700 mm**
- Height from floor to barrier/enclosure: **2000 mm**
- Live parts placed out of reach (cl. 417.3L): **2500 mm** above floor

**With obstacles (skilled/instructed persons only):**
- Same 700 mm / 700 mm / 2000 mm / 2500 mm dimensions apply

**Gangway length rules:**
- Gangways > 10 m: accessible from **both ends**
- Closed areas > 20 m: escape doors at both ends required
- Closed areas > 6 m: access from both ends recommended
- Door dimensions: width ≥ 700 mm, height ≥ 2000 mm; open outwards

---

## Section 740L — Festive Lighting, Trade-Fairs, Mini-Fairs, Exhibition Sites

**Refer to SS 650-2** for full compliance.

### Key Requirements
- **30 mA RCD mandatory** for all circuits
- Outdoor equipment: minimum **IP44**
- All temporary installations: inspected and tested before energising
- Wiring: armoured or protected; not run as trip hazard
- Generators: used as standby or primary source shall comply with cl. 551 (generating sets) and be properly earthed

---

## Annex A(L) — Medical Locations (Informative)

### Location Groups
- **Group 0:** No applied parts; supply interruption not life-threatening
- **Group 1:** Applied parts used externally or non-cardiac invasively; supply interruption not directly life-threatening
- **Group 2:** Applied parts for intracardiac procedures or vital/surgical; supply interruption may be life-threatening

### Key Requirements for Group 2 Locations
- **Medical IT system** (isolated power supply) required for final circuits supplying equipment with applied parts
- IT system monitor: insulation monitoring device to detect first fault; visual and audible alarm
- Automatic disconnection NOT used for final circuits with applied parts (would interrupt supply to life-critical equipment)
- Supplementary equipotential bonding: all exposed and extraneous conductive parts within patient environment (2.5 m radius around patient)
- Max resistance of supplementary bonding: ≤0.2 Ω
- Socket-outlets in Group 2: min 16 A, with individual labelling, connected to UPS-backed circuits where appropriate
- Safety services: max 0.5 s changeover time for critical medical equipment
