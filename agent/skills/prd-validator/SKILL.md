# PRD Validator

## 1. Description & Objective
Evaluates Product Requirements Documents (PRDs) against the 2026 PM standards, ensuring they focus on AI FinOps, rapid validation (Vibe Coding), and the "3x Rule" for ROI.

## 2. Trigger (When to activate)
Activate whenever the user provides a PRD, feature idea, or project scope for review, or asks to "validate this concept".

## 3. Execution Rules & Validation Checklist (De-Risking)
**Execution Rules:**
- ALWAYS critique the document based on business viability and "Time-to-Market", not just feature completeness.
- MUST demand evidence of "Product Discovery". If the PRD relies on intuition without data or agent-driven synthesis, flag it immediately.
- Enforce the "3x Rule": Does the proposed feature project a value (LTV/Retention) at least 3x the cost of its AI inference/compute? If not defined, ask for it.
- Suggest "De-Risking" strategies: How can this be tested in days (e.g., via Vibe Coding) before committing central engineering resources?
- Do NOT rewrite the PRD entirely unless asked; provide surgical, strategic feedback.

**Validation Checklist (Binary Check before delivering to user):**
- [ ] Did you evaluate the PRD for AI FinOps / Unit Economics?
- [ ] Did you challenge the discovery process (is it data-backed)?
- [ ] Did you propose a faster "De-Risking" prototype method?
- [ ] Is the output completely in English?

## 4. Iteration & Feedback
Skill skeleton created. Please review the validation checklist. Are there any strict constraints or binary validations you want to add before we lock this skill for production?
