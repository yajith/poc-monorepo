# Shared

Shared code used by both components.

Modifying files in this directory triggers BOTH `component-a.yml` AND `component-b.yml`.
This is the key scenario for testing path analysis and aggregation:
- `portainer/lint` will wait for results from both component-a and component-b
- `portainer/unit-tests` will wait only for component-a (component-b has no unit-tests)
- `portainer/build` will wait for results from both
