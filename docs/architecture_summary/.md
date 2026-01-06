# Sentinel Network — Architecture Summary

## Purpose

Sentinel Network is a systems-level exploration of a fault-tolerant Mars orbital relay constellation.
The objective is to evaluate whether communications availability, revisit time, and resilience can be achieved through constellation architecture rather than through individually complex spacecraft.

This document summarizes architectural intent and modeling scope. Detailed performance results are captured in the simulation outputs.

---

## Architectural Concept

Sentinel is designed as a **dedicated orbital infrastructure layer**, not as a multi-mission science platform.

Each satellite functions as a relay node within a dense constellation optimized for:
- Persistent line-of-sight availability to the Mars surface
- Network-level redundancy
- Predictable degradation under partial or catastrophic loss

No individual satellite is mission-critical.

---

## Constellation Philosophy

Key architectural assumptions:
- High node count enables statistical resilience
- Spatial diversity replaces single-point reliability
- Performance is evaluated at the network level, not per satellite

The constellation geometry and sizing are selected to favor:
- Global surface availability
- Short revisit intervals
- Long-duration orbital stability

---

## Modeling Scope

The simulations in this repository evaluate:
- Surface coverage and revisit behavior
- Network availability under nominal conditions
- Graceful degradation under progressive satellite loss
- Sensitivity to constellation size and orbital geometry

The models intentionally operate at first-order fidelity to isolate architectural behavior.

---

## Out of Scope

This project does not attempt to:
- Specify spacecraft hardware, buses, or radiation hardening
- Define RF link budgets or modulation schemes
- Optimize for mission-specific payloads
- Model surface terminals or Earth-side infrastructure

These exclusions are deliberate.

---

## Interpretation Guidance

Results should be interpreted as:
- Architectural feasibility indicators
- Relative performance comparisons
- System behavior trends under failure

They are not flight designs or procurement-ready specifications.

---

## Status

Sentinel Network is an open systems study.
The architecture and simulations are considered stable at the conceptual level, with refinement expected through review and iteration.
