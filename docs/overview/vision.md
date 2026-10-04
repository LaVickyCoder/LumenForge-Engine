# Vision & Design Philosophy

LumenForge is a long-term game-engine project being developed from low-level native foundations upward.

The project has two intended destinations:

1. a dependable internal engine for LumenForge-developed games;
2. a future externally licensed engine or SDK offering.

## What the project optimizes for

### Measurable progress

The public project distinguishes clearly between **integrated**, **next**, and **future** capability. Aspirational roadmap items are not presented as completed features.

### Explicit systems

Subsystem boundaries, ownership, lifetime and failure behavior should be visible in APIs rather than hidden in convention.

### Native performance foundations

The current implementation is C++20 and begins with Windows x64 and Direct3D 12 bring-up. Future platform/API expansion must preserve a clear capability/fallback story rather than assume feature uniformity.

### Testable contracts

Low-level systems are developed together with tests for successful and failing behavior. A successful compile alone is not treated as proof of a production-ready engine feature.

### Tooling grows with the runtime

Editor, asset pipeline, profiling and production workflows are long-term first-class goals, but they are intentionally not claimed before the runtime foundations they depend on exist.

## What LumenForge is not claiming today

LumenForge is not currently production-ready, a complete public SDK, feature-equivalent to established commercial engines, a stable ABI/API promise, or open source.

The purpose of this public repository is to show the real evolution of the project without exposing proprietary engine source or private development infrastructure.
