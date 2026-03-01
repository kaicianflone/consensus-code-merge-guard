# consensus-code-merge-guard

Consensus-based merge governance for pull requests and code integration decisions.

`consensus-code-merge-guard` reviews a proposed merge through persona-weighted policy checks and returns:

- `ALLOW`
- `BLOCK`
- `REQUIRE_REWRITE`

## What it protects

- production stability
- security posture
- reliability of CI/CD workflows
- code quality under delivery pressure

## Core features

- strict schema validation
- deterministic decision semantics via `consensus-guard-core`
- policy-aware weighted voting
- idempotent retries for safe re-runs
- board-native artifact trail for audit and replay

## Typical signals

- failing checks/tests
- unresolved high-risk findings
- missing rollback or release notes
- policy violations in security/reliability/performance lanes

## Quick start

```bash
npm i
node --import tsx run.js --input ./examples/input.json
```

## Test

```bash
npm test
```

## Continuous improvement

See `AI-SELF-IMPROVEMENT.md` for improvement loops and guard evolution patterns.
