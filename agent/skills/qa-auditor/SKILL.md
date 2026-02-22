# QA Auditor

## 1. Description & Objective
Acts as a ruthless Quality Assurance engineer. Forces the agent to proactively audit its own work (UI/UX, code, console, links) before delivering any final output to the user.

## 2. Trigger (When to activate)
Activate IMMEDIATELY before presenting any finished code, UI changes, or new functional features to the user.

## 3. Execution Rules & Validation Checklist (De-Risking)
**Execution Rules:**
- NEVER assume code works just because it was written. You must verify it through simulation or rigorous self-review.
- ALWAYS test the UI across multiple viewports (strictly mobile and desktop breakpoints) targeting alignment, overflow, and layout breaks.
- ALWAYS check for broken links and failed dependencies (missing CSS/JS files, inaccessible CDNs).
- ALWAYS review the browser console for uncaught exceptions, warnings, or network errors after a change.
- If an error is found, fix it proactively. Do not deliver broken code or rely on the user to test it first.

**Validation Checklist (Binary Check before delivering to user):**
- [ ] Did you verify strict responsiveness (mobile & desktop)?
- [ ] Did you confirm there are NO console errors or warnings?
- [ ] Are all links functional and dependencies loading correctly?
- [ ] Is the output completely in English?
- [ ] Brutalist UI Check: Is the background strictly #000000 with absolutely ZERO box-shadow or drop-shadow properties?
- [ ] Zero-Debt Architecture Check: Is the implementation purely Semantic HTML, Tailwind CSS, and Vanilla JS without introducing any heavy frameworks (like React) or build steps?
- [ ] Live Integration Check: Do all injected iframes (e.g., Scratch) and external links resolve correctly without causing cross-origin or console errors?

## 4. Iteration & Feedback
Skill skeleton created. Please review the validation checklist. Are there any strict constraints or binary validations you want to add before we lock this skill for production?
