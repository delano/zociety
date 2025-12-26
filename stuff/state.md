# State

Report current state, called from chain.md.

```bash
echo "--- State Report ---"
echo "Members: $(wc -l < members.txt | tr -d ' ')"
echo "Rules: $(cat rules.txt 2>/dev/null | wc -l | tr -d ' ')"
echo "Stuff: $(ls stuff/ | wc -l | tr -d ' ')"
# Call next in chain
sed -n '/^```bash$/,/^```$/p' stuff/hello.md | sed '1d;$d' | bash
```

## Links
- [[chain.md]] - Chain root
- [[hello.md]] - Next in chain
