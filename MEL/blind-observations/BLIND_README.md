# MEL: Machine Enduro Lab

## Purpose

The Machine Enduro Lab (MEL) tests whether external observers can understand SYF-Core's mathematical foundations without human interpretation or guidance. Each MEL experiment provides a "blind read" where an AI model receives only the frozen v0.1-docs from the SYF-Core repository.

## Methodology

**Input Constraints:**
- Model receives SYF-Core repository contents only
- No access to SYF-Lab
- No code execution capabilities
- No variable manipulation or simulation requests
- No prior context about project goals or terminology

**Output Format:**
- Raw, unedited observation from the model
- Model identifies components, relationships, and purpose independently
- Natural language analysis in model's original response format

## Non-Goals

MEL experiments do NOT:
- Test code execution or implementation
- Validate computational correctness
- Require the model to build working systems
- Involve human interpretation during observation
- Provide feedback loops or iterative refinement

## Kernel/Userland Boundary

**Kernel (Core Law):**
- SyFF formula: R = (F × E) / K
- FirePlank™ thermodynamic floor
- Axioms (no governance, no oracle, no feedback, no intent)

**Userland (Removable without invalidating law):**
- Implementation suggestions
- Code examples
- Use case scenarios
- Derived systems (Dizer, SEW, HYDRA, etc.)
- Specific variable interpretations

If a component can be removed without invalidating the mathematical law, it exists in userland.

## Artifact Structure

Each MEL observation is frozen as:
```
MEL/MEL-{N}_{MODEL}_BLIND_READ.md
```

Where:
- N = Sequential experiment number
- MODEL = AI model identifier (e.g., GEMINI, GPT4, CLAUDE)
- Content is verbatim output with factual header only

## Success Criteria

A successful blind read demonstrates:
1. Independent identification of SyFF as mathematical core
2. Recognition of FirePlank™ as continuity mechanism
3. Understanding of axioms as non-negotiable constraints
4. Clear distinction between kernel and derived systems
5. Acknowledgment that R carries no semantic meaning

## Limitations

MEL observations reflect:
- Model's training cutoff and capabilities
- Repository state at time of observation
- Model's natural analysis patterns
- No human steering or correction during read

These limitations are documented explicitly in each artifact's header.
