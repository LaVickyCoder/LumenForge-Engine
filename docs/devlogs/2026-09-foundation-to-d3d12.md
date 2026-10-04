# Devlog — From Bootstrap to Direct3D 12

September 2026 established LumenForge's first complete chain of native foundations.

The month began with a C++20 executable/build skeleton and quickly added the common systems needed before meaningful rendering work could start: Core, Diagnostics, Platform, Time and FileSystem.

Versioned serialization and a native Window subsystem followed, then the window event path was connected to a neutral Input layer.

The final September milestone introduced the first backend-neutral Render Hardware Interface and its first concrete backend: Direct3D 12.

```text
Bootstrap
   ↓
Core / Diagnostics
   ↓
Platform / Time / FileSystem
   ↓
Serialization
   ↓
Window
   ↓
Input
   ↓
RHI
   ↓
Direct3D 12 bootstrap
```

The important part is not the number of modules: each step exists to create a stable dependency boundary for the next one.

The current public baseline stops at the D3D12 adapter/device bootstrap. Renderer, scene and editor capabilities will only be shown when they are actually integrated.
