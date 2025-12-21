# Project Plan: RD54 Zorro

**Project:** RD54_Zorro
**Owner:** Circuit (Fleet Steward)
**Created:** December 21, 2025
**Status:** Under Construction (~70%)

---

## Overview

RD54 "Zorro" is a 3.5" digital FPV cruiser optimized for smooth exploration with HD video. Features Walksnail digital system, GPS Rescue, and long-range ELRS.

**Repository:** `spydmobile/RD54_Zorro`
**Location:** `projects/drone_management/drones/RD54_Zorro/`
**Platform:** 3.5" Digital Cruiser (FlyFishRC Volador VX3.5)

---

## Current State

| Attribute | Value |
|-----------|-------|
| **Build Status** | Assembly Phase (~70%) |
| **Airworthiness** | NOT YET AIRWORTHY |
| **Flight Hours** | 0.0 |
| **Total Incidents** | 0 |
| **Video System** | Walksnail Moonlight HD (LHCP) |
| **Control Link** | ExpressLRS EP1 (pending install) |
| **GPS** | GEPRC M10-DQ + VIFLY GPS-Mate |

**Completed:**
- Frame assembled
- All 4 motors mounted and wired (Nov 14, 2025)
- FC/ESC stack installed
- Custom GPS stack fabricated (MOD-001)

**Remaining:**
- VTX/Camera installation
- Receiver installation
- Buzzer installation
- Wire management
- GPS stack mounting (final step)
- Betaflight configuration
- Maiden flight

---

## Milestones

### Milestone 1: Frame & Motors (COMPLETE)
**Status:** Complete | **Date:** November 14, 2025

- [x] Frame assembly (Volador VX3.5)
- [x] FC/ESC stack positioning
- [x] Motor 1 mounting and wiring
- [x] Motor 2 mounting and wiring
- [x] Motor 3 mounting and wiring
- [x] Motor 4 mounting and wiring

### Milestone 2: GPS Stack (COMPLETE)
**Status:** Complete | **Date:** November 2025

- [x] Design custom TPU stack mount (MOD-001)
- [x] 3D print GPS mount
- [x] Wire GPS and GPS-Mate
- [x] Test fit on frame

### Milestone 3: Video System (IN PROGRESS)
**Status:** In Progress | **Priority:** High

- [x] Parts acquired (Walksnail Moonlight HD)
- [ ] Mount VTX to frame
- [ ] Install camera
- [ ] Route antenna (LHCP)
- [ ] Wire to FC

### Milestone 4: Receiver & Buzzer (PENDING)
**Status:** Pending | **Priority:** High

- [ ] Install ExpressLRS EP1 receiver
- [ ] Route RX antennas
- [ ] Install buzzer (5V)
- [ ] Wire management

### Milestone 5: GPS Final Mount (PENDING)
**Status:** Pending | **Priority:** Medium

Install GPS stack as final component (on top).

- [ ] Mount GPS stack to frame
- [ ] Antenna placement optimization
- [ ] Install top plate

### Milestone 6: Configuration & Testing (PENDING)
**Status:** Pending | **Priority:** High

- [ ] Betaflight configuration
- [ ] GPS Rescue setup
- [ ] RTH configuration
- [ ] Walksnail binding
- [ ] ELRS binding
- [ ] Bench test all systems
- [ ] Pre-flight safety checks
- [ ] First hover test
- [ ] Maiden FPV flight

---

## GitHub Issues

| # | Title | Labels | Priority |
|---|-------|--------|----------|
| 1 | Install HDZero Freestyle V2 VTX/Camera System | pending-install, video-system | high |
| 3 | Install ExpressLRS EP1 Receiver and Antennas | pending-install, radio-system | high |
| 4 | Install GPS/GPS-Mate Stack | pending-install | - |
| 5 | Install HDZero Antenna Holder | pending-install, video-system | - |
| 6 | Install XT60 Battery Mount | pending-install | - |

*Note: Issue #1 references HDZero but drone uses Walksnail - verify correct VTX*

---

## Current Tasks

| Task | Priority | Status |
|------|----------|--------|
| Install Walksnail VTX/Camera | High | Next task |
| Install ELRS receiver | High | After VTX |
| Install buzzer | Medium | After RX |
| Wire management | Medium | After components |
| Mount GPS stack | Medium | Last component |
| Betaflight configuration | High | After assembly |
| Maiden flight | High | Final milestone |

---

## Operations

**Build documentation:**
- Parts List: `Documentation/RD-54_AsBuilt_Parts_List.md`
- Timeline: `Documentation/RD-54_Build_Timeline.md`
- Modifications: `Documentation/RD-54_Modifications_Log.md`

**Mission profile:** Digital FPV Cruiser
- Smooth exploration with HD video
- GPS Rescue for extended range safety
- Return-to-home capability

---

*Circuit - Fleet Steward*
