# Agent Skills

A collection of portable skills for AI coding agents. Each skill is a directory with a `SKILL.md` file and supporting resources, following the [Agent Skills specification](https://agentskills.io/specification).

## Skills

### [Spec Forge](spec-forge/SKILL.md)

Turn an architecture, a session plan, a feature proposal, a GitHub issue, or a Jira ticket into detailed technical specifications for implementation agents. Each specification can include requirements, acceptance criteria, a feature-specific implementation review checklist, and handoff prompts. Spec Forge can also review local changes or a pull request against an existing spec.

The skill explores relevant project context and available tools, proposes a manageable grouping of specs, and offers focused discussion when decisions need attention. It distinguishes established requirements from assumptions and review prompts. It does not itself deploy, modify tickets, post PR comments, or implement changes without appropriate authorization.

## Install

Using the [Skills CLI](https://github.com/vercel-labs/skills), from the project where you want the skill:

```bash
npx skills add paialex/skills --skill spec-forge
```

Choose the target agents when prompted. Consult `npx skills add --help` for agent selection and global installation options. Review third-party skills and their permissions before installing them.

Alternatively, copy the entire [`spec-forge`](spec-forge/) folder, including `assets/`, into the skill directory supported by your agent:

| Agent | Example project skill location |
| --- | --- |
| Codex | `.agents/skills/spec-forge/` |
| GitHub Copilot | `.github/skills/spec-forge/` |
| Google Antigravity | `.agents/skills/spec-forge/` |
| Claude Code | `.claude/skills/spec-forge/` |

Discovery paths and invocation syntax may vary by product, version, and configuration. Consult the agent's documentation if the skill does not appear. Examples: [Copilot in VS Code](https://code.visualstudio.com/docs/agent-customization/agent-skills), [Antigravity](https://antigravity.google/docs/skills), and [Agent Skills](https://agentskills.io/specification). The common format supports portability, but behavior varies by agent and model.

## Use

Ask the agent to use **Spec Forge** and provide an accessible source. For example:

```text
Use spec-forge to analyze this project's architecture and propose a small set
of technical specifications. Explain the boundaries and open decisions.
```

```text
Use spec-forge to turn the current session plan into a detailed specification,
including acceptance criteria and a feature-specific review checklist.
```

```text
Use spec-forge to review my local changes against specs/my-feature-spec.md.
Report deviations and evidence for the applicable checklist items.
```

You can also provide an open PR and the corresponding spec, or an issue or ticket as source material. Reading external sources requires appropriate access and tools. In Codex, an installed skill may also be invoked as `$spec-forge`.

By default, the skill proposes Markdown output, uses project conventions or requested paths, and preserves existing documents. The spec and checklist are decision-support artifacts: review the result and validate behavior before relying on it.

## Development and validation

This is an initial release; behavioral quality and compatibility should be evaluated in the target agents. Validate the skill format and relative resource links, then try realistic inputs and have a fresh agent review the resulting spec for ambiguity, testability, and missing requirements. The skill does not depend on any specific MCP server or cloud provider, although it can use relevant tools and domain skills when available.

## Attribution

Spec Forge's collaborative writing workflow is inspired by [Anthropic's Doc Co-authoring skill](https://github.com/anthropics/skills/tree/main/skills/doc-coauthoring). Its approach to identifying coherent work and dependencies is also informed by [Matt Pocock's to-tickets workflow](https://github.com/mattpocock/skills/blob/main/docs/engineering/to-tickets.md). Spec Forge is an independent implementation and does not require either skill at runtime.

## License

[MIT](LICENSE).
