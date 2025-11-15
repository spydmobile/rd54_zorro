# RD-54 "Zorro" - Build Timeline

**Aircraft Designator**: RD-54 (Code Name: Zorro)
**Operator**: SpyD (Franco Nogarin)
**Last Updated**: November 14, 2025

---

## Project Overview

**Platform**: 3.5" Digital FPV Cruiser
**Primary Mission**: Exploration and cinematic FPV flights with HD digital video
**Build Philosophy**: Reliable mini platform optimized for smooth cruising and GPS-assisted flights
**Key Features**: Walksnail HD digital FPV, GPS Rescue/RTH, ExpressLRS long range, lost model recovery

---

## Timeline

### Phase 1: Planning & Parts Procurement

#### May 17, 2025 - Parts Ordered
**Status**: ✓ Completed

Initial parts order placed for complete build:
- FlyFishRC Volador VX3.5 frame
- SpeedyBee F405 AIO 40A FC/ESC
- Emax ECO II 2004 3000KV motors (x4)
- Gemfan Hurricane 3525-3 props
- Walksnail Moonlight VTX kit
- HappyModel ExpressLRS EP1 receiver
- GEPRC M10-DQ GPS/GNSS module
- 5V buzzer
- 2x GNB 880mAh 6S HV 160C XT30 batteries

**Lead Time**: ~9 days

---

### Phase 2: Initial Build

#### May 26, 2025 - Build Started
**Status**: 🔨 In Progress

Build activities commenced. Initial assembly phase.

**Completed Activities**:
- ✓ Frame assembled
- ✓ FC/ESC stack installed and positioned
- ✓ All 4 motors mounted to frame
- ✓ All 4 motors wired to AIO (completed Nov 14, 2025)
- ✓ Solder pads cleaned with alcohol

**In Progress**:
- ⚠️ VTX/Camera installation (next major task)

**Pending Installation**:
- ⏳ ExpressLRS receiver (EP1 available)
- ⏳ Buzzer
- ⏳ Antenna routing
- ⏳ Wire management
- ⏳ GPS stack (fabricated, wired, will be installed last)
- ⏳ Top plate installation

#### November 2025 - MOD-001: Custom GPS Stack
**Status**: ✓ Completed (ready for installation)

Custom 3D printed TPU GPS/GPS-Mate stack designed and fabricated:
- Yellow TPU modular stack design
- Integrates GEPRC M10-DQ GPS module
- Adds VIFLY GPS-Mate lost-model finder
- Both components wired and ready for installation
- Provides improved GPS elevation for better signal reception

**Rationale**: Lost-model recovery critical for small 3.5" platform. Custom integrated solution more elegant than separate mounts.

#### November 14, 2025 - Motor Wiring Completed
**Status**: ✓ Major Milestone Completed

All 4 motors successfully wired to SpeedyBee AIO:
- Motor soldering completed (4 of 4)
- Solder pads cleaned with alcohol for clean connections
- FC/ESC stack positioned and mounted
- Ready for VTX/Camera installation (next major component)

**Status as of November 14, 2025**: Assembly phase ~70% complete. Core structure complete, all motors wired, FC/ESC mounted. Remaining work: install VTX/Camera, receiver, buzzer, GPS stack (last), wire management, top plate.

---

### Phase 3: Configuration & Testing

**Status**: ⏳ Pending

Planned activities:
- [ ] Betaflight configuration
- [ ] ExpressLRS binding
- [ ] GPS setup
- [ ] Walksnail VTX configuration
- [ ] Initial power-up testing
- [ ] Bench testing
- [ ] Motor direction verification
- [ ] Pre-flight checks

**Estimated Start**: TBD

---

### Phase 4: First Flight & Tuning

**Status**: ⏳ Pending

Planned activities:
- [ ] Maiden flight
- [ ] Initial PID tuning
- [ ] Rates configuration
- [ ] Performance evaluation
- [ ] Video system testing

**Estimated Start**: TBD

---

## Build Statistics

**Project Duration** (as of Nov 14, 2025):
- Days since parts ordered: 181 days
- Days since build started: 172 days
- Current phase: Initial Build (Assembly Phase)
- Completion: ~70% (estimated)

**Time Allocation**:
- Planning & procurement: 9 days (completed)
- Build in progress: 172+ days (ongoing)
- Configuration: Pending
- Testing: Pending

**Progress Breakdown**:
- Frame/structure: 100%
- Motor mounting: 100%
- Motor wiring: 100% (all 4 complete - Nov 14)
- Electronics installation: 30% (FC/ESC mounted, VTX/RX/buzzer pending)
- Custom modifications: 100% (GPS stack fabricated, ready to install)
- Configuration: 0%
- Testing: 0%

---

## Key Milestones

