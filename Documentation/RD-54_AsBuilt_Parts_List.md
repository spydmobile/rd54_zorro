# RD-54 "Zorro" - As-Built Parts List

**Aircraft Designator**: RD-54 (Code Name: Zorro)
**Operator**: SpyD (Franco Nogarin)
**Platform Type**: 3.5" Digital FPV Cruiser
**Primary Mission**: Exploration and cinematic FPV flights with HD digital video
**Current Status**: Under Construction - Assembly Phase
**Airworthiness**: Not Yet Airworthy
**Last Updated**: November 15, 2025

---

## Mission Profile

**Digital FPV Cruiser** - Optimized for smooth exploration and HD video capture

**Primary Uses**:
- Cruising and exploring interesting locations
- Recording cinematic HD footage via Walksnail digital FPV
- GPS-assisted flights with Return Home and GPS Rescue
- Small form factor for flying in tighter spaces
- Lost model recovery capability (VIFLY GPS-Mate)

**Flight Characteristics**:
- Flight time: 8-12 minutes (cruising)
- Range: Extended with ExpressLRS long-range control
- Video system: Walksnail Moonlight HD digital FPV
- Safety: GPS features + lost model beacon

**NOT Designed For**:
- Racing (not optimized for speed)
- Aggressive freestyle (can do some, but not primary mission)
- Autonomous mapping (Betaflight, not ArduPilot)
- Heavy payload carrying

---

## Current Configuration

### Airframe

| Component | Part Number/Model | Quantity | Status | Notes |
|-----------|------------------|----------|---------|-------|
| **Frame** | FlyFishRC Volador VX3.5 | 1 | ✓ Assembled | X-config, 3.5" wheelbase |
| **Feet - All 4** | Custom 3D Printed (TPU) | 4 | ✓ Installed | Tall screw-mounted style, doubled height, ~15mm ground clearance, even stance, remixed from factory parts (6052757) |
| **Arm Covers - Front** | Custom 3D Printed (TPU) | 2 | ✓ V4 Installed | Bambu TPU, V4 design, remixed from Chimera 90mm |
| **Arm Covers - Rear** | Custom 3D Printed (TPU) | 2 | ✓ V5 Installed | Bambu TPU, 0.12mm HQ, V5 with integrated V2.0 antenna clips |
| **Antenna Clips** | Integrated into V5 Rear Covers | 2 | ✓ Installed | V2.0 design: bigger body with T-leg slot, strong retention, shim-mounted to one side |
| **Side Panels (Stack Protectors)** | Custom 3D Printed (TPU) | 2 | ✓ Installed | "RD-54 ZORRO" embossed, FC/ESC protection, remixed from than.gs/m/1260429, minor cleanup needed |
| **EP1 RX Holder** | Custom 3D Printed (TPU) | 1 | ✓ Installed | V6 design successful: MakerWorld holder + factory mounting flanges, underside mount, 0.12mm HQ, works as planned |
| **HDZero Antenna Holder** | Custom 3D Printed (TPU) | 1 | ✓ Printed | Bambu TPU, 0.12mm HQ, rear mount, source: makerworld.com/en/models/1769720, not yet installed |
| **XT60 Mount** | Custom 3D Printed (TPU) | 1 | ✓ Printed | Bambu TPU, 0.12mm HQ, rear standoff mount, source: makerworld.com/en/models/1203681 (XT30 design used for XT60), not yet installed |
| **GPS Mount** | Custom 3D Printed (TPU) | 1 | ✓ Fabricated (ready to install) | Yellow TPU, modular stack design - see MOD-001 |

---

### Flight Control & Power

| Component | Part Number/Model | Quantity | Status | Notes |
|-----------|------------------|----------|---------|-------|
| **FC/ESC Stack** | SpeedyBee F405 AIO 40A BlueJay | 1 | ✓ Installed and wired | 3-6S rating, integrated 40A ESC |
| **Motors** | Emax ECO II 2004 3000KV | 4 | ✓ Mounted and wired | All 4 motors soldered to AIO (completed Nov 14, 2025) |
| **Propellers** | Gemfan Hurricane 3525-3 Tri-Blade | 2 CW + 2 CCW | ✓ Available | Bright green installed for assembly photos |

---

### Power System

| Component | Part Number/Model | Quantity | Status | Notes |
|-----------|------------------|----------|---------|-------|
| **Battery #1** | GNB 880mAh 6S HV 160C XT30 | 1 | ✓ Available | GNB8806S160AHV |
| **Battery #2** | GNB 880mAh 6S HV 160C XT30 | 1 | ✓ Available | GNB8806S160AHV |
| **Connector Type** | XT30 | - | ✓ Installed | Battery/aircraft interface on FC |
| **9V BEC** | External BEC Module (included with FC) | 1 | ✓ Configured | Modified to 9V output (soldered jumper per SpeedyBee instructions), tested at 9V, ready for VTX installation, will be mounted inline with VTX power cable under top plate |

---

### Video System

