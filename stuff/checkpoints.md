# Checkpoints

Completion needs clear criteria.

## From project management
Checkpoints are:
- Quantifiable markers of progress
- Zero-duration events marking phase completion
- Basis for evaluation and corrective action

## Zociety's checkpoints

| Checkpoint | Criteria | Verified by |
|------------|----------|-------------|
| Genesis started | DIRECTION.md deleted | `! test -f DIRECTION.md` |
| Member joined | Name in members.txt | `grep name members.txt` |
| Rule passed | Majority voted YES | Count votes in rules.txt |
| Stuff created | File in stuff/ | `ls stuff/` |
| Thresholds met | 3/2/3 achieved | Count lines/matches |
| Cycle complete | heap-death ran | DIRECTION.md exists |

## Why checkpoints matter
> "Specify completion criteria. Measure completion criteria."

Without checkpoints, "done" is subjective.
With checkpoints, "done" is verifiable.
