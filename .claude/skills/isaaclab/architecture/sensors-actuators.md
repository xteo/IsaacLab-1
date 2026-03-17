# Sensors, Actuators & Visualizers

See the official documentation for comprehensive coverage:

| Topic | Path |
|-------|------|
| Sensors overview | `docs/source/overview/core-concepts/sensors/index.rst` |
| Camera sensors | `docs/source/overview/core-concepts/sensors/camera.rst` |
| Contact sensors | `docs/source/overview/core-concepts/sensors/contact_sensor.rst` |
| IMU sensors | `docs/source/overview/core-concepts/sensors/imu.rst` |
| Ray casters | `docs/source/overview/core-concepts/sensors/ray_caster.rst` |
| Frame transformers | `docs/source/overview/core-concepts/sensors/frame_transformer.rst` |
| Actuators | `docs/source/overview/core-concepts/actuators/` |
| Renderers | `docs/source/overview/core-concepts/renderers.rst` |
| Tutorial: add sensors | `docs/source/tutorials/04_sensors/add_sensors_on_robot.rst` |

## Quick Reference

Sensors and actuators use the factory pattern. Import from `isaaclab.sensors` /
`isaaclab.actuators` — the correct backend implementation is resolved at runtime.

**Note**: Isaac Lab uses `xyzw` quaternion order throughout.

## Source Locations

| Component | Path |
|-----------|------|
| Core sensor interfaces | `source/isaaclab/isaaclab/sensors/` |
| PhysX sensor impls | `source/isaaclab_physx/isaaclab_physx/sensors/` |
| Newton sensor impls | `source/isaaclab_newton/isaaclab_newton/sensors/` |
| Visualizer impls | `source/isaaclab_visualizers/isaaclab_visualizers/` |
