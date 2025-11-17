# RD-54 "Zorro" - Modifications Log

**Aircraft Designator**: RD-54 (Code Name: Zorro)
**Operator**: SpyD (Franco Nogarin)
**Last Updated**: November 15, 2025

---

## Purpose

This log tracks all engineering changes and modifications to RD-54 "Zorro" from the original build specification. Each modification receives a sequential MOD number.

---

## Modification Summary

| MOD # | Date | Category | Component | Status | Impact |
|-------|------|----------|-----------|--------|--------|
| MOD-001 | Nov 2025 | Enhancement | GPS/GPS-Mate Stack | Completed | Added VIFLY GPS-Mate, improved GPS elevation |
| MOD-002 | Nov 15, 2025 | Replacement | VTX System | In Progress | Changed from Walksnail Moonlight to HDZero Freestyle V2 |

**Total Modifications**: 2
**Current Configuration**: Original Build Spec + GPS Stack Enhancement + HDZero VTX

---

## Modification Categories

- **Emergency Repair**: Forced by damage/incident
- **Upgrade**: Performance or reliability improvement
- **Enhancement**: New capability addition
- **Replacement**: Like-for-like part swap

---

## Modifications

### MOD-001 - Custom 3D Printed GPS/GPS-Mate Stack

**Date Proposed**: November 2025
**Date Implemented**: November 2025
**Category**: Enhancement
**Status**: Completed (ready for installation)

#### Original Configuration

| Component | Part Number | Specification |
|-----------|-------------|---------------|
| GPS | GEPRC M10-DQ | GPS/GNSS with DPS310 baro, front mount elevated 8mm+ |
| GPS-Mate | N/A | Not included in original build |
| GPS Mount | N/A | Standard elevation mount |

#### Modified Configuration

| Component | Part Number | Specification |
|-----------|-------------|---------------|
| GPS | GEPRC M10-DQ | GPS/GNSS with DPS310 baro, mounted on custom stack |
| GPS-Mate | VIFLY GPS-Mate | Lost-model finder, integrated into stack |
| GPS Mount | Custom 3D Printed (TPU) | Modular vertical stack design |

#### Rationale

**Technical Justification**:
- Elevates GPS module higher for improved signal reception and reduced interference from carbon fiber frame
- Integrates VIFLY GPS-Mate lost-model finder for aircraft recovery capability
- Modular design allows easy servicing/replacement of individual components
- TPU material provides vibration damping and impact resistance

**Performance Impact**:
- Expected: Better GPS lock performance with increased elevation
- Expected: Aircraft recovery capability via GPS-Mate beacon
- Expected: Reduced vibration-induced GPS noise

**Operator Notes**:
Lost-model recovery is critical for a small 3.5" platform that could be difficult to visually locate. Custom integrated stack solution is more elegant than separate mounting solutions.

#### Parts Required

| Part | Vendor | Order Date | Cost | Status |
|------|--------|------------|------|--------|
| VIFLY GPS-Mate | TBD | TBD | TBD | ✓ Acquired |
| TPU Filament | TBD | TBD | TBD | ✓ Used |
| Custom 3D Printed Parts | In-house design/print | Nov 2025 | Material cost only | ✓ Completed |

#### Implementation Notes

**Design Date**: November 2025
**Print Date**: November 2025
**Wiring Completed**: November 2025
**Installation Status**: Ready for installation (not yet mounted to aircraft)
**Designed/Built By**: SpyD

**Design Features**:
- Yellow TPU construction for visibility and flexibility
- Modular vertical stack configuration
- GPS module on top ("ANTENNA THIS SIDE UP" orientation)
- VIFLY GPS-Mate in middle section
- Both components pre-wired with harnesses ready for FC connection
- Integrated mounting points for frame installation

**Notes**:
Assembly has been fabricated, wired, and tested off-aircraft. Ready to install when frame wiring phase continues. See reference photo: `Documentation/reference/build-images/GPS_Stack.jpg`

#### Post-Modification Performance

**Test Flight Date**: TBD (aircraft not yet airworthy)
**Test Results**: TBD

**Expected vs Actual**: TBD after flight testing

#### Related Documents

- Incident: N/A
- Timeline: Updated in RD-54_Build_Timeline.md
- Parts List: Updated in RD-54_AsBuilt_Parts_List.md
- Reference Photo: `Documentation/reference/build-images/GPS_Stack.jpg`

---

