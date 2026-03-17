---
name: isaaclab
description: |
  Isaac Lab robotics learning framework. Use for: environment setup/troubleshooting,
  architecture questions (manager-based vs direct), RL training (SB3/RSL-RL/SKRL/
  RL-Games), building custom environments, or running tutorials like CartPole.
allowed-tools: Bash, Read, Write, Edit, Glob, Grep
---

# Isaac Lab

## Critical: Use `./isaaclab.sh -p` for All Python

All Isaac Lab scripts MUST use the wrapper. Never use bare `python3`.

```bash
./isaaclab.sh -p <script>
```

See [AGENTS.md](../../../AGENTS.md) for the full project guide (conventions, testing,
formatting, commit rules).

## What do you need?

### Setup & Troubleshooting
- [Installation](setup/fresh-install.md) - Points to official install docs
- [Verification](setup/verification.md) - Quick smoke tests and existing test suite
- [Troubleshooting](setup/troubleshooting.md) - Points to official troubleshooting docs

### Architecture & Design Patterns
- [Architecture overview](architecture/overview.md) - Factory pattern, source paths, doc pointers
- [Backends & renderers](architecture/backends.md) - Physics backends, renderers, visualizers
- [Pattern comparison](architecture/patterns-comparison.md) - Manager-based vs Direct
- [Sensors & actuators](architecture/sensors-actuators.md) - Sensor/actuator doc pointers

### RL Training & Evaluation
- [Training guide](training/guide.md) - CLI quick reference for all frameworks
- [SB3 reference](training/sb3-reference.md) - Stable Baselines3
- [RSL-RL & SKRL reference](training/rsl-rl-reference.md) - RSL-RL and SKRL
- [RL-Games reference](training/rl-games-reference.md) - RL-Games
- [Hyperparameters](training/hyperparameters.md) - Config file locations, TensorBoard

### Building Custom Environments
- [Environment builder](environments/builder.md) - Config structure, reward design rules
- [Code templates](environments/templates.md) - Pointers to real examples in the codebase

### Tutorials
- [CartPole](tutorials/cartpole.md) - Quick start and key source files
- [Code walkthrough](tutorials/code-walkthrough.md) - Source file pointers
- [Experiments](tutorials/experiments.md) - Common modifications and customization

### Key Documentation Paths
| Topic | Path |
|-------|------|
| Official installation | `docs/source/setup/installation/` |
| Tutorials | `docs/source/tutorials/` |
| Migration to Lab 3.0 | `docs/source/migration/migrating_to_isaaclab_3-0.rst` |
| API reference | `docs/source/api/` |
| Reference architecture | `docs/source/refs/reference_architecture/` |
| Troubleshooting | `docs/source/refs/troubleshooting.rst` |
