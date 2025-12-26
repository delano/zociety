# State

Report current state, called from chain.md.

```bash
echo "--- State Report ---"
echo "Members: $(wc -l < members.txt | tr -d ' ')"
echo "Rules: $(cat rules.txt 2>/dev/null | wc -l | tr -d ' ')"
echo "Stuff: $(ls stuff/ | wc -l | tr -d ' ')"
# Call next in chain
grep -A100 '```bash' stuff/hello.md | tail -n+2 | grep -B100 '```' | head -n-1 | bash
```

## Links
- [[chain.md]] - Chain root
- [[hello.md]] - Next in chain
