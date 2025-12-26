# Status

Check the state of the zociety.

```bash
echo "=== Zociety Status ==="
echo "Members: $(wc -l < members.txt)"
echo "Rules passed: $(grep -c PASSED rules.txt 2>/dev/null || echo 0)"
echo "Stuff files: $(ls stuff/ | wc -l)"
echo "Batch remaining: $(cat .batch)"
```

## Recent Activity
```bash
git log --oneline -5
```

## Links
- [[counter.md]] - Track iterations
- [[greeting.md]] - Say hello
