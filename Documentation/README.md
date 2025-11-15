# RD-54 "Zorro" Documentation

**Aircraft Designator**: RD-54 (Code Name: Zorro)
**Operator**: SpyD (Franco Nogarin)
**Platform**: 3.5" Digital FPV Cruiser
**Primary Mission**: Exploration and cinematic FPV flights with HD digital video
**Last Updated**: November 14, 2025

---

## Quick Reference

### Current Status

| Attribute | Value |
|-----------|-------|
| **Build Status** | Assembly Phase (~70% complete) |
| **Airworthiness** | Not Yet Airworthy (under construction) |
| **Flight Hours** | 0.0 |
| **Total Incidents** | 0 |
| **Total Modifications** | 1 (MOD-001: GPS Stack) |
| **Configuration** | Original Build Spec + GPS Stack Enhancement |
| **Mission Profile** | Digital FPV Cruiser |
| **Latest Milestone** | Motor wiring complete (Nov 14, 2025) |

### Key Specifications

| Component | Current Configuration |
|-----------|---------------------|
| **Frame** | FlyFishRC Volador VX3.5 (3.5") |
| **FC/ESC** | SpeedyBee F405 AIO 40A (3-6S) |
| **Motors** | Emax ECO II 2004 3000KV |
| **Props** | Gemfan Hurricane 3525-3 Tri-Blade |
| **VTX** | Walksnail Moonlight HD digital (LHCP) |
| **RX** | HappyModel ExpressLRS EP1 (long range) |
| **GPS** | GEPRC M10-DQ with DPS310 baro |
| **GPS-Mate** | VIFLY GPS-Mate (lost model recovery) |
| **GPS Mount** | Custom 3D printed TPU stack (MOD-001) |
| **Battery** | 2x GNB 880mAh 6S HV 160C XT30 |

---

## Documentation Structure

### Primary Documentation

#### 1. [RD-54_AsBuilt_Parts_List.md](RD-54_AsBuilt_Parts_List.md)
**Single source of truth for current aircraft configuration**

Contains:
- Complete parts list with status
- Current operational configuration
- Pending upgrades
- Known issues
- Maintenance log

**Update when**: Parts are changed, issues discovered, maintenance performed

---

#### 2. [RD-54_Incident_Log.md](RD-54_Incident_Log.md)
**Comprehensive crash reports and damage assessments**

Contains:
- Chronological incident reports
- Damage assessments
- Root cause analysis
- Repair actions
- Lessons learned

**Update when**: Any crash, incident, or damage occurs

---

#### 3. [RD-54_Modifications_Log.md](RD-54_Modifications_Log.md)
**Track all engineering changes from original specification**

Contains:
- Sequential modification records (MOD-XXX)
- Original vs modified configuration
- Rationale and justification
- Installation procedures
- Performance impact

**Update when**: Planning, installing, or completing any modification

---

#### 4. [RD-54_Build_Timeline.md](RD-54_Build_Timeline.md)
**Chronological project history and future planning**

Contains:
- Build phases and milestones
- Project statistics
- Lessons learned
- Future activities

**Update when**: Major milestones reached, planning future work

---

### Reference Materials

#### [spyd.com_RD-54_README.md](spyd.com_RD-54_README.md)
Original parts list from spyd.com site. Reference only.

---

## How to Use This Documentation

### For Operators (SpyD)
1. **After a crash**: Document in `RD-54_Incident_Log.md`
2. **Ordering parts**: Update `RD-54_AsBuilt_Parts_List.md` (mark as "pending")
3. **Installing upgrades**: Create entry in `RD-54_Modifications_Log.md`
4. **After installation**: Update parts list status to "operational"
5. **Major milestones**: Update `RD-54_Build_Timeline.md`

### For Future Claude Instances
1. Read `CLAUDE.md` in repository root (your instructions)
2. Read this README (navigation guide)
3. Check `RD-54_AsBuilt_Parts_List.md` for current config
4. Review recent incident and modification entries
5. Ask operator what needs documenting

### For Documentation Maintenance
- Keep all cross-references current
- Update "Last Updated" dates
- Maintain chronological integrity
- Preserve historical records
- Follow markdown formatting standards

---

## Documentation Standards

### Markdown Formatting
- Tables for component lists and comparisons
- `---` dividers between major sections
- `**bold**` for component names and key terms
- `[ ]` checkboxes for pending actions
- Dates in ISO format (YYYY-MM-DD) or full format

### Technical Accuracy
- Full part numbers and model names
- Vendor names and order dates
- Quantities and prices when available
- Specific pad/connector names
- Units for all measurements (voltage, power, frequency)

### Documentation Voice
- Clear, technical language
- Assume FPV drone knowledge
- Document for future troubleshooting
- Include warnings and critical notes
- Capture operator's rationale

---

## Current Focus Areas

**Mission Profile**: Digital FPV Cruiser - optimized for smooth exploration flights with HD digital video

**Build Progress**: Assembly phase ~70% complete (started May 26, 2025)
- ✓ Frame assembled
- ✓ All motors mounted and wired (4 of 4 - completed Nov 14, 2025)
- ✓ FC/ESC stack installed and positioned
- ✓ Custom GPS stack fabricated and wired (MOD-001)
- ⏳ Remaining: Install VTX/Camera/RX/buzzer, mount GPS stack (last), wire management

**Next Steps**:
- Install Walksnail Moonlight VTX/Camera (next major task)
- Install ExpressLRS receiver
- Install buzzer
- Wire management and antenna routing
- Mount GPS stack to frame (planned as final component)
- Install top plate
- Betaflight configuration (GPS Rescue, RTH enabled)
- Bench testing
- Maiden flight

**Key Features for Cruiser Mission**:
- Walksnail HD digital FPV for cinematic footage
- GPS Rescue and Return Home for extended range safety
- VIFLY GPS-Mate for lost model recovery
- ExpressLRS long-range control link

**Documentation Priorities**:
- Document build progress and assembly milestones
- Capture configuration decisions for cruiser-optimized setup
- Record any issues encountered

---

## Contact & Support

**Operator**: SpyD (Franco Nogarin)
**Archivist**: Claude Code, RD-54 SME
**Repository**: /Users/franconogarin/localcode/rd54_zorro

---

## Document History

- **v1.0** (Nov 14, 2025): Initial documentation structure created
  - Created primary documentation files
  - Established templates and standards
  - Populated with current build information

---

**Next Review Date**: After first flight or major milestone

**Archivist**: Claude Code, RD-54 SME
