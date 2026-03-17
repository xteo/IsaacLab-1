# Manager-Based vs Direct Environments

Isaac Lab offers two environment patterns. See the official docs for full details:

| Topic | Path |
|-------|------|
| Task workflows overview | `docs/source/overview/core-concepts/task_workflows/` |
| Create a manager-based env | `docs/source/tutorials/03_envs/create_manager_base_env.rst` |
| Create a manager-based RL env | `docs/source/tutorials/03_envs/create_manager_rl_env.rst` |
| Create a direct RL env | `docs/source/tutorials/03_envs/create_direct_rl_env.rst` |
| Modify a direct RL env | `docs/source/tutorials/03_envs/modify_direct_rl_env.rst` |

## Quick Summary

| Aspect | Manager-Based | Direct |
|--------|---------------|--------|
| Style | Modular config classes | Monolithic class with overrides |
| Reward modification | Edit config weights | Edit function code |
| Multi-agent | Not supported | `DirectMARLEnv` |
| Best for | Most tasks, experimentation | Simple envs, max control, MARL |

## Code Examples

Working examples live in:

```
source/isaaclab_tasks/isaaclab_tasks/manager_based/   # Manager-based
source/isaaclab_tasks/isaaclab_tasks/direct/           # Direct
```
