# Environment Verification

See the installation docs for platform-specific verification steps:

```
docs/source/setup/installation/index.rst
```

## Quick Smoke Test

```bash
./isaaclab.sh -p -c "import isaaclab; print('isaaclab OK')"
./isaaclab.sh -p -c "import torch; print(f'PyTorch {torch.__version__}, CUDA: {torch.cuda.is_available()}')"
```

## Run Existing Tests

```bash
./isaaclab.sh -p -m pytest source/isaaclab/test/
./isaaclab.sh -p -m pytest source/isaaclab_physx/test/
./isaaclab.sh -p -m pytest source/isaaclab_newton/test/
./isaaclab.sh -p -m pytest source/isaaclab_tasks/test/test_environments.py
```
