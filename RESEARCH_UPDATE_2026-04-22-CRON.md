# MAIBOT Research Update — April 22, 2026 (00:00 UTC)

**Research Period:** April 21, 2026 22:12 UTC  
**Sources:** Official Ukrainian Ministry of Defence, Unmanned Systems Forces, Brave1, Defence Express, ArmyInform  
**Focus:** Ukrainian military robot technology, statistics, components, and specifications

---

## 📊 EXECUTIVE SUMMARY

Ukraine's Unmanned Systems Forces (USF) continues rapid expansion with **27,609 total targets** neutralized since June 2025. Ground robotic systems have scaled to **9,000+ missions per month** (up from 2,900 in November 2025), marking a 310% increase in operational tempo. Over **470 drone types** and **140+ robotic systems** are now registered on the Brave1 marketplace.

---

## 🎯 STATISTICS — UNMANNED SYSTEMS FORCES (USF)

### Killboard Data (Cumulative: June 2025 - Present)
| Metric | Value |
|--------|-------|
| **Total Targets** | 27,609 |
| **Destroyed** | 11,072 |
| **Enemy Personnel** | 6,692 |
| — Killed | 3,135 |
| — Wounded | 3,557 |

### Ground Robot Mission Scale
| Period | Missions/Month | Growth |
|--------|---------------|--------|
| Nov 2025 | 2,900 | Baseline |
| Mar 2026 | 9,000+ | +310% |

---

## 🤖 ROBOT PROFILES — Major Ukrainian Systems

### 1. MAUL (Medical Evacuation Robot)
**Developer:** 1st Separate Medical Battalion (USF)  
**Status:** Operational

| Specification | Value |
|--------------|-------|
| **Base Platform** | ATV (All-Terrain Vehicle) |
| **Propulsion** | Internal Combustion Engine (ICE) |
| **Max Speed** | 70 km/h |
| **Protection** | Armored capsule for casualty |
| **Communications** | 4 redundant systems (no fiber-optic) |
| **Survivability** | Survived 2 FPV hits + artillery barrage |

**Key Capabilities:**
- Speed-based survivability (harder to hit than slower electric platforms)
- Can self-right after overturning
- Protected capsule for casualty evacuation
- Cold-weather resistant (unlike battery-powered alternatives)

---

### 2. GNOM (Multifunctional Robotic Platform)
**Developer:** Temerland (Zaporizhzhia, Ukraine)  
**Status:** Mass production, NATO-certified

| Specification | Value |
|--------------|-------|
| **Chassis** | Wheeled 4×4 |
| **Drive** | Electric (4×1 kW motors) |
| **Power** | 42V Li-ion, 60 Ah |
| **Weight** | 50 kg |
| **Dimensions** | 570×380×600 mm |
| **Control Range** | <5 km |
| **Comm Channel** | WiFi 5 GHz / Private LTE (optional) |
| **Protection** | IP65 |
| **Operating Temp** | -25°C to +60°C |

**Components:**
- **Onboard Computer:** Odyssey single-board
- **Depth Camera:** Intel RealSense Depth Camera
- **Surveillance:** 360° panoramic camera on telescopic mast
- **Autonomy:** Smart Track (follow mode), GPS waypoints, return-home

**Roles:**
- Surveillance & reconnaissance
- Ammunition/food delivery
- Casualty evacuation (with trolley)
- Radio repeater for other systems
- Decoy/target identification

---

### 3. Ratel H (Logistics & Combat Support)
**Developer:** Ukrainian Ground Robotics Developer  
**Status:** Operational, mass production

| Specification | Value |
|--------------|-------|
| **Type** | Tracked/wheeled logistics UGV |
| **Payload** | ≥400 kg |
| **Weight** | 1,100 kg (1,500 kg with payload) |
| **Dimensions** | 2300×1300×1900 mm |
| **Range** | ≥60 km (on/off-road) |
| **Speed** | 8 km/h |
| **Control Range** | ≥50 km (via satellite) |
| **Cameras** | Day + night vision |

**Variants:**
- **Ratel H:** Logistics/tow truck (ammunition delivery, casualty evacuation)
- **Ratel Deminer:** Mine clearance (1,400mm sweep width, 2km control range)
- **Ratel FPV Launcher:** Armed with 4-cell fiber-optic FPV drone launcher

**System Components:**
1. Remotely controlled platform
2. Ground control station
3. Multicopter repeater
4. Charging station
5. Satellite-based remote control system

---

### 4. NC13 Unit Strike Robots
**Unit:** NC13 Robotic Strike Unit, 3rd Separate Assault Brigade (3rd Army Corps)  
**Commander:** Junior Lieutenant Mykola "Makar" Zinkevych

