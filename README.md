# Sentinel Network v4.6

**Mars Global Monitoring & Infrastructure Constellation**

A systems-level study of a fault-tolerant, cognitive-sensing orbital constellation designed as shared planetary infrastructure.

---

## Overview

Sentinel Network explores a fundamentally different approach to Mars orbital infrastructure: a dense, resilient constellation that combines **global synoptic monitoring** with **onboard cognitive intelligence** to deliver persistent awareness, low-latency decision support, and graceful degradation under failure.

Rather than relying on a small number of high-value relay orbiters, Sentinel distributes capability across 168 satellites, each carrying a dual-layer cognitive payload (wide-field global sensors + narrow-field AI-triggered inspection). The system is designed to operate as **planetary infrastructure** — supporting multiple users, missions, and operators over multi-decade lifetimes while maintaining performance even under significant satellite loss.

This repository contains the open simulations, analyses, and visualizations that define and validate the v4.6 architecture.

---

## What Sentinel Actually Is

- **Dual-layer cognitive payload** on every satellite (global synoptic + AI-gated narrow-field inspection)
- **Closed-loop autonomy** — onboard AI that detects, classifies, prioritizes, and retasks faster than light time to Earth
- **Extreme fault tolerance** — graceful degradation even under 75% satellite loss
- **Long-term infrastructure behavior** — 10+ year power/compute degradation modeling with adaptive modes
- **Radiation-adaptive intelligence** — AI and sensors intelligently throttle or safe themselves during SEP events
- **End-to-end latency modeling** — from event on Mars surface to actionable awareness on Earth

Sentinel is not just a communications relay. It is a **planetary nervous system** with onboard decision-making capability.

---

## Key Results (v4.6)

| Metric                              | Performance                          | Notes |
|-------------------------------------|--------------------------------------|-------|
| Mean global revisit (nominal)       | ~1.0–1.5 minutes                     | Wide-FOV MARCI-class sensors |
| Mean global revisit (75% loss)      | Still under 10 minutes               | Extreme resilience demonstrated |
| End-to-end awareness latency        | Minutes to low hours                 | Even in catastrophic scenarios |
| Decision/retasking latency          | Seconds (local) to minutes (global)  | Faster than light time |
| Propulsion-limited lifetime         | 40+ years                            | With conservative margins |
| Worst-case stacked failure survival | Survives (battery >0%)               | Dust + eclipse + 500× SEP + 43% loss |

---

## Repository Structure

```text
Sentinel-Network/
├── README.md
├── LICENSE
├── scripts/                    # Polished analysis scripts
├── figures/                    # Generated plots and animations
├── docs/                       # Architecture notes
└── simulations/                # Original/raw versions + reference files

Core Principles

Fault tolerance by design — No single satellite is mission-critical
Graceful degradation — Performance declines predictably, never catastrophically
Closed-loop autonomy — Onboard AI makes decisions without waiting for Earth
Infrastructure-first — Built for long-term, multi-user, multi-mission use
Conservative modeling — All analyses intentionally use pessimistic assumptions


Project Status
v4.6 Complete — Full systems-level modeling suite finished.
This is an open technical study. All scripts, models, and visualizations are released for review, critique, extension, and reuse.

License
MIT License — reuse, modify, and extend freely with attribution.
