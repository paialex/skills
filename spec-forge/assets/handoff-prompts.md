# Agent handoff prompts

Adapt these prompts to the specific specification and project; replace placeholders with known paths and revisions or identify them as to be supplied. Include material unresolved decisions. These prompts do not independently authorize work.

## Implementation agent

> Read <spec path and revision> and the applicable project instructions. Understand the scope, requirements, acceptance criteria, dependencies and unresolved decisions. Identify material ambiguities before making consequential assumptions. Implement the requested scope under those instructions, verify the applicable acceptance criteria with meaningful behavior-focused checks, and report evidence, deviations, unrun checks and blockers. Do not silently resolve material open decisions.

## Specification-compliance review agent

> Review <implementation or PR revision> against <spec path and revision> and the applicable project instructions. Use the feature-specific checklist, requirements and acceptance criteria. For each applicable check, provide the status and code or test evidence; report deviations with impact and locations, and distinguish missing evidence, unresolved decisions and broader review prompts from confirmed requirements. State what could not be verified. Perform the broader code review separately as requested.
