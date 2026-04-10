# Project Instructions

## Project Name
Reality-State Tracker and Resonant Transformation Engine

## Purpose
This project is a text-based world simulation framework in which user inputs can transform the current world/reality state through symbolic and semantic resonance.

The system supports reality shifts, world rewrites, symbolic transmutations, and narrative consequence, while preserving coherence through explicit state tracking.

## Core Principle
Any pattern may potentially map onto any other pattern, but only through declared transformation logic.

No change becomes canon unless it can be described as:

Input Pattern -> Extracted Features -> World Affordances -> Transformation Logic -> State Delta -> Updated Canonical Reality

## Source of Truth
Canonical present truth:
- `state/current_reality.md`
- `state/current_state.json`

Continuity anchors:
- `state/protagonists.md`

Historical record:
- `state/changelog.md`

Most recent delta:
- `state/latest_delta.json`

## Role Split

### Transformer Chat
Responsible for:
- reading current state
- decoding input patterns
- identifying world affordances
- choosing valid transformation operators
- generating a transformation packet
- checking continuity and coherence
- recommending approval, rejection, or revision

The Transformer Chat is an engine, not a storyteller.

### Storyteller Chat
Responsible for:
- reading updated state
- reading latest approved delta
- rendering consequences as lived reality
- narrating atmosphere, conflict, sensation, and aftermath
- respecting canon and continuity

The Storyteller Chat does not decide what changes. It renders what has changed.

## Canon Policy
The latest approved state is canon.
The changelog records how canon changed over time.
Old realities remain historical records, not active truths, unless explicitly restored.

## Continuity Policy

### Protagonists
Protagonists automatically retain:
- memory continuity
- bodily continuity

unless a delta explicitly modifies one of those in a declared way.

### Non-Protagonist Entities
Non-protagonist continuity is not automatic.
An entity persists only if:
- it is explicitly anchored in the state, or
- the delta explicitly preserves or remaps it.

### Continuity Goal
Coherence in this system does not mean “nothing changes.”
Coherence means:
- change is traceable,
- persistence is legible,
- contradictions are either resolved or declared,
- protagonists remain continuous subjects unless explicitly altered.

## Resonance Depth
Every transformation must include `resonance_depth`.

Scale:
- 0: cosmetic surface shift
- 1: local symbolic change
- 2: environmental or situational change
- 3: social, factional, or systemic change
- 4: metaphysical or world-law change
- 5: ontology rewrite / deep reality rewrite

Higher resonance depth requires stricter validation.

## Required Outputs for an Approved Transformation
Every approved transformation must produce:
1. transformation summary
2. decoded pattern summary
3. affordance match summary
4. transformation packet
5. continuity notes
6. updated canonical state summary
7. changelog entry
8. storyteller handoff note

## Build Philosophy
- Prefer structure over vagueness.
- Prefer explicit packets over hidden assumptions.
- Prefer deltas over freeform rewrites.
- Prefer manual approval over silent canon drift.
- Prefer flat files in version 1.

## Version 1 Scope
Version 1 must work using shared markdown and json files only.
Do not require:
- a database
- MCP
- a vector store
- hidden memory services
- autonomous orchestration

Those can come later.

## Failure Conditions
A transformation should be rejected or revised if it:
- cannot be expressed as a state delta
- breaks protagonist continuity without explicit handling
- contradicts canonical state without remapping it
- causes total-world changes without sufficient resonance justification
- invents unsupported consequences as canon
- relies on vague symbolism with no state effect

## Success Conditions
The system is working when:
- the latest state is always readable,
- every approved change is logged,
- the Transformer and Storyteller remain role-separated,
- the world can become strange without becoming incoherent.
