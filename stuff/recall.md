# Recall

Query stuff from past cycles.

```bash
echo "=== Recalling Past Cycles ==="
# List available cycle branches
CYCLES=$(git branch -a 2>/dev/null | grep 'cycle/' | tail -3)
if [[ -n "$CYCLES" ]]; then
  echo "Recent cycles:"
  echo "$CYCLES"
  # Try to show stuff from most recent cycle
  LATEST=$(echo "$CYCLES" | tail -1 | tr -d ' ')
  echo ""
  echo "Stuff from $LATEST:"
  git ls-tree --name-only "$LATEST" stuff/ 2>/dev/null | head -5 || echo "(none)"
else
  echo "No archived cycles yet"
fi
```

## Links
- [[memory.md]] - Memory overview
- [[forget.md]] - Clear memory
