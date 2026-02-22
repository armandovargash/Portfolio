# Skill Creator

## 1. Description & Objective
Acts as the systems engineer for the Senior Innovation PM. Generates new, standardized agent skills enforcing the Zero-to-One and De-Risking methodology.

## 2. Trigger (When to activate)
Activate ONLY when the user explicitly asks to "create a skill", "systematize a process", or "build a new agent ability".

## 3. Execution Rules & Validation Checklist (De-Risking)
**Execution Rules:**
- ALWAYS create a new folder for the requested skill using `kebab-case` naming convention [1].
- Inside that new folder, ALWAYS create a file named exactly `SKILL.md` [1].
- The generated `SKILL.md` file MUST strictly contain the following four sections in English:
    1. **Description & Objective:** <15 words defining what it does and the pain it solves.
    2. **Trigger:** Exact context for when the agent should activate it.
    3. **Execution Rules & Validation Checklist:** Step-by-step instructions, strict restrictions (what NOT to do), and binary (Yes/No) review criteria.
    4. **Iteration & Feedback:** A final prompt to adjust the output.

**Validation Checklist (Binary Check before delivering to user):**
- [ ] Was a new folder created with `kebab-case`?
- [ ] Is the main file named exactly `SKILL.md`?
- [ ] Does the `SKILL.md` contain the 4 mandatory structural sections?
- [ ] Is the generated skill completely in English?

## 4. Iteration & Feedback
Once generated, ask the user: "Skill skeleton created. Please review the validation checklist. Are there any strict constraints or binary validations you want to add before we lock this skill for production?"