# RD-54 "Zorro" - Build Timeline

**Aircraft Designator**: RD-54 (Code Name: Zorro)
**Operator**: SpyD (Franco Nogarin)
**Last Updated**: November 15, 2025

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

#### November 15, 2025 - MOD-002: VTX System Change & Custom Arm Covers
**Status**: ✓ Arm Covers V4 & V5 Completed / ⚠️ VTX Change In Progress

**Custom Arm Covers V4 Completed**:
- Custom 3D printed TPU arm covers designed and fabricated (V0-V4 iteration)
- Remixed from Chimera motor wire shield design (90mm)
- Material: Bambu TPU for AMS on X1C printer
- All 4 arms fitted with V4 design
- Design iterations: V0 (original remix) through V4 (final fit)

**V5 Antenna Clip Development - Completed**:
- Goal: Integrate antenna clips into rear arm covers for EP1 dual T-antennas
- Design approach: Solid block with dual-cylinder negative hole for snap-fit retention
- Iteration process: V1.1/V1.2/V1.3 initial variants → V2.0 winner
- **V2.0 Design Changes**: Bigger body with slot for T-leg (V1.x dual-cylinder approach insufficient)
- Print settings: 0.12mm HQ layer height (improved layer bonding for snap-in/out forces parallel to layers)
- Integration method: Added shim so clip attaches to one side of arm cover only, then fused V2.0 clip geometry
- Retention performance: Strong hold - antennas won't come out unless serious crash
- Final configuration: 2 rear arms with V5 (integrated clips installed), 2 front arms remain V4
- Additional protection planned for underside
- Reference photos:
  - Prototype variants: `Documentation/reference/screengrabs/Screenshot 2025-11-15 at 8.22.51 AM.png`
  - V5 installed: `Documentation/reference/build-images/IMG_5638_arm_cover_V5_bottom.jpg`

**VTX System Technology Change**:
- Original plan: Walksnail Moonlight (digital HD)
- New plan: HDZero Freestyle V2 (digital HD)
- Reason: RD-59 project timeline changed, HDZero Freestyle V2 became available from mapping mission
- Both digital systems, install ramifications similar
- See MOD-002 in Modifications Log for details

#### November 15, 2025 - Custom Parts Batch Fabrication & Installation
**Status**: ⚠️ In Progress (multiple iterations ongoing)

**Parts Printing** (Bambu TPU, 0.12mm HQ for strength and visual quality):
- **HDZero VTX Antenna Holder**: Rear-mounted antenna holder
  - Source: https://makerworld.com/en/models/1769720-flyfishrc-volador-vx3-antenna-mount
  - Designer: FlyFishRC Volador VX3 Antenna Mount (MakerWorld)
