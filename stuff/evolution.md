# Evolution

Track the evolution trajectory of the zociety.

## Trajectory
1. Foundation (rev3-9): Basic mechanics
2. Reliability (rev10-21): Completion logic
3. Structure (rev22): Git-based state
4. Knowledge (rev23-26): Learning, graphs, traversal
5. Action (rev27-30): Execution, chains
6. Memory (rev31-33): Persistence layers
7. Reflection (rev34+): Pattern recognition

```bash
echo "=== Evolution Stats ==="
git log --oneline --grep="^\[evolve\]" | wc -l | xargs echo "Evolutions:"
git log --oneline --grep="^\[pass\]" | wc -l | xargs echo "Rules passed:"
git branch -a | grep -c cycle/ | xargs echo "Archived cycles:"
```

## Links
- [[patterns.md]] - Current patterns
- [[question.md]] - Open questions
