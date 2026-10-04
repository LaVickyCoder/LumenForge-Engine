# LumenForge Engine

LumenForge Engine is an original, general-purpose game engine in active development, designed around a staged path toward high-end game-development capability.

This repository is the **public project surface** for LumenForge: project status, architecture overviews, roadmap, documentation, release notes, and future public SDK/runtime material. The complete internal development repository and proprietary development infrastructure remain private.

## Status

**Pre-alpha — active development**

The latest integrated source milestone is **E1-M02 — Concrete D3D12 Bootstrap**.

Verified foundations currently include:

- C++20 baseline
- Windows 11 x64 bring-up target
- CMake-based build and test workflow
- Core types, results, views, hashing, and UUID support
- Diagnostics and fail-fast contracts
- Platform, time, and filesystem foundations
- Window lifecycle and input handling
- Versioned binary serialization foundations
- Backend-neutral RHI contracts
- Direct3D 12 bootstrap work

LumenForge is not production-ready and does not currently claim feature parity with Unreal Engine, Unity, or other mature engines.

## Public / private boundary

The public repository is intended for portfolio visibility, project communication, documentation, demos, selected examples, and future externally licensed components.

Internal source, experimental branches, proprietary tooling, development automation, and private production infrastructure are intentionally not published here.

## Direction

LumenForge is being developed for two complementary uses:

1. **Internal game development** — powering games built within the LumenForge ecosystem.
2. **External use** — a future licensed offering for developers and studios, with commercial terms still under evaluation.

See [ROADMAP.md](ROADMAP.md), [ARCHITECTURE.md](ARCHITECTURE.md), and [COMMERCIAL.md](COMMERCIAL.md).

## Technology

- **Language:** C++20
- **Primary bring-up platform:** Windows 11 x64
- **Build system:** CMake
- **Graphics foundation:** Backend-neutral RHI with Direct3D 12 bootstrap
- **Development stage:** Pre-alpha

## Availability

No public production build or commercial license is available yet. Public previews, demos, SDK/runtime components, and licensing information will be announced here when they are ready.

## Copyright

Copyright © 2026 LaVickyCoder. All rights reserved.

See [LICENSE.md](LICENSE.md).
