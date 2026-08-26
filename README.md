# TouchDesigner MCP

> Control a running TouchDesigner instance through MCP to create operators, set parameters, wire networks, and execute Python.

This repository packages one focused Hermes skill as a public, documentation-first capability. The blueprint below explains the actual operating surfaces, control points, failure paths, and evidence expected from a trustworthy run.

![Detailed systems blueprint for TouchDesigner MCP](assets/system-blueprint.png)

## The problem it solves

Creative requests often lose their intent between the initial brief, generation, export, and final quality check.

## System components

- **Visual brief**
- **TouchDesigner process**
- **Operator network**
- **MCP parameter commands**
- **Rendered realtime output**

## Execution walkthrough

1. **Confirm the running TouchDesigner instance**
2. **Inspect existing operators paths and connections**
3. **Create the smallest operator network**
4. **Set parameters and wire dependencies**
5. **Execute approved Python or pulses**
6. **Inspect viewer output and runtime errors**

## Example request

> Using original or licensed sample material, control a running TouchDesigner instance through MCP to create operators, set parameters, wire networks, and execute Python. Return the result, the evidence used to verify it, and any limitations or actions that still require approval.

## Evidence contract

- `request.json` — captures request.
- `inspection.json` — captures inspection.
- `preview.json` — captures preview.
- `execution.json` — captures execution.
- `verification.json` — captures verification.
- `receipt.json` — captures receipt.

A run is complete only when the final artifact can be reopened or re-read and compared with the requested acceptance criteria. An attempted command or successful API response alone is not sufficient proof.

## Safety boundaries

- Confirm the exact target, owner, environment, and authority before acting.
- Preview consequential changes and pause at the approval gate.
- Keep credentials, personal data, and private endpoints out of logs and examples.
- Preserve user work and avoid unrelated changes.
- Report verification failures as incomplete work.

Read [SAFETY.md](SAFETY.md), [SECURITY.md](SECURITY.md), and the detailed [How it works](docs/HOW-IT-WORKS.md) guide before connecting this workflow to a real service or production environment.

## Repository contents

| Path | Purpose |
| --- | --- |
| `SKILL.md` | Trigger conditions and concise agent workflow. |
| `assets/system-blueprint.png` | High-resolution technical architecture poster. |
| `docs/HOW-IT-WORKS.md` | Component and execution-stage details. |
| `docs/EXAMPLES.md` | Safe, review-only, and failure scenarios. |
| `docs/PRODUCT.md` | Audience, problem statement, and maturity. |
| `SAFETY.md` / `SECURITY.md` | Operational and disclosure boundaries. |
| `tests/README.md` | Contract and package validation guidance. |

## Maturity

This is a public reference workflow extracted from a larger private workbench. It does not include a hosted runtime, credentials, or private infrastructure. Adopters must connect compatible tools and validate behavior in their own environment.

## Contributing

Contributions should improve capability accuracy, safe defaults, reproducible examples, or verification evidence without broadening the skill beyond its stated purpose. See [CONTRIBUTING.md](CONTRIBUTING.md).
