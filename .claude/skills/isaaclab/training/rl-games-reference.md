# RL-Games Reference

See the training tutorial for full documentation:

```
docs/source/tutorials/03_envs/run_rl_training.rst
```

## Quick Start

```bash
./isaaclab.sh -p scripts/reinforcement_learning/rl_games/train.py --task <TASK> --num_envs 4096 --headless
./isaaclab.sh -p scripts/reinforcement_learning/rl_games/play.py --task <TASK> --num_envs 10
```

- **Wrapper**: `RlGamesVecEnvWrapper` (from `isaaclab_rl.rl_games`)
- **Config format**: YAML files (nested `params.config.*` structure)
- **Resume**: `--checkpoint <path/to/model.pth>`
- **Scripts**: `scripts/reinforcement_learning/rl_games/`