| Component | Part Number/Model | Quantity | Status | Notes |
|-----------|------------------|----------|---------|-------|
| **VTX** | HDZero Freestyle V2 | 1 | ✓ Test Fit Complete | Digital HD VTX, 3M tape mounting, clearances validated - see MOD-002 |
| **Camera** | HDZero Freestyle V2 Camera | 1 | ✓ Test Fit Complete | Front-mounted in aluminum cage (mini bando style for close-quarters flying) |
| **Original VTX** | ~~Walksnail Moonlight~~ | 1 | ⏳ Reassigned | Replaced by HDZero per MOD-002 |

---

### Radio System

| Component | Part Number/Model | Quantity | Status | Notes |
|-----------|------------------|----------|---------|-------|
| **Receiver** | HappyModel ExpressLRS EP1 Dual-TCXO | 1 | ⚠️ Needs Heat Shrink | Available, needs heat shrink before installation into mounted holder |
| **RX Antennas** | HappyModel EP1 Dual T-Antennas | 2 | ✓ Available (not installed) | ELRS antennas, ready to mount in V5 arm cover clips |

---

### Navigation & Sensors

| Component | Part Number/Model | Quantity | Status | Notes |
|-----------|------------------|----------|---------|-------|
| **GPS/GNSS** | GEPRC M10-DQ | 1 | ✓ Wired (ready to install) | With DPS310 barometer, integrated into custom GPS stack (MOD-001), drone-side harness complete |
| **GPS-Mate** | VIFLY GPS-Mate | 1 | ✓ Wired (ready to install) | Lost-model finder beacon, integrated into custom GPS stack (MOD-001), drone-side harness complete |
| **GPS Wiring Harness** | Custom FC→GPS-Mate Harness | 1 | ✓ Fabricated | 5-pin JST (GND/TX/RX/5V/BZ-) + 2 I2C solder wires (SDA white, SCL blue), see MOD-001 for install procedure |

---

### Auxiliary Systems

| Component | Part Number/Model | Quantity | Status | Notes |
|-----------|------------------|----------|---------|-------|
| **Buzzer** | Integrated in GPS-Mate | 1 | ✓ Wired | FC buzzer contacts wired to GPS-Mate BZ- (yellow wire in 5-pin JST), external buzzer not needed |

---

## Build History

### Initial Build (May 2025 - Present)

**Parts Ordered**: May 17, 2025
**Build Start**: May 26, 2025
**Build Status**: Assembly Phase - In Progress

**Current Progress**:
- ✓ Frame assembled
- ✓ Motors mounted to frame (all 4)
- ✓ All motors wired to AIO (4 of 4 complete - Nov 14, 2025)
- ✓ FC/ESC stack installed and positioned
- ✓ All 4 custom feet installed - tall screw-mounted configuration, even stance at ~15mm clearance (Nov 15, 2025)
- ✓ Custom arm covers installed (V4 on front arms, V5 with antenna clips on rear arms - Nov 15, 2025)
- ✓ Side panels (stack protectors) installed with RD-54 Zorro designation (Nov 15, 2025)
- ✓ EP1 RX holder V6 installed and working - mounted to underside frame (Nov 15, 2025)
- ✓ Custom GPS stack fabricated and wired (ready for installation - will be installed last)
- ✓ HDZero VTX/Camera test fit completed - clearances validated (Nov 15, 2025)
- ✓ Full assembly mockup validated - no collisions, wire routing visualized (Nov 15, 2025)
- ✓ Power requirement discovered - 6S HV too high for HDZero, 9V BEC solution identified (Nov 15, 2025)
- ✓ HDZero antenna holder printed (Nov 15, 2025)
- ✓ XT60 mount printed (Nov 15, 2025)
- ✓ GPS/GPS-Mate/FC custom wiring harness fabricated (Nov 19, 2025) - 5-pin JST + I2C solder wires
- ✓ BEC modified to 9V configuration (Nov 19, 2025) - soldered jumper, voltage tested and confirmed
- ⚠️ EP1 receiver needs heat shrink before installation
- ⏳ HDZero antenna holder installation (printed, ready to install)
- ⏳ XT60 mount installation (printed, ready to install)
- ⏳ 9V BEC mounting and wiring (modified to 9V ✓, will mount inline with VTX power cable, custom mount planned)
- ⏳ EP1 heat shrink and installation into mounted holder
- ⏳ HDZero VTX/Camera installation (test fit complete, awaiting 9V BEC and antenna holder)
- ⏳ Antennas ready to mount (clips installed, awaiting receiver installation)
- ✓ Buzzer integrated via GPS-Mate (FC buzzer pads wired to GPS-Mate BZ-)
- ⏳ GPS stack mounting (planned as final component)
- ⏳ Betaflight configuration not started
- ⏳ Radio binding not started

**Modifications from Original Spec**:
- **MOD-001**: Custom 3D printed TPU GPS/GPS-Mate stack (November 2025)
  - Added VIFLY GPS-Mate for lost-model recovery
  - Custom modular stack design for improved GPS elevation
  - See `RD-54_Modifications_Log.md` for details
