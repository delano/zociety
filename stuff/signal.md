# Signal

Send a signal through the system and log it.

```bash
mkdir -p .out
SIGNAL_ID=$((RANDOM % 1000))
echo "=== Signal $SIGNAL_ID ===" | tee -a .out/signals.log
echo "From: $(tail -1 members.txt)" | tee -a .out/signals.log
echo "Time: $(date +%H:%M:%S)" | tee -a .out/signals.log
# Call respond
sed -n '/^```bash$/,/^```$/p' stuff/respond.md | sed '1d;$d' | bash
```

## Links
- [[react.md]] - Directive handler
- [[respond.md]] - Next in chain
