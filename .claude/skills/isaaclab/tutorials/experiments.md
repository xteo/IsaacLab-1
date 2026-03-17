# Environment Customization & Experiments

For guidance on modifying environments, see the official tutorials:

```
docs/source/tutorials/03_envs/modify_direct_rl_env.rst
docs/source/tutorials/03_envs/create_manager_rl_env.rst
docs/source/tutorials/03_envs/configuring_rl_training.rst
```

## Common Modifications

- **Reward weights**: Edit the `RewardsCfg` in the environment config
- **Episode length**: Change `episode_length_s` in `__post_init__`
- **Network architecture**: Edit the agent config YAML/Python files in `agents/`
- **Domain randomization**: Add `EventTerm` entries to `EventCfg`
- **Camera observations**: Use RGB/depth task variants (e.g., `Isaac-Cartpole-RGB-v0`)

## Creating a New Project

```bash
./isaaclab.sh --new
```

This creates an isolated project you can modify without touching the Isaac Lab repo.

## Environment Examples

Browse working examples in the codebase:

```
source/isaaclab_tasks/isaaclab_tasks/manager_based/   # Manager-based
source/isaaclab_tasks/isaaclab_tasks/direct/           # Direct
```
