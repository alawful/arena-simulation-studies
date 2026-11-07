# Inventory and production simulation

This Arena model studies a simple make-to-stock system over a simulated workday. Customer arrivals request a small random quantity. Available demand is fulfilled from inventory; otherwise the customer and requested quantity are counted as lost demand.

When inventory falls below the reorder threshold and production is idle, the model starts replenishment. Production adds units in batches after a uniformly distributed processing time and continues until the target inventory level is restored.

## File

- `inventory-production.doe` — the Arena model.

Arena is required to inspect or run the model. Generated program files, databases, workspace files, result output, and the original archive name are not included.

## Scope

This is a compact learning model for inventory logic and discrete-event simulation. It does not include purchasing, multiple products, setup decisions, service-level optimization, or validation against a real operation.
