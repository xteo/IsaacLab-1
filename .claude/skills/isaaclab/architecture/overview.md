# Isaac Lab Architecture

Isaac Lab uses a **factory pattern** for physics and rendering. The core `isaaclab`
package defines abstract base classes; concrete implementations live in backend
packages (`isaaclab_physx`, `isaaclab_newton`, `isaaclab_ov`). Your code imports from
`isaaclab` and the factory resolves the correct backend at runtime.

There are two environment patterns: **Manager-Based** (modular, recommended) and
**Direct** (monolithic, for full control or multi-agent).

## Documentation

| Topic | Path |
|-------|------|
| Reference architecture | `docs/source/refs/reference_architecture/index.rst` |
| Core concepts | `docs/source/overview/core-concepts/index.rst` |
| Task workflows (manager vs direct) | `docs/source/overview/core-concepts/task_workflows/` |
| Backends & renderers | [backends.md](backends.md) |
| Pattern comparison | [patterns-comparison.md](patterns-comparison.md) |
| Sensors & actuators | [sensors-actuators.md](sensors-actuators.md) |

## Key Source Locations

| Component | Path |
|-----------|------|
| Core framework | `source/isaaclab/isaaclab/` |
| MDP functions | `source/isaaclab/isaaclab/envs/mdp/` |
| Managers | `source/isaaclab/isaaclab/managers/` |
| Task environments | `source/isaaclab_tasks/isaaclab_tasks/` |
| Robot assets | `source/isaaclab_assets/isaaclab_assets/robots/` |
| RL wrappers | `source/isaaclab_rl/isaaclab_rl/` |
| Controllers | `source/isaaclab/isaaclab/controllers/` |