**Operational History:**
- **July 2025 Kharkiv:** World's first all-robotic assault (captured 2 Russian POWs)
- **Feb 2026 Kupiansk:** Thermobaric rocket attack on fortified school
- **Notable:** One robot held frontline position for 45 days

**Typical Payloads:**
- Explosive charges (up to 227 kg / 500 lbs)
- Thermobaric rockets (enclosed space effectiveness)
- 12.7mm machine guns (RSVK-M series)

---

## 🔧 COMPONENT DATABASE

### Flight Controllers (Ukrainian-Made)

#### GALYCHYNA F405 V2 6S/60A
**Manufacturer:** 603700 (Lviv, Ivano-Frankivsk, Kyiv, Vinnytsia, Dnipro)  
**Price:** $61 USD

| Feature | Specification |
|---------|--------------|
| **Firmware** | Betaflight 4.4.3 / 4.5.1, INAV 7.1.2+ |
| **ESC** | FRANKIVSK v2 6S/60A (Bluejay firmware) |
| **BEC** | Dual: 5V 3A + 5/9/12V 3A |
| **Servos** | 3 outputs |
| **UARTs** | 6 (telemetry, GPS, external modules) |
| **Motor Support** | Up to 6 motors (hexacopter capable) |
| **PINIO** | 2× controlled outputs (5V/1A) |
| **Frame Size** | Up to 10" |

**Special Features:**
- Video channel switching (anti-jamming)
- Hidden start point (OSD overlay covers location)
- Bi-directional DShot with RPM filtering
- Pre-configured for 7" and 10" drone builds

---

### AI/Computer Vision Systems

#### NVIDIA Jetson Xavier NX
**Usage:** Computer vision processing in combat robots

| Specification | Value |
|--------------|-------|
| **Size** | 103×90.5×34 mm |
| **Power** | Up to 10W |
| **GPU** | NVIDIA Volta (384 CUDA cores, 48 Tensor cores) |
| **CPU** | 6-core ARM Carmel 64-bit |
| **Memory** | 8 GB LPDDR4x (59.7 Gb/s) |
| **Performance** | 30 fps multi-model parallel processing |

**Capabilities:**
- Image classification
- Semantic segmentation
- Object detection (vehicles, personnel, obstacles)
- Autonomous navigation

---

### Sensors & Navigation

#### Inertial Measurement Units (IMUs)
| Manufacturer | Model | Application |
|-------------|-------|-------------|
| Analog Devices | Various | Navigation, stabilization |
| Bosch Sensortech | Various | Consumer/industrial grade |
| SBG Systems | High-precision | Military-grade navigation |
| InertialLabs | Various | Ground robotics |

#### Navigation System (DB Robotics Standard)
- **Satellite Receiver:** SNS (GPS/GLONASS/Galileo)
- **MEMS Sensors:** 9-axis (accelerometer, gyroscope, magnetometer)
- **Backup:** IMU-only mode for GPS-denied environments

#### Depth/Obstacle Detection
- **Intel RealSense Depth Camera** — Object identification and obstacle avoidance
- **Thermal Cameras** — Night operations, heat signature detection
- **IR Illuminators** — Low-light navigation

---

### Communication Systems

#### Military-Grade
| System | Specs | Notes |
|--------|-------|-------|
| **L3Harris** | MIL-STD-810G | US-supplied, $50-60k/set |
| **Programmable Frequency Hopping (PFR)** | 2-3 channel redundancy | Anti-jamming |
| **Private LTE** | Cellular-based | Optional on GNOM |
| **WiFi 5 GHz** | Standard | Consumer-grade backup |

#### Communication Range
| Platform | Range | Method |
|----------|-------|--------|
| MAUL | Unlimited (with comms) | Multi-redundant |
| GNOM | <5 km | WiFi/LTE |
| Ratel H | ≥50 km | Satellite-based |
| Ratel Deminer | ≥2 km | Radio |

---

### Power Systems

#### Battery Technologies
| Type | Voltage | Capacity | Application |
|------|---------|----------|-------------|
| Li-ion | 42V | 60 Ah | GNOM platform |
| 6S LiPo | 22.2V | 5000 mAh | FPV drones |
| ICE Generator | N/A | N/A | MAUL (cold-weather) |

#### Power Considerations
- **Electric platforms:** Silent, low IR signature, 24-hour endurance typical
- **ICE platforms:** Higher speed (70 km/h), cold-resistant, visible IR signature
- **Solar:** Available for Ratel (trailer accessory)

