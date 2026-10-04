# LumenForge Engine — Public Status

**Stage:** Pre-alpha  
**Latest verified integrated baseline:** E1-M02 — RHI Contract Foundation + Direct3D 12 Bootstrap  
**Primary bring-up platform:** Windows 11 x64  
**Language baseline:** C++20  
**Public repository role:** showcase / documentation / future demos and externally released components

## Verified integrated capability

| System | State | Notes |
| --- | --- | --- |
| Bootstrap & build | ✅ Integrated | CMake-based native build/test foundation |
| Core | ✅ Integrated | foundational types, Result/error contracts, views, hashing, UUID |
| Diagnostics | ✅ Integrated | diagnostics/assert/fatal behavior |
| Platform | ✅ Integrated | Windows x64 platform foundation |
| Time | ✅ Integrated | high-resolution Windows timing |
| FileSystem | ✅ Integrated | Windows file operations and public contracts |
| Serialization | ✅ Integrated | versioned binary-reference encoding/decoding and migration foundations |
| Window | ✅ Integrated | native Windows lifecycle and event pumping |
| Input | ✅ Integrated | neutral input events and runtime state |
| RHI | ✅ Integrated | backend-neutral adapter/device contracts |
| Direct3D 12 | ✅ Integrated | adapter enumeration and bounded device bootstrap |

## Not yet part of the verified public baseline

The following are not presented as completed features:

- swapchain and presentation;
- command submission/resource management beyond the current bootstrap contract;
- production renderer;
- scene/world runtime;
- asset pipeline/editor;
- physics;
- audio;
- networking;
- production SDK compatibility guarantees.

Some may exist as private design work or unmerged development, but the public showcase only marks capabilities as integrated after they are part of the verified internal baseline.

## Evidence policy

Public claims follow a simple rule:

> **Integrated means present in the canonical private engine baseline and supported by repository/test evidence.**

Roadmap entries are explicitly labeled as planned or future direction and should not be read as implementation claims.

## Media status

The public media structure is ready. Screenshots and short captures will be added from real running engine builds as useful visual milestones become available.