| Date | Milestone | Status |
|------|-----------|--------|
| May 17, 2025 | Parts ordered | ✓ Completed |
| May 26, 2025 | Build commenced | ✓ Completed |
| May 26 - Nov 2025 | Frame assembled | ✓ Completed |
| May 26 - Nov 2025 | Motors mounted (all 4) | ✓ Completed |
| May 26 - Nov 2025 | FC/ESC installed | ✓ Completed |
| November 2025 | MOD-001: Custom GPS stack fabricated | ✓ Completed |
| November 14, 2025 | Motor wiring completed (all 4) | ✓ Completed |
| TBD | VTX/Camera installed | ⏳ In Progress (next major task) |
| TBD | Receiver installed | ⏳ Pending |
| TBD | Buzzer installed | ⏳ Pending |
| TBD | GPS stack mounted to aircraft | ⏳ Pending (final component) |
| TBD | Assembly completed | ⏳ Pending |
| TBD | Configuration completed | ⏳ Pending |
| TBD | Maiden flight | ⏳ Pending |
| TBD | Tuning completed | ⏳ Pending |
| TBD | Operational status | ⏳ Pending |

---

## Lessons Learned

### Build Phase Lessons

**Custom Parts Development**:
- 3D printed TPU parts provide flexible, vibration-resistant mounting solutions
- Modular design philosophy allows easy component servicing
- Yellow color improves visibility for small components

**Component Sourcing**:
- Original ExpressLRS EP1 diverted to other aircraft mid-build
- Having second EP1 available resolved receiver shortage
- Planning for spare critical components valuable for multi-aircraft operation

**Build Approach**:
- Methodical 172-day build timeline reflects quality-over-speed philosophy
- Taking time to design custom solutions (GPS stack) better than rushing with off-the-shelf compromises
- Extended timeline allows for thoughtful engineering decisions

---

## Future Activities

### Immediate (Next Steps)
- [ ] Complete motor wiring (solder remaining 2 motors to AIO)
- [ ] Install Walksnail Moonlight VTX/Camera system
- [ ] Install ExpressLRS EP1 receiver
- [ ] Install 5V buzzer
- [ ] Mount GPS/GPS-Mate stack to frame
- [ ] Wire management and cleanup

### Short Term (Pre-flight)
- [ ] Initial Betaflight configuration
  - [ ] Motor direction verification
  - [ ] Receiver binding (ExpressLRS)
  - [ ] GPS configuration
  - [ ] Walksnail VTX setup
  - [ ] Buzzer testing
- [ ] Bench testing
  - [ ] Power-up tests
  - [ ] Failsafe configuration
  - [ ] Arming tests
- [ ] Pre-flight safety checks

### Medium Term (Initial Flight Operations)
- [ ] Maiden flight (LOS hover test)
- [ ] Initial PID tuning
- [ ] Rates configuration
- [ ] FPV system validation
- [ ] GPS-Mate functionality test
- [ ] Performance evaluation

### Long Term (Cruiser Operations)
- [ ] Optimize for smooth cruising flight
  - [ ] Tune rates for cinematic flying (smooth, not aggressive)
  - [ ] Optimize PID for stability (minimize oscillations in video)
  - [ ] Test GPS Rescue and Return Home functionality
- [ ] Extended range testing
  - [ ] Test ExpressLRS range with GPS failsafes
  - [ ] Validate GPS-Mate recovery beacon effectiveness
- [ ] Video quality optimization
  - [ ] Walksnail recording settings for best quality
  - [ ] Test different cruising speeds for stable footage
  - [ ] Vibration reduction if needed
- [ ] Explore interesting locations
  - [ ] Identify cruising spots (parks, trails, scenic areas)
  - [ ] Build exploration flight repertoire
  - [ ] Capture cinematic HD footage

---

## Notes

**Build Duration Context**:
Extended build timeline (172+ days) suggests this is a careful, methodical build process rather than rushed construction. Quality over speed approach.

**Platform Evolution**:
Originally planned as 3.5" freestyle platform. Mission refined to **Digital FPV Cruiser** - optimized for smooth exploration flights with HD digital video capture via Walksnail Moonlight. GPS stack (MOD-001) enables GPS Rescue, Return Home, and lost model recovery for extended cruising missions.

**ArduPilot Mapping Platform**:
Considered converting RD-54 to autonomous mapping platform (see `Documentation/reference/ardupilot-mapping-drone-project.md`), but 3.5" size and limited flight time (~5-10 min with camera payload) make it unsuitable for practical mapping work. Decision: Keep RD-54 as Betaflight digital FPV cruiser. Future dedicated mapping platform would be 5"+ with H7 FC and larger batteries.

---

**Document Version**: 2.0 (Updated November 14, 2025)
**Archivist**: Claude Code, RD-54 SME
