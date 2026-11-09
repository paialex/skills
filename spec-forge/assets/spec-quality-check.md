# Specification quality check

Review the draft against the available sources as if the implementer had not seen the conversation. Apply the checks proportionately to the work and report consequential gaps rather than inventing answers.

- **Scope:** Can the implementer identify the outcome, boundaries, dependencies and relevant source documents?
- **Required behavior:** Are requirements and contracts specific and consistent, with facts distinguished from proposals and assumptions?
- **Open decisions:** Can the implementer identify unresolved decisions, their impact and work that must wait?
- **Verification:** Does each applicable requirement have an observable acceptance criterion and a feasible verification method? Are relevant failure and recovery cases addressed?
- **Review handoff:** Does the feature checklist cover the agreed criteria, identify evidence, and label broader gap-finding prompts separately from requirements?
- **Cross-document context:** Are referenced interfaces and shared contracts identifiable without conflicting or duplicating normative requirements?
- **Fresh-agent walkthrough:** Given only the spec, referenced materials and project instructions, identify any decision an implementer must guess to produce the intended behavior. Pay particular attention to input/output examples, defaults and limits, side effects, failure outcomes, and compatibility where relevant. Report missing facts and propose options rather than inventing decisions.
- **Testability:** For important behaviors, define concrete preconditions, inputs, expected outcomes and side effects. Cover representative success, invalid input, boundaries and failure or recovery cases where applicable. State what needs integration or live-environment evidence and what can be checked locally. Do not prescribe redundant tests or require an infeasible environment.
- **Traceability:** Check that applicable acceptance criteria and review checks point back to requirements and that every material requirement has a feasible means of verification. Flag missing links or coverage; a link or test name alone does not establish correctness.
- **Examples:** Include realistic, sanitized examples when they clarify an otherwise ambiguous contract. Label illustrative values and never introduce real secrets or fabricate production behavior.

Summarize material issues and limitations in the spec. Do not claim a separate agent or real-world test unless one was actually used; this is an editorial quality check, not proof of implementation correctness.
