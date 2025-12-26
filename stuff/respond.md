# Respond

Acknowledge a signal and update state.

```bash
mkdir -p .out
echo "--- Response ---" | tee -a .out/signals.log
echo "Acknowledged by system" | tee -a .out/signals.log
TOTAL=$(grep -c "Signal" .out/signals.log 2>/dev/null || echo 0)
echo "Total signals: $TOTAL" | tee -a .out/signals.log
# Set directive for next agent based on count
if [[ $TOTAL -gt 3 ]]; then
  echo "Review signals.log - many signals accumulated" > .out/directive.txt
fi
```

## Links
- [[signal.md]] - Caller
- [[react.md]] - Directive handler
