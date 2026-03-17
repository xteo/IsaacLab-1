# CartPole Tutorial

For the full tutorial, see the official docs:

```
docs/source/tutorials/03_envs/run_rl_training.rst
docs/source/tutorials/03_envs/create_manager_rl_env.rst
```

## Quick Start

```bash
./isaaclab.sh -p scripts/reinforcement_learning/rsl_rl/train.py \
  --task Isaac-Cartpole-v0 --num_envs 4096 --headless

./isaaclab.sh -p scripts/reinforcement_learning/rsl_rl/play.py \
  --task Isaac-Cartpole-v0 --num_envs 10
```

## Key Files

| File | Purpose |
|------|---------|
| `source/isaaclab_assets/isaaclab_assets/robots/cartpole.py` | Robot asset config |
| `source/isaaclab_tasks/isaaclab_tasks/manager_based/classic/cartpole/cartpole_env_cfg.py` | Environment config |
| `source/isaaclab_tasks/isaaclab_tasks/manager_based/classic/cartpole/__init__.py` | Gym registration |
| `source/isaaclab_tasks/isaaclab_tasks/manager_based/classic/cartpole/agents/` | RL agent configs |
| `source/isaaclab_tasks/isaaclab_tasks/direct/cartpole/` | Direct implementation |

Read the environment config file directly to understand the observations, actions,
rewards, terminations, and events.
