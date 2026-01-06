# Sentinel Network — Modeling Scope and Boundaries

## Purpose

This repository focuses on first-order, system-level behavior of a fault-tolerant Mars orbital relay constellation. The simulations are intended to evaluate architectural feasibility, coverage characteristics, revisit time, and resilience under satellite loss.

The goal is not to produce a flight-ready design, but to assess whether a dense relay layer can outperform traditional sparse relay architectures at the network level.

---

## What Is Modeled

The simulations in this repository explicitly model:

- Orbital geometry and constellation layout
- Global and regional surface coverage
- Revisit time distributions
- Network availability under nominal conditions
- Graceful degradation under partial and catastrophic satellite loss
- Sensitivity to constellation size and orbital regime

These models are sufficient to evaluate architectural viability and comparative performance trends.

---

## What Is Not Modeled

The following are intentionally out of scope:

- Detailed RF link budgets or modulation schemes
- Antenna design, pointing, or beamforming
- Radiation effects, shielding, or component-level fault tolerance
- Spacecraft bus design or mass/power budgets
- Launch vehicle selection or deployment logistics
- Ground station or surface terminal implementations
- Economic or cost modeling

Excluding these elements is a deliberate choice to avoid premature optimization and design lock-in.

---

## Rationale

Sentinel Network treats satellite loss as an expected operating condition and resilience as a network-level property rather than a spacecraft-level feature.

By constraining scope to geometry and availability, the project isolates the architectural question:

**Can constellation-level redundancy deliver persistent, low-latency relay performance at Mars scale?**

Lower-level engineering details can be layered onto this architecture in future work if warranted.

---

## Intended Use

This repository is intended for:
- Systems engineers
- Mission architects
- Infrastructure planners
- Early-phase trade studies

It is not intended to replace detailed mission design, hardware qualification, or agency-level studies.