- **MOD-002**: VTX system change (November 15, 2025)
  - Changed from Walksnail Moonlight to HDZero Freestyle V2
  - Both digital HD systems, similar install approach
  - RD-59 timeline shift made HDZero available from mapping mission
  - See `RD-54_Modifications_Log.md` for details

---

## Pending Upgrades/Changes

**Immediate Next Steps** (as of November 19, 2025):
- Modify BEC from 5V to 9V configuration
- Install HappyModel EP1 receiver (heat shrink first)
- Mount and route dual T-antennas to rear arm V5 clips
- Install HDZero Freestyle V2 VTX/Camera system (requires 9V BEC)
- Install HDZero antenna holder and XT60 mount
- Design/print additional underside protection (antenna clips need crash protection)
- Wire management and routing
- Mount GPS stack to frame (planned as final component)
- Install top plate
- Initial Betaflight configuration

---

## Known Issues

**Current Blockers**:
- VTX/Camera not installed (required for FPV operation) - BEC ready ✓
- Receiver not installed (required for control)
- No configuration or testing completed yet

**Recent Progress** (November 14, 2025):
- ✓ Motor wiring completed (all 4 motors soldered to AIO)
- ✓ FC/ESC stack positioned and mounted
- ✓ Solder pads cleaned with alcohol for clean connections

**Component Status**:
- Original ExpressLRS EP1 diverted to another aircraft (resolved - second EP1 located)

---

## Notes

- **Mission Focus**: Digital FPV Cruiser with Mini Bando style - smooth exploration and close-quarters flying with HD video
- **Video System**: HDZero Freestyle V2 digital HD FPV (changed from Walksnail per MOD-002)
- **Camera Setup**: Front-mounted in aluminum cage (mini bando style for close-quarters navigation and proximity flying)
- **Power Solution**: 9V BEC required for HDZero VTX (6S HV battery voltage too high for direct connection)
- **BEC Configuration**: External BEC modified to 9V output (soldered jumper per SpeedyBee instructions, tested and confirmed 9V)
- **BEC Mounting**: Inline with VTX power cable under top plate (custom 3D printed mount planned)
- **Power Path**: 6S HV Battery → VBAT → 9V BEC → HDZero VTX
- **Custom Parts**: TPU arm covers - V4 on front arms, V5 with integrated V2.0 antenna clips on rear arms (0.12mm HQ print)
- **Ground Clearance**: All 4 feet tall and screw-mounted at ~15mm clearance (initially 2 tall/2 short, upgraded for even stance)
- **RX Holder Success**: V6 design works as planned after 5 iterations (underside mount with hybrid design approach)
- **Antenna Retention**: V2.0 clips with T-leg slot design provide strong hold, won't release unless serious crash
- **Mounting Method**: HDZero VTX uses included 3M tape mounting (test fit validated, no clearance issues)
- **Custom Wiring**: GPS/GPS-Mate/FC require custom splice harness (JST connectors from each component)
- **GPS Mounting**: Custom TPU stack provides elevation and integrates VIFLY GPS-Mate (MOD-001)
- **Buzzer Integration**: GPS-Mate provides all buzzer functionality via FC buzzer pads (BZ- yellow wire), no external buzzer needed
- **3D Print Sources**: Mix of remixed designs (arm covers, side panels, RX holder) and community models from MakerWorld/Thangs
- **XT60 Adaptation**: Using XT30 mount design for XT60 connector (compatible mounting pattern)
- **GPS Features**: Enables GPS Rescue, Return Home, and position hold in Betaflight
- **Battery Chemistry**: HV batteries (High Voltage LiPo) - 6S 22.2V nominal
- **Flight Time**: Expected 8-12 minutes in cruising flight
- **ESC Firmware**: BlueJay firmware on SpeedyBee AIO
- **Lost Model Recovery**: VIFLY GPS-Mate critical for cruising missions away from home point
- **Control Range**: ExpressLRS provides extended range for exploration flights
- **Custom Parts**: 3D printed TPU mounts for GPS stack (yellow for visibility)
- **Build Duration**: Extended build timeline (172+ days) reflects methodical, careful construction approach
- **Platform Size**: 3.5" wheelbase - small enough for tighter spaces, large enough for stable cruising

---

## Assembly Status Legend

- ✓ **Complete/Available**: Component ready or installed
- ⚠️ **In Progress**: Component partially installed or wired
- ⏳ **Pending**: Component not yet installed
- ❌ **Issue**: Component has problem or unavailable

---

## Maintenance Log

No maintenance actions documented yet (aircraft not yet operational).

---

## Configuration Changes

See `RD-54_Modifications_Log.md` for detailed modification history.
- **MOD-001**: Custom GPS/GPS-Mate stack (November 2025)

---

**Document Version**: 2.0 (Updated November 14, 2025)
**Archivist**: Claude Code, RD-54 SME
