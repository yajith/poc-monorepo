# Component B

Example component for the GitHub Status Check Aggregator PoC.

Modifying files in this directory triggers `component-b.yml`:
- `portainer/lint` (run-linters)
- `portainer/build` (build-manifests)

Note: component-b has NO unit-tests capability.
A PR touching only component-b will see `portainer/unit-tests` auto-skipped by the Worker.
test change
