# Public Development Changelog

This changelog summarizes externally meaningful milestones from the verified private engine history. It intentionally excludes internal governance, private development infrastructure, and proprietary implementation details.

## 2026-09-27 — E1-M02 Direct3D 12 bootstrap

- Integrated the concrete Direct3D 12 bootstrap.
- Added bounded backend initialization/device creation behavior.
- Hardened string handling around the D3D12 path.
- Reached the current verified public baseline.

## 2026-09-25 — E1-M02 RHI contract foundation

- Integrated backend-neutral RHI contracts.
- Added adapter/device concepts and explicit device-creation failure paths.
- Added RHI contract/public-header testing.

## 2026-09-20 — E1-M01 event & input loop

- Integrated neutral input contracts and input state.
- Integrated native window event/input handling.
- Added focus-loss/capture tracking and regression coverage.

## 2026-09-19 — Window lifecycle & serialization

- Integrated native Windows window lifecycle.
- Integrated versioned binary serialization foundations and migration support.

## 2026-09-18 — E0-M04 time & file system

- Integrated high-resolution time support.
- Integrated the Windows file-system foundation.

## 2026-09-17 — E0-M03 platform foundation

- Integrated the Windows x64 platform abstraction foundation.

## 2026-09-13 — Engine 0 foundation

- E0-M00: executable/bootstrap, CMake presets and CI foundation.
- E0-M01: core types, Result/error handling, views, hashing and UUID.
- E0-M02: diagnostics contracts and deterministic failure-path tests.
