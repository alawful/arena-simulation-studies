# Flow-shop blocking experiment

This Arena model studies a two-stage flow shop with a limited buffer before the second stage. When that buffer is full, a part remains blocked at the first-stage machine. The model also uses a shared AGV resource, so a part can be lost when no vehicle is available.

## Scenario explored

- Parts arrive with an exponential inter-arrival time of 3 minutes.
- Stage 1 has two machines with triangular processing time `TRIA(2, 3, 5)` minutes.
- Stage 2 has two machines with triangular processing time `TRIA(5, 7, 10)` minutes.
- The base buffer capacity is three parts.
- The saved scenarios compare machine, AGV, and buffer choices over an eight-hour run.

The original comparison used a simple teaching objective that rewards completed parts and penalizes lost parts and added resources. In that small experiment, adding resources did not always improve the objective enough to justify their assumed cost. Increasing the buffer reduced blocking and improved throughput, but the result is specific to these distributions, run length, and cost assumptions.

## Files

- `Model1.doe` is the Arena model.
- `1.png` through `7.png` are selected saved result views.

The submitted report was replaced by this note so the repository keeps the model and useful context without publishing university identifiers.