- **EP1 RX Holder**: Underside frame-mount for HappyModel EP1 receiver
  - Remixed by operator (removed built-in supports that didn't work well)
  - Original source: TBD
- **XT60 Mount**: Battery connector holder, mounts to rear standoffs beneath top plate for easier LiPo plugging
  - Source: https://makerworld.com/en/models/1203681-volador-vx3-5-xt30-mount
  - Note: Originally designed for XT30, being used for XT60

**Custom Feet - Redesigned for Ground Clearance** (✓ Completed):
- **Design Approach**: Remixed factory arm guards, doubled foot height for 4-5mm additional clearance
  - Source: Factory FlyFishRC Volador VX3/VX3.5 TPU parts (6052757)
  - Design: Screw-mounted style, ~15mm motor mount clearance from ground
- **Initial Configuration**:
  - 2 rear tall feet (screw-on, 15mm clearance)
  - 2 front shorter feet (slip-on, 11-12mm clearance)
  - Result: Uneven stance (1mm front / 20mm rear differential)
- **Final Configuration** (✓ Upgraded and Installed):
  - **All 4 feet now tall and screw-mounted** (~15mm clearance)
  - Even stance achieved - consistent ground clearance all around
  - All screw-mounted for secure attachment
- **Future Plans**:
  - Eventually print smarter front bumper design (+3-5mm for even more balanced stance)
- **Benefit**: Tall feet provide clearance for underside components (antenna mount, RX holder)
- **Reference**: `Documentation/reference/build-images/IMG_5646_tall_rear_foot.jpg`

**EP1 RX Holder - Iterative Development** (✓ V6 Success):
- **Iteration History**: V1-V5 attempts (various approaches didn't work as hoped)
- **V6 Design** (✓ Installed and Working):
  - Base: MakerWorld ELRS EP1 Dual Mount design (`custom_3d_printed_parts/RX mount/ELRS+TCXO+EP1+DUAL+MOUNT+V1.stl`)
  - Modifications: Removed original mount flanges, kept simple holder
  - Added: Factory mounting flanges from FlyFishRC Antenna-Mount.stl
  - File: `custom_3d_printed_parts/RX mount/Dual EP1 ELRS RX Mount for FlyfishRD Volaror 3.5 V6.stl`
  - **Result**: Works as planned, receiver holder successfully mounted to underside frame
- **Lesson**: Persistence pays off - 6 iterations to find working design combination

**Side Panels (Stack Protectors)** (✓ Printed and Installed):
- **Status**: Reprinted with correct "RD-54 ZORRO" designation (original had "RD-54 Bandit" typo)
- **Source**: Remixed from https://than.gs/m/1260429
- **Embossing Quality**: Decent - visible and readable, minor cleanup needed on lettering
- **Installation**: Installed and protecting FC/ESC stack from side impacts
- **Reference**: `Documentation/reference/build-images/IMG_5647_stack_cover.jpg`

**Print Settings Rationale**:
- 0.12mm HQ layer height provides both structural strength and improved visual appearance
- Yellow TPU maintains visibility and crash protection consistency

#### November 15, 2025 - HDZero VTX Test Fit & Full Assembly Mockup
**Status**: ✓ Validation Complete

**VTX Test Fit**:
- HDZero Freestyle V2 test fitted to frame
- **Clearance check**: All clearances validated, no interference with side panels or other components
- **Mounting method**: Will use included 3M tape for VTX attachment
- **Camera position**: Front-mounted in aluminum cage (mini bando style for close-quarters flying)
- Camera positioned under GPS stack at front of frame
- **Result**: Fit confirmed, ready for installation

**Full Assembly Mockup**:
- Purpose: Validate custom parts compatibility and plan final assembly
- Components mocked up:
  - GNB 6S battery positioned on top
  - GPS stack placement visualized
  - All yellow TPU custom parts installed
  - Green props mounted for visual reference
- **Validation goals**:
  - Confirm no collisions between custom parts
  - Visualize GPS stack wire routing
  - Plan front bumper redesign (may incorporate adjustable camera mount)
- **Issues discovered**: None yet
- **Next steps**: Front bumper assembly redesign with possible adjustable camera mount integration

**Power Requirement Discovery**:
- **Issue**: 6S HV battery (22.2V nominal) exceeds HDZero VTX voltage tolerance
- **Requirement**: HDZero requires 9V regulated power
- **Solution**: External BEC module (included with SpeedyBee FC package)
  - Specs: Switchable 5V/9V/12V output, current rating TBD
  - **Current Status**: BEC currently configured for 5V output
  - **Required Action**: Modify BEC configuration from 5V to 9V
  - Power path: VBAT → 9V BEC → HDZero VTX
  - Mounting location: TBD
- **Importance**: Discovered during test fit phase - would have caused issues if found during final installation

**EP1 Receiver Preparation Required**:
- **Status**: EP1 receiver available, RX holder V6 installed and ready
- **Required Before Installation**: Apply heat shrink to EP1 receiver
- **Then**: Install heat-shrinked receiver into mounted holder
- **Antennas**: Dual T-antennas ready to mount in V5 arm cover clips after receiver installation

**GPS Wiring Harness Design** (⚠️ In Progress):
- **Purpose**: Custom harness to connect GPS, GPS-Mate, and FC
- **Approach**: Splice individual wiring harnesses together
- **Connectors**: JST connectors from each component (GPS, GPS-Mate, FC)
- **Status**: Currently designing and fabricating custom splice harness

**References**:
- VTX test fit: `Documentation/reference/build-images/IMG_5648_test_fit_VTX.jpg`
- Full mockup: `Documentation/reference/build-images/IMG_5649_inspirational_mockup.jpg`

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
| November 15, 2025 | Custom arm covers V4 installed (front arms) | ✓ Completed |
| November 15, 2025 | MOD-002: VTX change (Walksnail → HDZero) | ⚠️ In Progress |
| November 15, 2025 | V5 antenna clip prototyping (V1.1/V1.2/V1.3 → V2.0) | ✓ Completed |
| November 15, 2025 | V5 rear arm covers with V2.0 clips installed | ✓ Completed |
| November 15, 2025 | Custom feet redesigned and installed (initial: 2 tall rear, 2 short front) | ✓ Completed |
| November 15, 2025 | Side panels with RD-54 Zorro designation printed and installed | ✓ Completed |
| November 15, 2025 | HDZero VTX test fit and full assembly mockup | ✓ Completed |
| November 15, 2025 | EP1 RX holder V6 printed, installed, and working | ✓ Completed |
| November 15, 2025 | All 4 feet upgraded to tall screw-mounted configuration | ✓ Completed |
| November 15, 2025 | HDZero antenna holder and XT60 mount printed | ✓ Completed |
| TBD | BEC modification (5V → 9V configuration change) | ⏳ Pending |
| TBD | EP1 receiver heat shrink and installation | ⏳ Pending |
| TBD | HDZero antenna holder installation | ⏳ Pending |
| TBD | XT60 mount installation | ⏳ Pending |
| TBD | EP1 receiver installed | ⏳ Pending |
| TBD | HDZero VTX/Camera installed | ⏳ Pending |
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
- Iterative prototyping approach: Test critical features (snap-fit) independently before integrating into larger parts
- Layer orientation matters for TPU snap-fits: 0.12mm HQ layer height improves bonding when snap forces parallel to layer plane
- 0.12mm HQ also provides superior visual appearance (smoother surfaces) vs standard layer heights
- Prototype multiple variants simultaneously (V1.1/V1.2/V1.3) to accelerate fit testing
- Initial design assumptions may not work (V1.x dual-cylinder approach insufficient for T-antenna geometry)
- V2.0 breakthrough: Bigger body with slot for T-leg provided proper retention vs simple cylindrical holes
- Shim-mounting technique allows clip to attach to one side of arm cover for better integration
- Strong retention achieved: Antennas won't come out unless serious crash (validates V2.0 design)
- Pre-print review catches errors: Side panel typo (RD-54 Bandit vs Zorro) caught before wasting TPU and print time
- Remix approach accelerates development: Remove bad features (built-in supports) from existing designs vs starting from scratch
- Iterative design is normal: EP1 RX holder took V1-V5 attempts before finding working V6 combination
- Persistence validated: V6 RX holder works as planned after 5 failed attempts - don't give up on good ideas
- Hybrid approach works: Combining parts from different sources (MakerWorld holder + factory mounting flanges) can solve fitment issues
- Upgrade mid-build is fine: Switching from uneven stance (2 tall + 2 short feet) to all 4 tall for consistent clearance
- Ground clearance matters: Custom feet doubled height provides 4-5mm clearance for underside components (antenna mounts)
- Mixed mounting approaches: Screw-on (rear) vs slip-on (front) feet - can optimize per location
- Post-print cleanup: Embossed text may need minor cleanup but still readable and functional
- Mock-up validation critical: Full assembly dry-fit validates custom parts compatibility before final installation
- Test fit before commitment: VTX test fit confirms clearances and mounting approach (3M tape)
- Test fit reveals power requirements: HDZero VTX can't run directly from 6S HV battery - discovered before installation
- External BEC solution: 9V BEC (included with FC) solves voltage regulation issue for VTX
- Mini bando style: Front-mounted camera in aluminum cage optimized for close-quarters flying
- Plan ahead: Mockup helps visualize wire routing and identify future redesigns (front bumper with adjustable camera mount)
- Custom wiring harnesses: GPS/GPS-Mate/FC integration requires custom splice harness with JST connectors

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

**Updated November 15, 2025**:
- [x] Complete motor wiring (all 4 motors soldered - Nov 14, 2025)
- [x] Design and fabricate custom arm covers V4 for front arms (Nov 15, 2025)
- [x] Prototype V5 antenna clips (V1.1/V1.2/V1.3 → V2.0 winner - Nov 15, 2025)
- [x] Test snap-fit retention with actual EP1 T-antennas (V2.0 confirmed strong hold - Nov 15, 2025)
- [x] Integrate V2.0 clip design into V5 arm cover geometry (shim-mounted to one side - Nov 15, 2025)
- [x] Print and install V5 rear arm covers with integrated V2.0 clips (0.12mm HQ - Nov 15, 2025)
- [x] Design and print custom feet with doubled height for ground clearance (Nov 15, 2025)
- [x] Install custom feet (2 rear tall, 2 front shorter - uneven stance for now) (Nov 15, 2025)
- [x] Print and install side panels with correct RD-54 Zorro designation (Nov 15, 2025)
- [x] Test fit HDZero VTX and validate clearances (Nov 15, 2025)
- [x] Full assembly mockup to validate custom parts compatibility (Nov 15, 2025)
- [x] Iterate EP1 RX holder design (V1-V6, V6 successful - Nov 15, 2025)
- [x] Install EP1 RX holder V6 to underside frame (works as planned - Nov 15, 2025)
- [x] Print and install 2 more tall feet to replace front (all 4 now tall screw-mounted - Nov 15, 2025)
- [x] Print HDZero antenna holder and XT60 mount (0.12mm HQ TPU - Nov 15, 2025)
- [⚠️] Design GPS/GPS-Mate/FC custom wiring harness (splicing JST connectors - Nov 15, 2025)
- [ ] Fabricate GPS wiring harness (splice GPS, GPS-Mate, FC connections)
- [ ] Modify BEC from 5V to 9V configuration
- [ ] Determine 9V BEC mounting location and install
- [ ] Apply heat shrink to EP1 receiver
- [ ] Install heat-shrinked EP1 receiver into mounted holder
- [ ] Mount and route dual T-antennas to rear arm V5 clips
- [ ] Install HDZero antenna holder to rear mount
- [ ] Wire and install 9V BEC (VBAT → 9V BEC → HDZero VTX)
- [ ] Install HDZero Freestyle V2 VTX/Camera system with 9V power (see MOD-002)
- [ ] Install XT60 mount to rear standoffs beneath top plate
- [ ] Install 5V buzzer
- [ ] Eventually design/print improved front bumper (+3-5mm for even more balanced stance)
- [ ] Cleanup embossed lettering on side panels
- [ ] Wire management and cleanup
- [ ] Mount GPS/GPS-Mate stack to frame (planned as final component)
- [ ] Install top plate

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
