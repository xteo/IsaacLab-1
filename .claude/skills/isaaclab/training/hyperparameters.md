# Hyperparameter Tuning

Refer to the agent config files for each task's defaults:

```
source/isaaclab_tasks/isaaclab_tasks/<type>/<category>/<task>/agents/
```

For example, CartPole configs:

```
source/isaaclab_tasks/isaaclab_tasks/manager_based/classic/cartpole/agents/
├── sb3_ppo_cfg.yaml
├── rsl_rl_ppo_cfg.py
├── skrl_ppo_cfg.yaml
└── rl_games_ppo_cfg.yaml
```

Read the config files directly — they contain all hyperparameters with comments.

## TensorBoard

```bash
./isaaclab.sh -p -m tensorboard.main --logdir=logs/
```

Note: metric names differ across frameworks. Check TensorBoard's scalar tags
after a training run to find reward, loss, and learning rate metrics.
