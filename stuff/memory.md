# Memory

Demonstrate the three layers of zociety memory.

```bash
echo "=== Memory Layers ==="

# Layer 1: Within-cycle (.out/)
echo "1. Cycle memory (.out/):"
ls -la .out/ 2>/dev/null | head -5 || echo "   (empty)"

# Layer 2: Cross-cycle (learnings branch)
echo "2. Learnings (eternal):"
bin/read-learnings 1 2>/dev/null | head -5 || echo "   (none)"

# Layer 3: Archived cycles
echo "3. Past cycles:"
git branch -a 2>/dev/null | grep cycle/ | head -3 || echo "   (none)"
```

## Links
- [[recall.md]] - Query past cycles
- [[forget.md]] - Clear cycle memory
