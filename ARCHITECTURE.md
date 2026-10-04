# Architecture Overview

LumenForge is being built as a modular native engine with explicit subsystem boundaries and testable contracts.

## Current subsystem map

```text
LumenForge
├── Core
├── Diagnostics
├── Platform
├── Time
├── FileSystem
├── Window
├── Input
├── Serialization
└── RHI
    └── Direct3D 12 bootstrap
```

### Core

Foundational types and low-level utilities used by other engine systems, including result/error handling, views, hashing, UUID support, and shared contracts.

### Diagnostics

Assertion, fatal-error, and diagnostic foundations intended to make engine failures explicit and testable.

### Platform

Platform abstraction foundations, currently focused on Windows 11 x64 bring-up.

### Time

High-resolution timing foundations and platform-specific time services.

### FileSystem

Filesystem abstractions and Windows implementation work.

### Window and Input

Native window lifecycle, event pumping, focus/capture behavior, and input-state contracts.

### Serialization

Versioned binary serialization and migration foundations.

### RHI

Backend-neutral rendering contracts designed to keep higher engine layers independent from one graphics API. Current implementation work includes Direct3D 12 bootstrap.

## Design direction

The architecture is intentionally being developed in measured stages. Higher-level systems will be added only after lower-level contracts are sufficiently stable and testable.

Long-term areas under consideration include resource management, rendering pipelines, scene/world systems, asset processing, editor tooling, animation, physics, audio, networking, profiling, and production build tooling.

These are roadmap directions, not current feature claims.
