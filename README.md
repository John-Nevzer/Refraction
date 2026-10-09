# Adaptive Traffic Control (PoC)

A proof-of-concept simulation of adaptive traffic light control for a city's
main routes. Instead of fixed timing plans, the controller adjusts signal
phases based on the current traffic situation at each intersection.

## How it works

- **Data collection** — Traffic parameters (waiting vehicles, queue length,
  flow rate) are read from virtual sensors. Each reading includes a random
  deviation to mimic the inaccuracy of real sensors.
- **Control logic** — The controller dynamically sets green times,
  prioritizing the heaviest load while capping the maximum wait. Main routes
  are coordinated into a "green wave" for minimal stopping.
- **Goal** — Demonstrate that adaptive, sensor-driven control improves traffic
  flow over static timing, reducing delays, emissions, and unnecessary waiting.

## Status

Proof-of-concept only. Not intended for production. Real-world deployment would
require fine-tuning or rewriting, including integration with physical sensors
and compliance with safety and regulatory requirements.
