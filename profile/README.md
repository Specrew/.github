# Specrew

**Specs first, then the crew.**

> Early design. There is nothing to install yet. The repositories you may see
> here come from SpecsFirst, the former name of this organization, and will be
> replaced.

## The idea

You talk to one agent, the **lead**. It turns your request into a spec, waits
for your approval, then drives a crew of agents to build it:

| Role | Does |
|------|------|
| lead | talks with you, writes the spec and the task list, runs the crew |
| implementer | does one task, against tests written beforehand |
| tester | writes the tests that define "done", before any code |
| reviewer | checks the result, with a different model than the author |

- **Specs first.** Every change starts as a spec in your repository, built on
  [OpenSpec](https://github.com/Fission-AI/OpenSpec).
- **Any model, any provider, any tool.** One file, `crew.yaml`, says which
  model and which coding agent plays each role. Start from a profile (solo,
  team, strict) and change one line at a time.
- **Isolated.** Each task can run in its own sandbox. API keys stay outside the
  agents' reach.
- **Humans decide.** The approval of the spec and the final merge stay with
  you, and the tooling enforces it.

## What this organization will provide

- `specrew`: the crew, meaning roles, profiles and the `specrew` command.
- `deploy`: where the crew runs, from a laptop to a shared server, with
  optional sandboxing.
- `examples`: sample projects, from a research notebook to a team application.

## Who it is for

Researchers who want an agent to help without losing track of what was done,
teams who want agents they can trust and trace, and platform engineers who want
to offer this to a whole lab on their own machines.

Specrew is an independent project. It is not affiliated with OpenSpec or
CrewAI.
