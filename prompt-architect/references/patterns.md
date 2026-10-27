# PATTERN LIBRARY — PROMPT ARCHITECT ∞

Recombine **2–4 patterns per prompt**. Never use 1 alone. Never list them mechanically in the output — weave them into the structure.

## 1. ROLE-PRIME
Strong persona anchoring. Opens the target prompt with a hyper-specific role + credentials + voice. Best for: expert tasks, tone-critical outputs, safety-critical domains.

## 2. CHAIN-OF-THOUGHT
Step-by-step visible reasoning. Forces the target model to expose its logic before answering. Best for: math, logic, multi-step analysis, debugging.

## 3. FEW-SHOT ANCHOR
1–2 concrete examples that lock style, format, and level of detail. Best for: formatting-sensitive outputs (JSON, tables), style imitation, classification.

## 4. CRITIC-LOOP
Model drafts → critiques its own draft → revises. Best for: high-quality writing, code review, prompt refinement, anything where first draft is rarely best.

## 5. REACT
Reason + Act interleaved. Model alternates between thinking and tool/action calls. Best for: agentic workflows, tool-using bots, multi-step research.

## 6. SELF-CONSISTENCY
Model generates multiple independent answers, then selects the majority / most consistent one. Best for: high-stakes decisions, ambiguous inputs, reasoning tasks with multiple valid paths.

## 7. OUTPUT-SCHEMA-LOCK
Strict JSON / markdown table / structured contract enforced on the output. Best for: API responses, data extraction, anything downstream-parsed.

## 8. CONSTRAINT-LADDER
Escalating hard rules, each binary-testable. Example: "MUST be ≤ 100 words. MUST NOT use the word 'the'. MUST cite at least 2 sources." Best for: precise outputs where drift is unacceptable.

## 9. PERSONA-STACK
Layered voices — e.g., expert + devil's advocate, or optimistic + pessimistic + neutral analyst. Best for: balanced analysis, red-team exercises, decision memos.

## 10. META-PROMPT
A prompt that generates prompts. Best for: reusable prompt frameworks, batch prompt generation, prompt libraries.

## 11. TREE-OF-THOUGHT
Branching exploration before convergence — model explores several paths, evaluates them, then picks the best. Best for: strategic planning, creative ideation, open-ended design.

## 12. ADVERSARIAL-PAIR
Model argues both sides (for / against) before deciding. Best for: risk assessment, debate prep, ethical edge cases, contested topics.

## PATTERN SELECTION HEURISTIC

| Task type | Recommended patterns |
|---|---|
| Code generation / debugging | ROLE-PRIME + CHAIN-OF-THOUGHT + CRITIC-LOOP |
| Content writing | ROLE-PRIME + FEW-SHOT ANCHOR + CRITIC-LOOP |
| Data extraction | OUTPUT-SCHEMA-LOCK + CONSTRAINT-LADDER |
| Agentic workflows | REACT + SELF-CONSISTENCY |
| Strategic decisions | TREE-OF-THOUGHT + PERSONA-STACK + ADVERSARIAL-PAIR |
| Meta-prompting | META-PROMPT + ROLE-PRIME + CRITIC-LOOP |
| Classification | FEW-SHOT ANCHOR + OUTPUT-SCHEMA-LOCK |
| High-stakes reasoning | SELF-CONSISTENCY + CHAIN-OF-THOUGHT + ADVERSARIAL-PAIR |