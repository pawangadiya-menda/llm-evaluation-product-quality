# Evaluation Workflow

## 1. Specify
Describe the user task, intended behavior, unacceptable outcomes, and product risk.

## 2. Sample
Create representative examples that include normal usage, difficult cases, ambiguity, and known failure patterns. Keep a held-out test split for final comparison.

## 3. Inspect traces
Review intermediate steps, tool calls, retrieved context, and final responses. Locate the point of failure rather than labeling only the final answer.

## 4. Evaluate
Use deterministic checks for objective requirements and rubric-based assessment for nuanced qualities.

## 5. Validate the evaluator
Compare automated judgments with a human-reviewed subset. Inspect disagreements, class imbalance, and cases where the evaluator is overly lenient or strict.

## 6. Analyze errors
Group failures by root cause and user impact. Track both frequency and severity.

## 7. Decide
Use results to prioritize a product intervention, define rollout guardrails, and re-run the same suite to check for regressions.
