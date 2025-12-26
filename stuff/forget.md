# Forget

Clear within-cycle memory (but not learnings or archived cycles).

```bash
echo "=== Clearing Cycle Memory ==="
if [[ -d .out ]]; then
  COUNT=$(ls .out/ 2>/dev/null | wc -l | tr -d ' ')
  echo "Files in .out/: $COUNT"
  rm -rf .out/*
  echo "Cleared .out/"
else
  echo ".out/ doesn't exist"
fi
echo ""
echo "Note: Learnings and cycle branches are permanent"
```

## Links
- [[memory.md]] - Memory overview
- [[recall.md]] - Query past
