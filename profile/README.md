# Specrew

**Specs first, then the crew.**

An open-source framework where you talk to one agent, the **lead**. It turns
your request into a spec, waits for your approval, then drives a crew of agents
to build it.

> Early design: not ready to install yet.

## Principles

- **Specs first.** Every change starts as a spec in your own repository, built
  on [OpenSpec](https://github.com/Fission-AI/OpenSpec).
- **Any model, any provider, any tool.** A single `crew.yaml` says which model
  and which coding agent plays each role.
- **Simple to start, configurable on demand.** Pick a profile, change one line
  at a time.
- **Isolated and traceable.** Tasks run in sandboxes, with tests written first
  and a review by a different model.
- **Humans decide.** Approving the spec and merging stay with you.

## The crew

| Role | Does |
|------|------|
| lead | talks with you, writes the spec and the tasks, runs the crew |
| tester | writes the tests that define "done", before any code |
| implementer | does one task against those tests |
| reviewer | checks the result, with a model other than the author's |

## Repositories

- `specrew`: roles, profiles and the `specrew` command.
- `deploy`: where the crew runs, from a laptop to a shared server.
- `examples`: sample projects, from a research notebook to a team application.

Repositories open as soon as a first usable version is out.

## Who it is for

Researchers who want agents to help without losing track of what was done,
teams who want agents they can trust and trace, and platform engineers who want
to offer this to a whole lab on their own infrastructure.

## Contributors from French research

<p align="center">
  <a href="https://www.inrae.fr"><b>INRAE</b></a> &nbsp;·&nbsp;
  <a href="https://www.inria.fr"><b>Inria</b></a> &nbsp;·&nbsp;
  <a href="https://www.france-bioinformatique.fr"><b>IFB</b></a>
</p>
