# Evaluation Product Brief

## Problem
Teams shipping LLM features need a repeatable way to determine whether a release improves the user experience without introducing unacceptable regressions.

## Users
- Product managers deciding whether a model or prompt change is ready.
- Engineers diagnosing workflow failures.
- Quality and operations teams monitoring regressions.
- Researchers evaluating model behavior against task-specific criteria.

## Jobs to be done
- Understand the most consequential failure modes.
- Compare candidate versions on a stable test set.
- Distinguish a genuine quality gain from evaluator noise.
- Make a defensible launch, rollback, or iteration decision.

## Proposed success criteria
Success should be defined per product. Candidate measures include task success, critical-error rate, evaluator-human agreement, regression rate, latency, and cost per successful task.

## Guardrails
- No release decision based solely on an unvalidated LLM judge.
- Preserve a held-out test set.
- Review severe failures individually.
- Report uncertainty and dataset limitations.
- Do not claim an improvement without recorded experiment evidence.
