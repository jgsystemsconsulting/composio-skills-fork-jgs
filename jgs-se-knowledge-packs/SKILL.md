---
name: jgs-se-knowledge-packs
description: Catalogue of 74 licence-vetted systems-engineering reference packs for coding agents. Use when a coding task needs SE domain knowledge - requirements, architecture, testing, safety, data, or operations.
---

# JGS SE Knowledge Packs

A catalogue of 74 systems-engineering reference packs, each written as an Anthropic
Agent Skill (`SKILL.md`). Packs encode real-world practice: requirements elicitation,
architecture decisions, testing strategy, safety assurance, data engineering, and
operations. All sources are open (public standards bodies, regulators, universities);
every pack records its sources and licence status.

## When To Use This Skill

- A coding agent needs domain grounding for an SE task (e.g. writing a requirements
  section, choosing an architecture pattern, planning a test approach).
- You want a vetted reference instead of general model memory.
- You are building an agent workflow that should cite standard practice.

## What This Skill Does

1. **Routes to the right pack**: maps the task at hand to a specific reference pack.
2. **Installs on demand**: packs install individually or as a catalogue via the
   skills.sh CLI.
3. **Keeps provenance**: every pack lists its open sources and licence status.

## How To Use

### Basic Usage

```text
npx skills add jgsystemsconsulting/jgs-se-knowledge-packs -l
```

List the 74 packs and pick one.

### Advanced Usage

```text
npx skills add jgsystemsconsulting/jgs-se-knowledge-packs --all
```

Install the whole catalogue. The full browsable catalogue and per-pack details:
https://github.com/jgsystemsconsulting/jgs-se-knowledge-packs

## Example

**User**: "Help me write the failure-mode section for this component spec."

**Output**: the agent loads the relevant safety/reliability pack and drafts the
section against its checklists and source citations.

## Tips

- Install single packs (`--skill sebok`) when you only need one domain.
- Packs cite their sources; follow them for standard wording.

## Common Use Cases

- Requirements and elicitation guidance for specs
- Architecture pattern selection and trade-off notes
- Testing strategy and verification planning
- Safety assurance and data-engineering references
