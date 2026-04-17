# MAIBOT — Ukrainian Military Robot Intelligence Research

> Research Ukrainian military robot technology, statistics, and components with hourly updates from official Ukrainian sources.

## 🎯 Mission

Track and document:
- **Technology** — Robot types, AI systems, autonomy levels
- **Statistics** — Units deployed, success rates, operational data
- **Parts & Components** — Hardware, sensors, propulsion, weapons systems
- **Sources** — Official Ukrainian Ministry of Defence, news, verified reports

## 📁 Project Structure

```
MAIBOT/
├── research/
│   ├── daily-reports/        # Daily compiled research
│   ├── robot-profiles/       # Individual robot specs
│   └── component-database/   # Parts & technology index
├── data/
│   ├── robots.json           # Robot inventory
│   ├── components.json       # Parts database
│   └── statistics.json       # Deployment stats
├── docs/
│   ├── README.md
│   ├── SOURCES.md            # Verified Ukrainian sources
│   └── METHODOLOGY.md        # Research approach
├── scripts/
│   ├── research-updater.sh   # Hourly research runner
│   └── data-aggregator.py    # Parse & structure findings
└── src/
    └── dashboard.tsx         # Research visualization
```

## 🔗 Official Ukrainian Sources

| Source | URL | Content |
|--------|-----|---------|
| **Ministry of Defence** | https://www.mil.gov.ua | Official announcements |
| **Main Directorate** | https://gur.gov.ua | Intelligence reports |
| **Defence Express** | https://defence.ua | Military analysis |
| **Militarny.com** | https://militarny.com | Hardware specs |
| **Zbroya.net** | https://zbroya.net | Equipment database |
| **UCCA** | https://www.ucca.kmu.gov.ua | Coordination Center |

## 🤖 Tracked Robot Systems

### Known Ukrainian Military Robots
- **Loitering Munitions** — FPV drones, drone swarms
- **Ground Robots** — Clearance, reconnaissance, combat
- **Aerial Systems** — Fixed-wing, rotary, hybrid
- **Underwater** — Mine countermeasures, surveillance

### Data Points per Robot

```json
{
  "id": "robot-001",
  "name": "FPV Drone Swarm v3",
  "category": "loitering-munition",
  "technology": {
    "autonomy": "semi-autonomous",
    "ai_system": "basic-cv",
    "communication": "video-link + RC",
    "range": "3-10km",
    "endurance": "15-30min"
  },
  "components": {
    "frame": "carbon-fiber",
    "propulsion": "4x brushless-motors",
    "battery": "6S-LiPo-5000mAh",
    "camera": "hd-fpv-camera",
    "transmission": "digital-hdmi"
  },
  "statistics": {
    "units_deployed": 500,
    "success_rate": 0.85,
    "cost_per_unit": "$3000-5000"
  },
  "sources": ["mil.gov.ua", "defence-express"],
  "last_updated": "2026-04-17"
}
```

## 📊 Research Categories

### Technology Tracking
- **Autonomy Level** — Manual, semi-autonomous, autonomous
- **AI/CV Systems** — Object detection, targeting, pathfinding
- **Communication** — Radio, satellite, mesh-networks
- **Sensors** — Camera, LIDAR, thermal, radar
- **Weapons Integration** — Explosives, EMP, kinetic

### Component Database
- **Frames** — Materials, design, modularity
- **Propulsion** — Motors, batteries, fuel cells
- **Electronics** — Autopilots, flight controllers, SDRs
- **Optics** — Cameras, thermal, targeting systems
- **Armor/Protection** — Shielding, hardening

### Operational Statistics
- Deployment numbers
- Combat effectiveness
- Casualty rates (if public)
- Maintenance cycles
- Cost per unit

## 🔄 Hourly Research Loop

**Cron Job:** `maibot-research` (every 1 hour)

### Process
1. **Scrape Ukrainian sources** for new robot mentions
2. **Extract data** — specs, statistics, component info
3. **Validate** — Cross-reference with multiple sources
4. **Aggregate** — Update JSON databases
5. **Report** — Generate daily summary markdown
6. **Commit** — Push to GitHub

## 📝 Output Files

Generated hourly:
- `research/daily-reports/2026-04-17.md` — Daily findings
- `data/robots.json` — Updated inventory
- `data/components.json` — Parts database
- `data/statistics.json` — Deployment stats

## 🔐 Ethical Guidelines

- ✅ Only use **publicly available** Ukrainian government sources
- ✅ Focus on **defensive** technology context
- ✅ No targeting data or operational security info
- ✅ Attribute all sources explicitly
- ✅ Document methodology clearly
- ❌ No private military contractor data
- ❌ No current operational locations
- ❌ No classified information

## 📚 Related

- Ukrainian Ministry of Defence: https://www.mil.gov.ua
- Defence of Ukraine portal: https://www.defensepolicy.org.ua
- Military.com Ukraine section

---

**Status:** 🟢 Just created (2026-04-17)
**Repository:** https://github.com/TheWinterProgrammer/MAIBOT
**Update Frequency:** Hourly via cron
