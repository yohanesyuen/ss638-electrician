# SS 638 Electrician — AI Assistant Skill

An AI skill providing expert-level guidance on **SS 638:2018+C1:2020+A1:2022** — Singapore's *Code of Practice for Electrical Installations* (formerly CP 5). The skill covers circuit design, cable sizing, earthing, RCD protection, inspection/testing, and all Part 7 special locations (bathrooms, PV, EV charging, construction sites, etc.).

Answers include clause-level citations and flag Singapore-specific (L) deviations from BS 7671.

---

## Install on Claude Code

Claude Code uses `.skill` files installed via the CLI.

### Prerequisites

- [Claude Code](https://claude.ai/code) installed
- A Claude subscription (Pro or above)

### Steps

1. Clone this repository:
   ```bash
   git clone https://github.com/yuenweiping/ss638-electrician.git
   cd ss638-electrician
   ```

2. Install the skill:
   ```bash
   claude skill install claude/
   ```

3. Verify it is active — in Claude Code, type:
   ```
   /ss638-electrician
   ```
   or ask any question about Singapore electrical installations. The skill triggers automatically.

### What triggers the skill

The skill activates when you ask about:
- Electrical installation design, wiring, or earthing in Singapore
- RCD protection rules, socket-outlet requirements
- Cable sizing, voltage drop, correction factors
- Disconnection times, earth fault loop impedance
- Inspection, testing, EMA certification
- Special locations: bathrooms, PV systems, EV charging, construction sites, pools
- SS 638 clause queries, or comparisons with BS 7671

---

## Install on ChatGPT (Custom GPT)

### Prerequisites

- [ChatGPT Plus, Team, or Enterprise](https://chatgpt.com) subscription
- Access to the **My GPTs** feature

### Steps

1. Go to [chatgpt.com](https://chatgpt.com) → click your profile → **My GPTs** → **Create a GPT**

2. Click **Configure**

3. Fill in the fields:
   - **Name**: `SS 638 Electrician`
   - **Description**: `Expert on Singapore's SS 638 Code of Practice for Electrical Installations. Gives clause-level answers on wiring, earthing, RCDs, cable sizing, special locations, and EMA compliance.`

4. In the **Instructions** field, paste the entire contents of [`chatgpt/system-prompt.md`](chatgpt/system-prompt.md)
   *(copy everything after the `---` separator at the top of the file)*

5. Under **Capabilities**, enable:
   - [x] Web search *(optional — allows looking up related EMA circulars)*

6. Click **Save** → **Only me** (or **Anyone with a link** to share)

7. Start a conversation and ask something like:
   > *"What is the maximum Zs for a 16 A Type B MCB at 230 V in a TN-S system?"*

---

## Repository Structure

```
ss638-electrician/
├── README.md                          ← you are here
├── claude/
│   ├── SKILL.md                       ← Claude Code skill definition
│   └── references/
│       ├── part4-electric-shock.md    ← Chapter 41: disconnection tables, SELV/PELV
│       ├── part5-wiring-earthing.md   ← Chapters 52–54: CPC sizing, bonding, colours
│       ├── appendix4-cable-tables.md  ← Cable current capacity & correction factors
│       └── special-locations.md      ← Part 7: bathrooms, PV, EV, pools, etc.
└── chatgpt/
    └── system-prompt.md               ← Flattened system prompt for Custom GPT
```

The Claude skill uses a modular approach: the main `SKILL.md` loads reference files on demand, keeping the base context small. The ChatGPT system prompt inlines all content since Custom GPTs do not support dynamic file loading.

---

## Coverage

| Topic | Clause reference |
|---|---|
| TN-S / TT earthing systems | cl. 411.4L, 411.5 |
| Disconnection times | Table 41.1 |
| RCD ≤30 mA domestic rule | cl. 411.3.3L |
| Max Zs for MCBs (Type B/C/D) | Table 41.3L |
| Max Zs for fuses | Tables 41.2, 41.4 |
| CPC sizing | Table 54.7 |
| Main bonding conductors | cl. 544.1.1L |
| Cable concealment in walls | cl. 522.6L |
| Voltage drop limits | Appendix 12(L) |
| Cable sizing procedure | Appendix 4(L) |
| Correction factors Ca, Cg, Ci | Tables 4C1, 4B1, 4B2 |
| Bathroom zones | Section 701L |
| Solar PV | Section 712L |
| EV charging | Section 722L |
| Construction sites | Section 704L |
| Festive lighting | Section 740L |
| Inspection & test sequence | Chapter 61 |
| EMA certification forms | cl. 63L |

---

## Limitations

- This skill is based on **SS 638:2018+C1:2020+A1:2022**. Always verify against the current edition purchased from [Enterprise Singapore (ESG)](https://www.singaporestandardseshop.sg/).
- The skill is an informational aid. For licensed electrical work in Singapore, consult a qualified and licensed electrical worker (LEW) registered with EMA.
- Cable current-carrying capacity tables in Appendix 4(L) contain many variants; this skill covers the most common installation methods. For unusual installations, refer to the full standard.

---

## Licence

MIT — free to use, modify, and redistribute. Attribution appreciated.
