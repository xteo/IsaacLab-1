# Stable Baselines3 (SB3) Reference

See the training tutorial for full documentation:

```
docs/source/tutorials/03_envs/run_rl_training.rst
```

## Quick Start

```bash
./isaaclab.sh -p scripts/reinforcement_learning/sb3/train.py --task <TASK> --num_envs 64 --headless
./isaaclab.sh -p scripts/reinforcement_learning/sb3/play.py --task <TASK> --num_envs 10
```

## Key Details

- **Wrapper**: `Sb3VecEnvWrapper` (from `isaaclab_rl.sb3`)
- **Config format**: YAML files (see `agents/sb3_ppo_cfg.yaml` in each task)
- **Resume**: `--checkpoint <path/to/model.zip>`
- **Scripts**: `scripts/reinforcement_learning/sb3/`
