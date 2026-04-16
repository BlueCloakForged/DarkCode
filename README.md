Dark Code Framework is a lightweight governance and engineering framework for AI-generated and AI-assisted software.

It is built for a simple problem:

Code can pass tests, ship to production, and still be poorly understood by the humans responsible for it.

That is Dark Code.

## Why This Exists

AI can generate working systems faster than traditional engineering processes can fully inspect them. The result is often code that is operationally useful but structurally opaque:

- hidden state
- unclear architectural intent
- undocumented side effects
- logic in the wrong layer
- misleading contracts between callers and services
- docs that no longer match reality

Dark Code Framework helps teams move at AI speed without giving up human accountability.

## The Core Shift

This framework shifts the standard from authorship to comprehension.

The question is no longer:

“Did a human write every line?”

The question becomes:

“Can a human explain why this code exists, how it behaves, and what risks it introduces?”

## The Three Layers

### Layer 1: Spec-Driven Development
Before code is generated, define:

- requirements
- task list
- constraints

The spec becomes the basis for evaluation. Humans approve the spec, not just the final code.

### Layer 2: Self-Describing Systems
Every important module should carry enough structural and semantic context to be understandable in isolation.

This includes:

- purpose
- dependencies
- dependents
- performance expectations
- failure modes
- retry semantics
- behavioral contracts

### Layer 3: Comprehension Gate
Before accepting AI-generated code, review it through senior-level questions:

- Why was this dependency chosen here?
- Why is the architecture shaped this way?
- Where is state managed, and is it visible?
- Is business logic leaking into the wrong layer?

This is not just code review. It is comprehension review.

## What The Framework Helps You Find

Dark Code Framework is especially useful for uncovering:

- hidden state and singleton coupling
- silent fallthrough behavior
- broken or imaginary contracts between modules
- business logic leaking into UI or transport layers
- storage and path resolution bugs
- misleading documentation
- missing failure and retry semantics
- AI-generated code that is technically functional but hard to trust

## What You Get

Using this framework helps teams produce:

- clearer specs
- better evals
- more legible modules
- safer reviews
- more maintainable AI-generated systems
- stronger human ownership of shipped behavior

## When To Use It

Use Dark Code Framework when:

- you are reviewing AI-generated code
- you inherited a system built through trial and error
- the codebase “works” but no one can explain key paths
- docs and runtime behavior seem misaligned
- you need a structured way to reduce hidden complexity

## Prompting With The Framework

When using an AI coding agent, ask it to operate through the framework explicitly.

Example prompts:

- “Review this subsystem using the Dark Code Framework. Identify hidden state, contract drift, misleading logic, and separation-of-concerns violations.”
- “Apply Layer 1, Layer 2, and Layer 3 to this feature. Tell me what spec is missing, what context is undocumented, and what a comprehension gate would flag.”
- “Audit this service for Dark Code. Focus on dependency logic, architectural intent, resource management, and policy leakage.”
- “Turn this trial-and-error implementation into a self-describing system. Propose specs, manifests, and behavioral contracts before changing code.”
- “Find code paths that work accidentally rather than intentionally, then recommend how to make them explicit.”

## Practical Review Pattern

A useful way to apply the framework is:

1. Identify the system boundary.
2. Reconstruct or write the missing spec.
3. Document module purpose, dependencies, dependents, and behavioral contracts.
4. Review for hidden state, contract mismatch, and misplaced logic.
5. Feed findings back into tests, docs, and architecture decisions.

## Goal

The goal is not to slow teams down.

The goal is to make fast AI-assisted engineering explainable, reviewable, and safe to evolve.


### Review Prompt
Review this subsystem using the Dark Code Framework.
Focus on:
- missing or weak specs
- hidden state and persistence logic
- misleading or imaginary contracts
- business logic in the wrong layer
- documentation drift
Return findings ordered by severity.

### Refactor Prompt
Apply the Dark Code Framework to this module.
First identify missing Layer 1, Layer 2, and Layer 3 artifacts.
Then propose the minimum changes needed to make the behavior explicit and self-describing.

### Architecture Prompt
Use the Comprehension Gate on this feature.
Explain:
- why each major dependency exists
- why the code is structured this way
- where state is managed
- whether logic is leaking across boundaries
Then recommend concrete fixes.
Short Tagline Options

Make AI-generated code understandable enough to own.
From working code to comprehensible systems.
A framework for turning opaque AI output into accountable engineering.
Ship at AI speed without shipping code nobody understands.
