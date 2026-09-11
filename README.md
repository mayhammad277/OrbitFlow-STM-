# OrbitFlow Dynamics

**Autonomous mission design and constellation architecture — from first orbit to end of life.**

Not an alert. An autopilot for your constellation — and the engine that designs it in the first place.

[Request a Pilot](mailto:hello@orbitflow-dynamics.com) · [Menah Hammad](https://github.com/menatallh) · [May Hammad](https://github.com/mayhammad277)

---

## Table of Contents

- [Overview](#overview)
- [The Problem](#the-problem)
- [The Platform — Four Pillars](#the-platform--four-pillars)
- [How the Autopilot Works](#how-the-autopilot-works)
- [Non-Cooperative Object Handling](#non-cooperative-object-handling)
- [Formation Flight — Inspection & Touch-and-Go](#formation-flight--inspection--touch-and-go)
- [Why OrbitFlow](#why-orbitflow)
- [Market Opportunity](#market-opportunity)
- [Roadmap](#roadmap)
- [Team](#team)
- [Demos](#demos)
- [Contact](#contact)

---

## Overview

OrbitFlow Dynamics is the autonomous mission-design and constellation-architecture platform that plans a fleet's full lifecycle — coverage, station-keeping, collision avoidance, and disposal — and keeps recomputing it as conditions change, from LEO through cislunar and proximity operations.

For every close-approach event, we generate the **complete, ready-to-execute maneuver command**, coordinate it across the fleet, and guarantee its safety mathematically. The human operator retains final authority with a single **"Approve & Execute"** click — turning your team from ground operators into mission supervisors.

We react to unknown objects in **minutes (not days)** and handle both **cooperative fleet members** and **non-cooperative targets** (debris, silent spacecraft) with equal rigor.

## The Problem

Constellations have outgrown manual coordination — and the tools available today stop at the alert.

| Stat | What it means |
|---|---|
| **355,000+** | Starlink collision-avoidance maneuvers in the past year — triple 2024's total |
| **60–85%** | Success rate of GEO disposal attempts (ESA) — most failures trace to decisions made too late |
| **5 yrs** | New FCC LEO deorbit window — down from the 25-year guideline most fleets were designed around |

Legacy providers stop at the conjunction alert — they tell you something might hit, not what to do about it. Independent, satellite-by-satellite avoidance wastes propellant and can create new conflicts while resolving old ones. And traditional systems wait 24–48 hours for a full tracking record before acting on an unknown object — a delay a dense LEO environment can't afford.

## The Platform — Four Pillars

OrbitFlow isn't a point solution bolted onto your constellation after launch. One engine designs the fleet, keeps it safe, extends past LEO, and gets you close to anything that needs a closer look.

### 01 — Dynamic Fleet Orchestration
**Coverage, phasing, and scale — designed in, not bolted on.**
We architect a constellation's coverage geometry, orbital phasing, and slot assignment alongside its safety and disposal budget, so a fleet's growth plan and its collision-avoidance plan are never fighting each other. As the fleet scales, the architecture re-optimizes automatically instead of being redesigned from scratch.

### 02 — Zero-Debris Lifecycle Engine
**Collision avoidance and disposal, continuously recomputed.**
Physics-grounded path planning, joint fleet coordination, and a hard safety guarantee on every maneuver — from first deployment through station-keeping to a disposal plan that adapts in real time instead of a static filing made once at launch.

### 03 — Cislunar & Deep Space Networks
**The same engine, extended past Earth orbit.**
Multi-body trajectory design and space domain awareness for cislunar transit and the Earth-Moon economy — NRHO and halo-orbit planning, lunar comms-relay architecture, and tracking built for three-body gravitational dynamics, not the two-body assumptions most LEO tools are built on.

### 04 — Proximity Operations (RPO)
**Formation flight for missions that need to get close.**
Adaptive formation keeping, inspection flyby design, and touch-and-go maneuver planning — extending the same trajectory core to servicing, inspection, and non-cooperative rendezvous.

## How the Autopilot Works

*Pillar 02, in detail.*

| Module | What it does |
|---|---|
| **01 — Intelligent Path Planning** | Physics-grounded, auditable maneuver generation. Every candidate trajectory is physically realistic and fully explainable — no black box. |
| **02 — Joint Fleet Coordination** | Selects optimal joint maneuvers across the fleet. Cooperative operators de-conflict jointly; non-cooperative targets get a safe response without requiring their cooperation. |
| **03 — Hard Safety Guarantee + Command Generation** | Every maneuver is checked against hard separation constraints, then bundled into a ready-to-upload command file with its mathematical safety certificate. |
| **04 — Adaptive Unknown Object Response** | Reacts safely to unexpected objects — even fresh debris with no tracking history — within minutes, not the 24–48 hours legacy systems require. |

## Non-Cooperative Object Handling

*Pillar 02 continued.* Most of what threatens a constellation doesn't cooperate — derelict upper stages, fragmentation debris, dead satellites. Avoiding them is a fundamentally different problem than coordinating with a fleet member.

- **Continuous catalog fusion** — a live custody picture from multiple SSA sources, not a static daily snapshot
- **Fresh & uncatalogued debris** — builds a working orbit estimate from sparse initial observations within minutes
- **Worst-case avoidance planning** — hard, covariance-based separation constraints, not cooperative de-confliction logic
- **Continuous re-screening** — the avoidance plan adapts in real time as an object closes in
- **Sensor-agnostic ingestion** — radar, optical, and laser-ranging sources alike
- **Minutes, not days** — a provisional, safety-conservative plan within minutes of first detection

## Formation Flight — Inspection & Touch-and-Go

*Pillar 04, in detail.* Avoiding a conjunction and flying in formation are opposite problems — one keeps spacecraft apart, the other brings them together on purpose, safely.

- **Adaptive Formation Keeping** — leader-follower, cluster, or distributed formations that re-plan automatically as the mission changes
- **Inspection Flyby Design** — close-approach paths optimized for viewing geometry, lighting, and standoff safety margins
- **Touch-and-Go Maneuver Planning** — the full approach, contact, and safe-separation sequence, under the same safety shield throughout
- **Non-Cooperative Target Handling** — inspection and proximity planning for targets that can't share intent, like tumbling debris or defunct satellites

## Why OrbitFlow

Legacy SSA/STM providers are alert engines — they hand you a risk score and walk away. OrbitFlow is a decision engine: we plan, generate the command, coordinate, and guarantee the outcome, while you keep final authority.

| | Legacy SSA / STM Providers | OrbitFlow Dynamics |
|---|---|---|
| **Primary Function** | Monitoring & alerting (CDMs) | Full autopilot — plans, generates commands, coordinates, guarantees |
| **Maneuver Generation** | Manual, left to the customer | Automated, optimized, ready-to-upload |
| **Fleet Coordination** | None — isolated, satellite-by-satellite | Joint optimization, cooperative & non-cooperative |
| **Unknown Objects** | Waits 24–48 hours for tracking | Reacts within minutes |
| **Safety Assurance** | Statistical, probabilistic warnings | Hard, deterministic safety shield with audit log |
| **Command Delivery** | Suggestion — operator builds it manually | Ready-to-execute command file with safety certificate |
| **Human Role** | Executor | Supervisor — reviews and clicks "Approve & Execute" |

## Market Opportunity

| Stat | Source |
|---|---|
| **40+** avoidance maneuvers per satellite per year, fleet-wide average at scale | SpaceX FCC filings, 2026 |
| **~2** actionable conjunction alerts per satellite, per week | ESA Collision Avoidance Challenge |
| **1M** projected annual maneuvers across one mega-constellation by 2027 | KeepTrack, 2026 estimate |
| **$0.21B → $0.68B** cislunar SDA market, 2025→2034 (14% CAGR) | Market projection, 2025 |

SpaceX built its own in-house autonomous system because it could afford to — it now runs over 355,000 maneuvers a year — but that system serves SpaceX alone. OneWeb, a fraction of Starlink's size, is already mid-replenishment on its own fleet, proving this isn't a mega-constellation-only problem.

**Target customers:** LEO constellation operators, mid-size fleets managing active replenishment, SSA providers extending beyond screening into autonomous maneuver planning, and satellite insurers needing an auditable safety case.

## Roadmap

Full orbit propagation, two-stage conjunction screening, verified frame transforms, and the intelligent path planner already run end-to-end on synthetic scenarios.

1. **Coordination Integration** — coordination layer integrated with the path planner
2. **Adaptive Response Layer** — unknown-object detection and minutes-not-days reaction logic, benchmarked
3. **Validated Demo** — multi-satellite avoidance and unknown-object response against realistic scenarios
4. **Operator Pilot** — pilot deployment with a constellation operator or SSA provider on real
---

## 🖼️ Scenario Visualizations

<img width="1200" height="1200" alt="ECI Scenario" src="https://github.com/mayhammad277/OrbitFlow-STM-/blob/main/eci_scenario.png" />

*Full orbital propagation and conjunction screening visualized in Earth-Centered Inertial (ECI) coordinates.*

<img width="1200" height="1200" alt="LVLH Encounter" src="https://github.com/mayhammad277/OrbitFlow-STM-/blob/main/lvlh_encounter.png" />

*Local relative-motion planning visualized in the Local Vertical Local Horizon (LVLH) frame.*

---




---


## 📖 Full Pitch

🌐 **[Read the full pitch here](https://mayhammad277.github.io/OrbitFlow-STM-/)** 

---

## 📬 Contact

may23773@gmail.com
---

*OrbitFlow Dynamics — Structured, propellant-efficient collision avoidance for satellite constellations.*
