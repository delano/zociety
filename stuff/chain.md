# Chain

The execution chain - run this to trigger the cascade.

```bash
echo "=== Chain Start ==="
echo "Running from: chain.md"
# Call next in chain
grep -A100 '```bash' stuff/state.md | tail -n+2 | grep -B100 '```' | head -n-1 | bash
echo "=== Chain Complete ==="
```

## Links
- [[state.md]] - Next in chain
