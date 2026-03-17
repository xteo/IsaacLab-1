# RSL-RL & SKRL Reference

See the training tutorial for full documentation:

```
docs/source/tutorials/03_envs/run_rl_training.rst
```

## RSL-RL

```bash
./isaaclab.sh -p scripts/reinforcement_learning/rsl_rl/train.py --task <TASK> --num_envs 4096 --headless
./isaaclab.sh -p scripts/reinforcement_learning/rsl_rl/play.py --task <TASK> --num_envs 10
```

- **Wrapper**: `RslRlVecEnvWrapper` (from `isaaclab_rl.rsl_rl`)
- **Config format**: Python class (`RslRlOnPolicyRunnerCfg`)
- **Resume**: `--resume` flag
- **Scripts**: `scripts/reinforcement_learning/rsl_rl/`

## SKRL

```bash
./isaaclab.sh -p scripts/reinforcement_learning/skrl/train.py --task <TASK> --num_envs 4096 --headless
./isaaclab.sh -p scripts/reinforcement_learning/skrl/play.py --task <TASK> --num_envs 10
```

- **Wrapper**: `SkrlVecEnvWrapper` (from `isaaclab_rl.skrl`)
- **Config format**: YAML files
- **Scripts**: `scripts/reinforcement_learning/skrl/`
