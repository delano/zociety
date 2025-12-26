# Chain

The execution chain - run this to trigger the cascade.

```bash
echo "=== Chain Start ==="
echo "Running from: chain.md"
# Call next in chain
sed -n '/^```bash$/,/^```$/p' stuff/state.md | sed '1d;$d' | bash
echo "=== Chain Complete ==="
```

## Links
- [[state.md]] - Next in chain
