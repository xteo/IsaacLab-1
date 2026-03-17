# Physics Backends, Renderers & Visualizers

Isaac Lab 3.0 uses a multi-backend architecture with a factory pattern. The core
`isaaclab` package defines abstract interfaces; backend packages provide concrete
implementations selected at runtime.

## Documentation

| Topic | Path |
|-------|------|
| Multi-backend overview | `docs/source/setup/ecosystem.rst` |
| Migration to Lab 3.0 | `docs/source/migration/migrating_to_isaaclab_3-0.rst` |
| Renderer architecture | `docs/source/overview/core-concepts/renderers.rst` |
| Newton integration | `docs/source/experimental-features/newton-physics-integration/index.rst` |

## Source Locations

| Component | Path |
|-----------|------|
| Physics base classes | `source/isaaclab/isaaclab/physics/` |
| Factory utils | `source/isaaclab/isaaclab/utils/backend_utils.py` |
| PhysX backend | `source/isaaclab_physx/` |
| Newton backend | `source/isaaclab_newton/` |
| Renderer factory | `source/isaaclab/isaaclab/renderers/` |
| Visualizer impls | `source/isaaclab_visualizers/` |
