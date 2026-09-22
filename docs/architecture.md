# Architecture

```text
Artificial Individual
│
├── Individual
├── Mind
├── Artificial Physiology
├── Body
├── Kernel
├── Interface
└── External World
```

## Domain responsibilities

| Domain | Responsibility | Must not become |
|---|---|---|
| Individual | identity, lifecycle, continuity, history | a prompt or model wrapper |
| Mind | perception, memory, learning, models, control | a list of LLM prompt labels |
| Artificial Physiology | state, interoception, homeostasis, needs | a battery status panel |
| Body | action, sensing, embodiment, body model | an unowned peripheral |
| Kernel | clocks, events, scheduling, recovery, contracts | a personality or knowledge store |
| Interface | stable external capabilities and observations | direct access to private state |
| External World | the environment and its consequences | a scripted answer source |

Communication is contract-first: domain owners expose capabilities and events; consumers do not mutate another owner's internal state.

