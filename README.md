# Sentinel Network

Systems-level modeling and simulation of a fault-tolerant Mars orbital relay constellation.

---

## Overview

Future Mars surface operations—human and robotic—will require continuous, low-latency, and resilient communications coverage. Today’s relay architecture relies on a small number of aging orbiters performing multiple roles simultaneously, creating single points of failure and constraining operational scale.

Sentinel Network explores an alternative: a dense, fault-tolerant orbital relay layer designed explicitly as shared infrastructure rather than as a set of multi-mission flagship orbiters. In Sentinel, each satellite functions as a communications node, providing line-of-sight and store-and-forward connectivity between Mars surface assets, orbital users, and Earth relay paths.

This repository contains open simulations and systems-level analyses that evaluate the feasibility, performance, and failure tolerance of such a network.

---

## Problem Statement

Mars communications today face several structural limitations:

- Reliance on a small number of critical relay assets  
- Increasing data demand from surface operations  
- Limited fault tolerance and graceful degradation  
- Growing latency and availability constraints for autonomous systems  

As surface activity scales, data transport—not sensing or computation—becomes the primary bottleneck.

---

## What Sentinel Is

Sentinel Network is a conceptual Mars orbital relay constellation designed around the following principles:

- **Fault tolerance by design**  
  No single satellite is mission-critical; resilience is achieved at the constellation and network layers.

- **Graceful degradation**  
  Network performance degrades predictably under partial or catastrophic loss, rather than via abrupt service failures.

- **Infrastructure-first architecture**  
  A payload-agnostic relay layer that can support multiple missions, operators, and users over time.

- **Scalable deployment**  
  Constellation sizing and orbital regimes are selected for long operational lifetimes, volumetric efficiency, and compatibility with bulk deployment.

---

## Key Characteristics (Current Model)

- Constellation size: 168 satellites  
- Function: Communications and navigation relay  
- Coverage: Global Mars surface coverage  
- Performance focus: Revisit time, availability, and resilience under loss  
- Deployment philosophy: Bulk deployment compatible with high-capacity launch systems, without dependence on a specific launch vehicle  
- Operational lifetime: Long-duration orbital regimes (multi-decade class)  

Quantitative performance results and failure-mode analyses are implemented in the simulations and supporting documentation within this repository.

---

## Repository Contents

```text
Sentinel-Network/
├── README.md            — Project overview and context
├── LICENSE              — MIT License
├── simulations/         — Coverage, revisit, and loss-tolerance modeling
├── docs/                — Architecture summary and modeling scope
│   ├── architecture_summary.md
│   └── modeling_scope.md
├── figures/             — Generated plots and constellation visuals
└── data/                — Constants and reference parameters
```

This layout separates core simulations, documentation, figures, and reference data to support reproducible analysis and external review.

---

## Fault Tolerance Model

Fault tolerance is achieved at the constellation level through redundancy, spatial diversity, and orbital geometry rather than through highly complex, internally fault-tolerant satellites.

Satellite loss—whether isolated, clustered, or catastrophic—is treated as an expected operating condition. Network performance degrades in a predictable and quantifiable manner as nodes are lost, instead of exhibiting sharp thresholds or single-point failures.

---

## Non-Goals

This project intentionally does **not** attempt to:

- Replace high-data-rate science orbiters or flagship missions  
- Specify detailed RF link budgets, modulation schemes, or hardware designs  
- Optimize for mission-specific payloads or proprietary architectures  
- Address surface terminal, user equipment, or ground network implementation details  

The focus is on first-order system behavior, architectural feasibility, and fault-tolerance characteristics.

---

## Relationship to Existing Mars Assets

Sentinel Network is intended to complement existing and future Mars orbiters by providing a dedicated, resilient communications infrastructure layer optimized for availability and continuity.

Science orbiters and specialized missions remain responsible for high-value sensing and data generation, while Sentinel provides a persistent relay backbone capable of supporting scaled surface operations and multi-user demand.

---

## Project Status

**Active and evolving.** 

- Core simulations: initial set complete  
- Documentation: in progress  
- Higher-fidelity modeling: planned  
- External review, critique, and extension: encouraged  

This repository represents an open systems study, not a finalized design or flight program. 

---

## License

This project is released under the MIT License. Reuse, modification, and extension are encouraged with attribution. 

---

## Disclaimer

This work is an independent technical exploration. It is not affiliated with, endorsed by, or representative of any space agency or commercial entity.
