# Selected API Snapshot

These excerpts are selected from the current integrated engine contracts to illustrate coding style and architecture.

They are **not** a public compatibility promise or an SDK release. The API is pre-alpha and may change.

## Window lifecycle

```cpp
auto created = lf::window::Window::Create({});
if (created.has_error())
{
    return 1;
}

lf::window::Window window = std::move(created).value();

if (window.Show().has_error())
{
    return 2;
}

while (!window.ShouldClose())
{
    if (window.PumpEvents().has_error())
    {
        break;
    }
}

window.Destroy();
```

The current window contract exposes creation, show/close/destroy operations, event pumping, open/close state, client size and resize consumption.

## Result-oriented errors

```cpp
Result<Window> Window::Create(const WindowDesc& desc) noexcept;
Result<void> Window::Show() noexcept;
Result<void> Window::PumpEvents() noexcept;
```

The generic `Result<T, E>` model supports explicit success/failure states and typed errors.

## Render Hardware Interface

```cpp
auto backend = lf::rhi::CreateBackend(lf::rhi::Backend::Direct3D12);
if (backend.has_error())
{
    // Handle backend initialization failure.
}

auto& instance = *backend.value();
auto adapters = instance.GetAdapters();
```

Current RHI concepts include backend identity, adapters, queue capabilities and device-creation contracts.

## Versioned serialization

```cpp
Result<VersionedReferenceBytes, SerializationError>
EncodeVersionedReference(const VersionedReference& reference) noexcept;

Result<VersionedReference, SerializationError>
DecodeVersionedReference(Span<const u8> bytes) noexcept;
```

This establishes versioned binary-reference foundations while keeping migration/error handling explicit.

## Licensing note

These excerpts are published for portfolio/evaluation purposes under the repository's [All Rights Reserved notice](../../LICENSE.md).
