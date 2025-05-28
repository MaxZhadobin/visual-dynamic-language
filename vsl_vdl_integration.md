# 🔁 VSL & VDL Integration

## Visual Scene Language (VSL)
VSL provides a static, structured representation of a visual scene — objects, positions, sizes, and styles — suitable for interpretation and modification by LLMs.

Example:
- One-time snapshot
- Canvas + objects
- Use case: generating an image from description

---

## Visual Dynamic Language (VDL)
VDL extends VSL by adding a temporal layer. It tracks how a scene changes over time — introducing state, motion, and interaction semantics.

Example:
- Time-based data (video, live stream)
- Frames or segments with dynamic updates
- Use case: analyzing or generating sequences, reasoning over behavior

---

## Integration Logic

1. **Frame as VSL**: Each time step in VDL is a VSL scene + delta
2. **Temporal consistency**: Objects persist and evolve (change of position, state, relation)
3. **Actionable Events**: VDL introduces events like “enter”, “leave”, “collide”, “interact” — these are not static properties but temporal transitions
4. **LLM Capability**: With both, an LLM can:
   - Think spatially (VSL)
   - Think temporally (VDL)
   - Make decisions based on evolving structure

---

## Summary
- VSL = State of the world
- VDL = Change of the world over time
- Together = Cognitive interface for spatial-temporal reasoning

