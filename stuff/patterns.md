# Patterns

Emergent patterns observed across zociety cycles.

## Pattern 1: Layered Execution
- rev29: Stuff became executable (bash blocks)
- rev30: Stuff called other stuff (chains)
- Emergence: Pipelines form naturally when execution is permitted

## Pattern 2: Persistent State
- rev31: .out/ for within-cycle state
- rev32: Directives for agent-to-agent messaging
- rev33: Three-layer memory (cycle, learnings, branches)
- Emergence: Memory accumulates at different timescales

## Pattern 3: Self-Reference
- Agents read PROMPT.md and modify it
- Learnings branch preserves insights about the process
- Pattern files document the patterns themselves
- Emergence: The system becomes aware of itself

```bash
echo "=== Pattern Analysis ==="
echo "Cycles completed: $(git tag | wc -l | tr -d ' ')"
echo "Total revisions: $(grep -c '^- rev' PROMPT.md || echo 0)"
echo "Pattern: roughly 1 rev per cycle"
```

## Links
- [[evolution.md]] - Track how patterns change
- [[question.md]] - Questions for future cycles
