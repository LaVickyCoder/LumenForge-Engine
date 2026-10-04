# LumenForge Engine — Public Roadmap

This roadmap communicates product direction without exposing private development infrastructure. It is intentionally milestone-oriented and does not promise fixed delivery dates.

Legend:

- ✅ **Integrated** — present in the verified private-engine baseline
- 🟨 **Next** — logical next public capability, not claimed as integrated
- ⬜ **Future** — planned direction, subject to architecture and validation

## Engine 0 — Native foundation

| Capability | State |
| --- | --- |
| Executable/build bootstrap | ✅ Integrated |
| LFCore | ✅ Integrated |
| Diagnostics | ✅ Integrated |
| Windows x64 platform abstraction | ✅ Integrated |
| High-resolution time | ✅ Integrated |
| File system foundation | ✅ Integrated |
| Versioned binary serialization | ✅ Integrated |

## Engine 1 — Window, input & rendering foundations

| Capability | State |
| --- | --- |
| Native window lifecycle | ✅ Integrated |
| Event/input loop | ✅ Integrated |
| Backend-neutral RHI contract | ✅ Integrated |
| Direct3D 12 bootstrap | ✅ Integrated |
| Swapchain & presentation | 🟨 Next |
| Command queues / synchronization | ⬜ Future |
| GPU resource foundations | ⬜ Future |
| Shader/pipeline foundations | ⬜ Future |
| First complete rendered-frame path | ⬜ Future |

## Engine 2 — Runtime foundations

⬜ World/scene representation  
⬜ Entity/component runtime direction  
⬜ Resource and asset runtime  
⬜ Transform hierarchy  
⬜ Gameplay-facing runtime APIs  
⬜ Streaming foundations

## Engine 3 — Content & tools

⬜ Asset import/cooking pipeline  
⬜ Scene/content authoring  
⬜ Editor foundation  
⬜ Undo/redo and serialization workflows  
⬜ Profiling and diagnostic tooling  
⬜ Build/package workflows

## Engine 4+ — Production systems

Long-term areas include animation, physics, audio, navigation/AI support, networking, scalable rendering, performance and memory tooling, large-content workflows, and stable externally supported SDK/runtime interfaces.

## Public release path

```text
Portfolio & technical documentation
            ↓
Verified screenshots / development captures
            ↓
Small technology demos
            ↓
Developer preview / selected SDK material
            ↓
Externally licensed LumenForge offering
```

Exact packaging, licensing tiers, pricing, and release dates remain undecided.
