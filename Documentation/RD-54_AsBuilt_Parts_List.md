# RD-54 "Zorro" - As-Built Parts List

**Aircraft Designator**: RD-54 (Code Name: Zorro)
**Operator**: SpyD (Franco Nogarin)
**Platform Type**: 3.5" Digital FPV Cruiser
**Primary Mission**: Exploration and cinematic FPV flights with HD digital video
**Current Status**: Under Construction - Assembly Phase
**Airworthiness**: Not Yet Airworthy
**Last Updated**: November 14, 2025

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

---

### Video System

| Component | Part Number/Model | Quantity | Status | Notes |
|-----------|------------------|----------|---------|-------|
| **VTX** | Walksnail Moonlight | 1 | ⏳ Not Installed | Large footprint kit, JST-SH 4-pin power, LHCP pigtails included |
| **Camera** | (Included with Moonlight kit) | 1 | ⏳ Not Installed | Integrated with VTX |

---

### Radio System

| Component | Part Number/Model | Quantity | Status | Notes |
|-----------|------------------|----------|---------|-------|
| **Receiver** | HappyModel ExpressLRS EP1 Dual-TCXO | 1 | ✓ Available (not installed) | Original diverted to other aircraft, second EP1 located for RD-54 |

---

### Navigation & Sensors

| Component | Part Number/Model | Quantity | Status | Notes |
|-----------|------------------|----------|---------|-------|
| **GPS/GNSS** | GEPRC M10-DQ | 1 | ✓ Wired (ready to install) | With DPS310 barometer, integrated into custom GPS stack (MOD-001) |
| **GPS-Mate** | VIFLY GPS-Mate | 1 | ✓ Wired (ready to install) | Lost-model finder beacon, integrated into custom GPS stack (MOD-001) |

---

### Auxiliary Systems

| Component | Part Number/Model | Quantity | Status | Notes |
|-----------|------------------|----------|---------|-------|
| **Buzzer** | 5V Standard Buzzer | 1 | ⏳ Not Installed | To be mounted near top plate |

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
- ✓ Custom GPS stack fabricated and wired (ready for installation - will be installed last)
- ⏳ VTX/Camera installation (next major task)
- ⏳ Receiver not installed (EP1 available)
- ⏳ Buzzer not installed
- ⏳ GPS stack mounting (planned as final component)
- ⏳ Betaflight configuration not started
- ⏳ Radio binding not started

**Modifications from Original Spec**:
- **MOD-001**: Custom 3D printed TPU GPS/GPS-Mate stack (November 2025)
  - Added VIFLY GPS-Mate for lost-model recovery
  - Custom modular stack design for improved GPS elevation
  - See `RD-54_Modifications_Log.md` for details

---

## Pending Upgrades/Changes

**Immediate Next Steps**:
- Install Walksnail Moonlight VTX/Camera system (next major task)
- Install ExpressLRS receiver
- Install buzzer
- Wire management and routing
- Mount GPS stack to frame (planned as final component)
- Install top plate
- Initial Betaflight configuration

---

## Known Issues

**Current Blockers**:
- VTX/Camera not installed (required for FPV operation)
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

- **Mission Focus**: Digital FPV Cruiser - designed for smooth exploration flights with HD video recording
- **Video System**: Walksnail Moonlight HD digital FPV (LHCP pigtails included)
- **GPS Mounting**: Custom TPU stack provides elevation and integrates VIFLY GPS-Mate (MOD-001)
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
