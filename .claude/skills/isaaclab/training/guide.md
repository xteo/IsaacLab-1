# Isaac Lab RL Training

For full training documentation, refer to:

```
docs/source/tutorials/03_envs/run_rl_training.rst
docs/source/tutorials/03_envs/configuring_rl_training.rst
```

## Quick Reference

```bash
# Train (replace <framework> with sb3, rsl_rl, skrl, or rl_games)
./isaaclab.sh -p scripts/reinforcement_learning/<framework>/train.py --task <TASK> --headless

# Evaluate
./isaaclab.sh -p scripts/reinforcement_learning/<framework>/play.py --task <TASK> --num_envs 10

# TensorBoard
./isaaclab.sh -p -m tensorboard.main --logdir=logs/
```

## Common CLI Arguments

| Arg | Description |
|-----|-------------|
| `--task` | Task ID (e.g., `Isaac-Cartpole-v0`) |
| `--num_envs` | Parallel envs (256+ for large GPUs) |
| `--headless` | No viewport rendering |
| `--seed` | Random seed |
| `--max_iterations` | Training iterations |
| `--checkpoint` | Resume from checkpoint path |

## Agent Configs

Each task has per-framework agent configs at:

```
source/isaaclab_tasks/isaaclab_tasks/<type>/<category>/<task>/agents/
```

## RL Wrapper Source

```
source/isaaclab_rl/isaaclab_rl/
```
