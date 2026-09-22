# Embodiment

Body belongs to the Artificial Individual. Engineering knows devices such as motors, cameras, IMUs, encoders, temperature sensors, and batteries; the individual must gradually learn a body model through consequences.

```text
Motor Command → Visual Change → Proprioception → Touch
              → Vestibular Change → Environmental Result
```

Mind must use an abstract Body API rather than ports, GPIO labels, servo numbers, or camera device names. The same Mind should be able to target simulation, a small experimental robot, an advanced robot, or a humanoid body without rewriting its cognitive contracts.

Physical Body Specification and Learned Body Model are distinct artifacts.

