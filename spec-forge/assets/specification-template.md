# Technical specification: <title>

- **Status:** Draft / In review / Approved / Superseded
- **Owner:** <owner or unassigned>
- **Revision/date:** <revision and date>
- **Sources:** <links and revisions of relevant inputs>
- **Source plan:** <conversation plan or file and version, when applicable>
- **Source ticket / schema:** <issue link or identifier, schema source and version, when applicable>
- **Audience:** <implementers, reviewers, operators>

## 1. Summary and problem

<Describe the problem, the proposed outcome, and why it matters. Separate known current behavior from the proposed design.>

## 2. Scope and context

- **In scope:** <boundaries>
- **Out of scope:** <boundaries>
- **Existing behavior and evidence:** <links and observations; identify unverified deployed behavior>
- **Dependencies and constraints:** <systems, policies, compatibility, environment>

## 3. Requirements

| ID | Requirement | Priority | Source / rationale |
|---|---|---|---|
| REQ-01 | <one verifiable requirement> | <required or optional> | <source> |

## 4. Design and contracts

<Describe components, responsibilities, data flow, interfaces, inputs and outputs, state transitions, compatibility, and relevant configuration. Use examples where they clarify a contract. Identify proposals and alternatives considered.>

<Where relevant, include sanitized example inputs and outputs, defaults, validation boundaries, side effects, and error outcomes. Label illustrative values and leave unresolved details explicit.>

## 5. Failure, security, and operations

<Describe applicable failure modes, retry and recovery behavior, identity and authorization, data protection, observability, support, and rollback. Identify decisions and dependencies that remain unresolved.>

## 6. Quality attributes and trade-offs

<Address relevant reliability, performance, cost, maintainability, and sustainability constraints with measurable targets when known. For AWS architecture consider all six Well-Architected pillars as relevant. Mark non-applicable topics with a reason.>

## 7. Acceptance criteria and verification

| ID | Requirement | Observable criterion | Planned verification |
|---|---|---|---|
| AC-01 | REQ-01 | <testable outcome, including preconditions> | <test, inspection, or other evidence> |

<For important behaviors specify concrete preconditions, inputs, expected outcomes and side effects. Cover relevant success, invalid input, boundary, failure and recovery cases. Identify what needs integration or live-environment evidence versus what can be checked locally, without prescribing redundant tests. Distinguish planned checks from executed results.>

## 8. Feature-specific implementation review checklist

<Write concrete checks for this feature, grouped by component when useful. Requirement-backed checks link to the requirements or acceptance criteria they verify and name the evidence a review agent should inspect. Also include relevant broader review prompts, such as security, observability and failure handling, to expose missing requirements. Label those prompts as such and do not imply they are agreed requirements. Adapt the checklist to the actual design; generic prompts alone are insufficient.>

| ID | Component | Review check | Related IDs | Expected evidence |
|---|---|---|---|---|
| CHK-01 | <component> | <observable behavior or constraint to check> | REQ-01, AC-01 | <code location, configuration, test, or other evidence to look for> |
| CHK-02 | <component> | Review prompt: <relevant concern to investigate> | Spec gap / open question | <evidence to inspect> |

<Mark items dependent on unresolved decisions as blocked or open, explaining why. This is a review handoff, not a record of checks already performed.>

## 9. Dependencies and operational considerations

<Describe relevant dependencies, compatibility and migration constraints, and operational rollback requirements. Do not prescribe implementation steps or sequencing unless requested. Do not imply permission to deploy or perform external actions.>

## 10. Assumptions, decisions, and open questions

| ID | Type | Statement and impact | Owner / resolution |
|---|---|---|---|
| OQ-01 | Open question | <question and consequence> | <owner or unassigned> |

<When based on a plan, note any material discrepancies between the plan, repository evidence and current guidance, along with their impact and proposed resolution.>

## 11. Review readiness

- <List material unresolved issues, evidence gaps, and any limitations of this draft.>

## 12. Agent handoff prompts

<Include concise implementation and specification-compliance review prompts adapted from the skill's handoff templates. Identify this spec and its revision, preserve project instructions, and identify any unresolved decisions that affect the handoff. These prompts are for later use and do not authorize implementation or external changes now.>
