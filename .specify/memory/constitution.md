# Spec Kit Constitution: Crypto Trading OS

## Product Intent
Autonomous algorithmic trading and risk engine.

## Architectural Invariants
- Zero Blast-Radius: Isolated sandbox execution per task.
- Strict TDD: BDD acceptance tests frozen before code development.
- Clean Code & Deterministic Verification: Sole oracle is test runner exit code == 0.