### MOD-002 - VTX System Technology Change (Walksnail → HDZero)

**Date Proposed**: November 15, 2025
**Date Implemented**: In Progress
**Category**: Replacement
**Status**: In Progress

#### Original Configuration

| Component | Part Number | Specification |
|-----------|-------------|---------------|
| VTX | Walksnail Moonlight | Digital HD VTX, large footprint kit, JST-SH 4-pin power, LHCP pigtails |
| Camera | Walksnail Moonlight Camera | Integrated with VTX kit |
| Antennas | LHCP (included with kit) | Left-hand circular polarization |

#### Modified Configuration

| Component | Part Number | Specification |
|-----------|-------------|---------------|
| VTX | HDZero Freestyle V2 | Digital HD VTX (specifications TBD) |
| Camera | HDZero Freestyle V2 Camera | Integrated with VTX |
| Antennas | TBD | TBD |

#### Rationale

**Technical Justification**:
- Both systems are digital HD - technology swap with similar capabilities
- HDZero Freestyle V2 became available from mapping mission
- Installation ramifications similar between both digital systems
- Allows RD-54 to proceed while RD-59 timeline shifted

**Performance Impact**:
- Expected: Similar HD digital video performance
- Expected: Comparable latency and range characteristics
- Expected: Similar installation footprint and wiring requirements

**Operator Notes**:
RD-59 project timeline changed and won't be airworthy for a while. HDZero Freestyle V2 showed up from yesterday's mapping mission, making it available for RD-54 instead. Since both are digital systems, the install approach should be comparable.

#### Parts Required

| Part | Vendor | Order Date | Cost | Status |
|------|--------|------------|------|--------|
| HDZero Freestyle V2 VTX/Camera | From mapping mission | N/A | N/A | ✓ Available |
| Walksnail Moonlight (original) | - | May 17, 2025 | - | ⏳ Reassigned to other aircraft |

#### Installation Procedure

- [ ] Design and print any required camera/VTX mounts
- [ ] Mount HDZero Freestyle V2 VTX to frame
- [ ] Mount HDZero camera
- [ ] Wire VTX power to FC (verify voltage requirements)
- [ ] Wire VTX data connections (if applicable)
- [ ] Route antenna(s)
- [ ] Bench test video system
- [ ] Flight test video quality

#### Implementation Notes

**Installation Date**: TBD (in progress)
**Installed By**: SpyD

**Notes**:
Modification identified on November 15, 2025 after arm covers were completed. HDZero system will be installed after antenna mounts are designed/printed and ExpressLRS receiver is installed.

#### Post-Modification Performance

**Test Flight Date**: TBD
**Test Results**: TBD

**Expected vs Actual**: TBD

#### Related Documents

- Incident: N/A
- Timeline: Updated in RD-54_Build_Timeline.md (November 15, 2025)
- Parts List: Updated in RD-54_AsBuilt_Parts_List.md

---

## Modification Template

When documenting a modification, use this template:

### MOD-XXX - [Brief Description]

**Date Proposed**: [Date]
**Date Implemented**: [Date]
**Category**: [Emergency Repair / Upgrade / Enhancement / Replacement]
**Status**: [Proposed / In Progress / Completed / Abandoned]

#### Original Configuration

| Component | Part Number | Specification |
|-----------|-------------|---------------|
| | | |

#### Modified Configuration

| Component | Part Number | Specification |
|-----------|-------------|---------------|
| | | |

#### Rationale

**Technical Justification**:
[Why this modification is being made]

**Performance Impact**:
[Expected performance changes]

**Operator Notes**:
[Operator's reasoning/decision factors]

#### Parts Required

| Part | Vendor | Order Date | Cost | Status |
|------|--------|------------|------|--------|
| | | | | |

#### Installation Procedure

- [ ] [Step 1]
- [ ] [Step 2]
- [ ] [Bench test]
- [ ] [Flight test]

#### Implementation Notes

**Installation Date**: [Date]
**Installed By**: SpyD

**Notes**:
[Any installation observations]

#### Post-Modification Performance

**Test Flight Date**: [Date]
**Test Results**:
[Performance observations]

**Expected vs Actual**:
[Did it meet expectations?]

#### Related Documents

- Incident: [Link to incident if applicable]
- Timeline: [Link to timeline entry]
- Parts List: [Updated in RD-54_AsBuilt_Parts_List.md]

---

**Document Version**: 1.0
**Archivist**: Claude Code, RD-54 SME
