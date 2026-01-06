# Sentinel Network

Open simulation and systems analysis for a fault-tolerant Mars orbital relay constellation.

---

## Overview

Future Mars surface operations—human or robotic—will require continuous, low-latency, and resilient communications coverage. Today’s Mars relay architecture depends on a small number of aging orbiters performing multiple roles simultaneously, creating inherent single-point-of-failure risks and constraining operational scale.

Sentinel Network explores a different approach: a dense, fault-tolerant orbital relay layer designed explicitly as infrastructure rather than as a set of multi-mission flagship orbiters.

In Sentinel, each satellite functions as a communications relay, providing line-of-sight, store-and-forward connectivity between Mars surface assets, orbital users, and Earth relay paths.

This repository contains open simulations and systems-level analyses evaluating the feasibility, performance, and failure tolerance of such a network.

---

## Problem Statement

Mars communications today face several structural limitations:
- Reliance on a small number of critical relay assets
- Increasing data demand from surface operations
- Limited fault tolerance and graceful degradation
- Growing latency constraints for autonomous systems

As surface activity scales, data transport, not sensing or computation, becomes the bottleneck.

---

## What Sentinel Is

Sentinel Network is a conceptual Mars orbital relay constellation designed around the following principles:
- **Fault tolerance by design**  
  No single satellite is mission-critical; resilience is achieved at the network level.
- **Graceful degradation**  
  Network performance degrades predictably under partial or catastrophic loss.
- **Infrastructure-first architecture**  
  A payload-agnostic relay layer supporting multiple missions and users.
- **Scalable deployment**  
  Constellation sizing and orbital regimes selected for long operational lifetimes and volumetric efficiency.

---

## Key Characteristics (Current Model)

- Constellation size: 168 satellites
- Function: Communications and navigation relay
- Coverage: Global Mars surface coverage
- Performance focus: Revisit time, availability, and resilience
- Deployment philosophy: Bulk deployment compatible with high-capacity launch systems, but not dependent on any specific launch vehicle
- Operational lifetime: Long-duration orbital regimes (multi-decade class)

Quantitative performance results and failure-mode analyses are documented in the simulations and supporting documentation.

---

## Repository Contents:

Sentinel-Network/  
├── README.md            — Project overview and context  
├── LICENSE              — MIT License  
├── simulations/         — Coverage, revisit, and loss-tolerance modeling  
├── docs/                — Architecture notes, modeling assumptions, scope boundaries, and non-goals  
├── figures/             — Generated plots and constellation visuals  
└── data/                — Constants and reference parameters  

---

## Fault Tolerance Model

Fault tolerance is achieved at the constellation level through redundancy, spatial diversity, and orbital geometry rather than through complex, internally fault-tolerant satellites.

Satellite loss—whether isolated, clustered, or catastrophic—is treated as an expected operating condition. Network performance degrades in a predictable and quantifiable manner as nodes are lost, rather than experiencing abrupt failure modes.

---

## Non-Goals

This project intentionally does not attempt to:
- Replace high-data-rate science orbiters or flagship missions
- Specify detailed RF link budgets, modulation schemes, or hardware designs
- Optimize for mission-specific payloads or proprietary architectures
- Address surface terminal or ground network implementation details

The focus is on first-order system behavior and architectural feasibility.

---

## Relationship to Existing Mars Assets

Sentinel Network is intended to complement existing Mars orbiters by providing a dedicated, resilient communications infrastructure layer optimized for availability and continuity.

Science orbiters and specialized missions would continue to perform high-value sensing and data generation roles, while Sentinel provides a persistent relay backbone capable of supporting scaled surface operations and multi-user demand.

---

## Project Status

**Active and evolving.**
- Core simulations: complete
- Documentation: in progress
- Higher-fidelity modeling: planned
- External review and iteration: encouraged

This repository represents an open systems study, not a finalized design or flight program.

---

## License

This project is released under the MIT License.  
Reuse, modification, and extension are encouraged with attribution.

---

## Disclaimer

This work is an independent technical exploration.  
It is not affiliated with, endorsed by, or representative of any space agency or commercial entity.
