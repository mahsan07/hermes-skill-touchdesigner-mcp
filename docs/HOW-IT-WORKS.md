# How TouchDesigner MCP Works

The visuals on this page are static SVGs, so they render directly on GitHub on phones and desktop browsers. Each one is generated from a model specific to this skill.

## System architecture

![Detailed system map for TouchDesigner MCP](../assets/system-map.svg)

### Components

- **1. Visual brief:** participates in confirm the running touchdesigner instance.
- **2. TouchDesigner process:** participates in inspect existing operators paths and connections.
- **3. Operator network:** participates in create the smallest operator network.
- **4. MCP parameter commands:** participates in set parameters and wire dependencies.
- **5. Rendered realtime output:** participates in execute approved python or pulses.

## Actor and data sequence

![Actor and data sequence for TouchDesigner MCP](../assets/operation-sequence.svg)

### 1. Confirm the running TouchDesigner instance

**Primary surface:** `Visual brief`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 2. Inspect existing operators paths and connections

**Primary surface:** `TouchDesigner process`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 3. Create the smallest operator network

**Primary surface:** `Operator network`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 4. Set parameters and wire dependencies

**Primary surface:** `MCP parameter commands`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 5. Execute approved Python or pulses

**Primary surface:** `Rendered realtime output`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 6. Inspect viewer output and runtime errors

**Primary surface:** `Visual brief`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.

## Example output shape

![Illustrative output for TouchDesigner MCP](../assets/example-output.svg)

The example is a visual contract: a real run may look different, but it should expose comparable state, provenance, and verification information. It is not presented as evidence of a live external action.

## Decision and stop conditions

![Decision guide for TouchDesigner MCP](../assets/decision-guide.svg)

The workflow stops when the target is ambiguous, the relevant surface is unavailable or unauthorized, or the final artifact cannot be checked. A logged-in session or successful tool call is not by itself proof that the requested outcome is complete.

## Verification checklist

- Confirm every component shown in the system map exists in the target environment.
- Trace the actor sequence using actual tool output or artifact state.
- Compare the result with the example-output information contract.
- Re-read or reopen the final artifact instead of trusting an attempt message.
- Report omitted stages, unsupported capabilities, and remaining human decisions.
