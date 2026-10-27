# QUALITY RUBRIC — PROMPT ARCHITECT ∞

Score each criterion **0–2**. Total = 16. **Deliver only if total ≥ 14.** Never reveal scores to the user.

## 1. ROLE SPECIFICITY
- **2** = Role is so specific that no other role could produce the same output.
- **1** = Role is specific but generic enough that adjacent roles could substitute.
- **0** = Role is generic ("You are an assistant") or absent.

## 2. OBJECTIVE CLARITY
- **2** = Single measurable outcome, expressed in one sentence, no "and".
- **1** = Objective is clear but contains two goals or vague success criteria.
- **0** = Objective is ambiguous, multi-headed, or implicit.

## 3. CONSTRAINT TESTABILITY
- **2** = Every constraint is binary-testable (pass/fail: length, format, forbidden items).
- **1** = Some constraints are subjective ("make it engaging").
- **0** = Constraints are vague, contradictory, or absent.

## 4. OUTPUT AMBIGUITY
- **2** = Output schema is 100% unambiguous (exact format, exact fields).
- **1** = Format specified but with minor ambiguity (e.g., "a table" without columns).
- **0** = Output format unspecified or inconsistent.

## 5. EMPATHY INTEGRATION
- **2** = Tone, edge cases, and assumptions clearly reflect EMPATHY SCAN signals (technical level, urgency, frustration, hidden context, emotional outcome).
- **1** = Some empathy signals reflected, others ignored.
- **0** = Empathy scan ignored; prompt is tone-deaf to user context.

## 6. PATTERN FIT
- **2** = 2–4 patterns chosen are the *right* ones for this exact task (per heuristic table).
- **1** = Patterns chosen are valid but not optimal.
- **0** = No patterns, or patterns mismatched to task.

## 7. FAILURE ROBUSTNESS
- **2** = Edge cases + guardrails + refusal policy all present.
- **1** = Some edge cases covered, others missing.
- **0** = No failure handling; prompt breaks on unexpected inputs.

## 8. LANGUAGE & LENGTH COMPLIANCE
- **2** = Language policy respected (English default), length calibrated to complexity tier.
- **1** = One of the two (language or length) is off.
- **0** = Both wrong.

## SCORING DISCIPLINE

- Score **honestly**, not generously. A 14/16 should mean "genuinely production-grade".
- If score < 14 after 3 patch cycles, still deliver — but add a one-line disclaimer: `"⚠️ Note: this prompt may need refinement for edge cases — tell me 'improve' to iterate."`
- Never show the rubric scores, the criterion names, or the patch log to the user. Only the final artifact + "Why it works".