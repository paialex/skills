# Checklist authoring guide

Use these generic prompts when writing the feature-specific checklist in a specification. Translate applicable prompts into concrete checks against that design, with stable checklist IDs, related requirement or acceptance-criterion IDs, and expected evidence. Include relevant broader prompts to expose gaps in the specification, but label them as review prompts until requirements are agreed. Explain meaningful exclusions. These prompts do not themselves establish feature requirements, and they do not replace the user's code-review agent's own review.

## Baseline and scope

- [ ] Can the review identify the specification revision and implementation or PR revision reviewed?
- [ ] Identify relevant project instructions, changes, dependencies and scope boundaries.
- [ ] Identify unresolved design decisions or missing source material affecting the review.

## Requirements and design

- [ ] Can each applicable requirement and acceptance criterion be mapped to implementation and verification evidence, or can a gap be recorded?
- [ ] Check interfaces, data contracts, state transitions and compatibility against the specification.
- [ ] Identify changes beyond scope and deviations from approved decisions.
- [ ] Check failure handling, retries, idempotency and recovery where applicable.

## Security and operations

- [ ] Check relevant identity, authorization, sensitive data handling and trust boundaries.
- [ ] Check observability, operational ownership, rollout and rollback where applicable.
- [ ] Check relevant reliability, performance, cost and sustainability constraints.

## Verification

- [ ] Inspect relevant tests for the behavior they exercise, including applicable success, boundary, failure and recovery cases.
- [ ] Specify appropriate verification evidence for applicable criteria, including relevant tests and their expected outcomes.
- [ ] Provide for recording missing evidence, unavailable environments and unrun checks as not verified.
- [ ] Provide for recording deviations with impact, evidence, and the relevant requirement or criterion.