---

### Motors & Propulsion

#### Electric Motors (Ground Robots)
| Type | Specs | Usage |
|------|-------|-------|
| **4× BLDC 1kW** | Brushless DC | GNOM drive |
| **Stepper Motors** | Various | Weapon systems, turrets |

#### FPV Drone Propulsion
- **Brushless motors** with 6S/60A ESCs
- **4-6 motor configurations** (quad/hexacopter)
- **Bi-directional DShot** with RPM filtering

---

### Weapon Systems Integration

#### Combat Module Subsystems (RSVK-M series)
| Component | Technology |
|-----------|------------|
| **Machine Gun** | NSVT 12.7mm "Utyos" |
| **Fire Control** | Electronic single-shot system (unique Ukraine-developed) |
| **Alignment** | Laser module "cold firing" system (2-3 min calibration) |
| **Stabilization** | Gyroscopic barrel stabilization |
| **Targeting** | Ballistic calculator, rangefinder, reticle |

#### Explosive Payloads
- **Standard:** 30 kg charges
- **Heavy:** 227 kg (500 lbs) demolition charges
- **Thermobaric:** Enclosed-space effectiveness

---

## 📋 BRAVE1 MARKETPLACE DATA

### Platform Statistics
| Metric | Value |
|--------|-------|
| **Total Drone Types** | 470+ |
| **Robotic Systems Registered** | 140+ |
| **Defense Approved** | 96 |
| **NATO Standards Met** | 14 |
| **Systems Tested** | 50+ |

### Procurement Method
1. Soldiers browse 470+ drone types
2. Order placed via unit credits
3. Commander approval
4. Direct shipping to unit

---

## 🏢 UKRAINIAN ROBOTICS MANUFACTURERS

| Company | Location | Specialization |
|---------|----------|---------------|
| **Robotics Design Bureau** | Kyiv | RSVK-M series, combat modules |
| **Temerland** | Zaporizhzhia | GNOM platform |
| **Global Dynamics** | Lviv | Various platforms |
| **603700** | Multi-city | Flight controllers, FPV components |
| **Ukrainian Ground Robotics Developer** | — | Ratel series |

---

## 🎖️ USF UNIT STRUCTURE

### Brigades & Battalions
| Unit | Type | Commander/Notable |
|------|------|-------------------|
| **412th Separate Brigade** | Unmanned Systems | NEMESIS |
| **413th Regiment** | Unmanned Systems | RAID |
| **414th Separate Brigade** | Strike UAS | "Magyar's Birds" (Maj. Robert Brovdi) |
| **424th Battalion** | Unmanned Systems | SVAROG |
| **427th Separate Brigade** | Unmanned Systems | RAROG |
| **429th Separate Brigade** | Unmanned Systems | Achilles |
| **59th Assault Brigade** | Unmanned Systems | Steppe Predators |
| **20th Separate Brigade** | Unmanned Systems | K-2 |
| **NC13 Unit** | Robotic Strike | 3rd Assault Brigade |
| **Khartia Corps** | UGV Company | National Guard |

### Commander of USF
**Major Robert "Magyar" Brovdi** — Appointed June 2025, Hero of Ukraine

---

## 📚 OFFICIAL SOURCES

1. **Unmanned Systems Forces (USF)** — https://usforces.army/en/
2. **Brave1 Marketplace** — https://brave1.com.ua
3. **Defense Express** — https://en.defence-ua.com
4. **ArmyInform** — https://armyinform.com.ua/en/
5. **Temerland Robotics** — https://temerland.com/en/
6. **603700 FPV** — https://603700fpv.com.ua/en/
7. **Ukrainian Ground Robotics** — https://robots.com.ua/en/

---

## 🔍 RESEARCH METHODOLOGY

### Data Collection
- Public Ukrainian government sources only
- Official USF statistics and killboard data
- Manufacturer specifications from company websites
- Verified news reports from Defence Express, ArmyInform

### Validation
- Cross-referenced multiple sources for specifications
- Prioritized official government and manufacturer data
- Excluded operational security information (locations, current deployments)

---

## 🔄 NEXT RESEARCH TARGETS

1. **Shoolika mk6** — AI-enhanced drone specifications
2. **FoxTac Platform** — New evacuation system details
3. **Fiber-optic FPV launchers** — Technical specifications
4. **Electronic Warfare integration** — Counter-drone systems
5. **UB60D FPV** — 8-inch autonomous terminal guidance drone

---

**Report Generated:** 2026-04-22 00:00 UTC  
**Researcher:** MAIBOT Auto-Research System  
**Status:** ✅ Complete
