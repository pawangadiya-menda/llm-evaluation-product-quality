# Evaluation Workflow

## 1. Define expected behavior

Start with the user task, product promise, and risk profile. Convert these into observable success criteria and explicit failure conditions.

## 2. Build representative inputs

Cover common requests, boundary conditions, ambiguous inputs, missing information, and adversarial or unexpected cases. Keep the held-out test set separate from examples used to tune prompts and evaluators.

## 3. Inspect traces

Review the sequence of model calls, context construction, retrieval, tool invocation, intermediate decisions, and final output. Classify where the failure originated rather than labeling only the final answer.

## 4. Design evaluators

Use deterministic checks for objective properties such as required fields, source presence, formatting, or schema validity. Use rubric-based model judges for nuanced qualities that need contextual assessment.

## 5. Validate judges

Compare judge outputs against a human-labeled sample. Inspect false positives, false negatives, disagreements, and unstable results. Revise the rubric and repeat calibration before treating scores as useful signals.

## 6. Prioritize product fixes

Rank failure patterns using severity, frequency, user impact, and remediation cost. Identify whether the best intervention belongs in the prompt, context, retrieval, tools, data, model choice, or product UX.

## 7. Run regression checks

Re-run the evaluation suite after changes. Compare segmented results and guardrails, document trade-offs, and keep a record of what changed and why.
