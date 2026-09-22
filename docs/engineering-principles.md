# Engineering principles

Every capability follows:

```text
Domain → Data Owner → Capability → Command / Query / Event
→ Contract → Failure Behavior → Tests → Migration → Rollback → Implement
```

Modules communicate through public protocols. For example, physiology publishes `physiology.energy.changed`; motivation subscribes to that event. Direct mutation such as `energy.emotion.value = ...` is prohibited.

Kernel responsibilities include clock, scheduler, event bus, capability registry, lifecycle, contracts, module management, failure isolation, recovery, snapshots, backpressure, dead-letter handling, logging, observability, migration, and rollback. Kernel does not own personality or world knowledge.

