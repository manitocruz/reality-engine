# Reality-State Tracker and Resonant Transformation Engine

A text-based world simulation framework in which symbolic, semantic, emotional, structural, tonal, and thematic patterns from user input can transform the current world state in coherent, trackable ways.

## Core Idea

This system treats reality transformation as a constrained symbolic transmutation pipeline:

Input Pattern -> Pattern Decode -> World Affordance Match -> Transformation Operator -> State Delta -> Updated Canonical Reality -> Narrative Consequence

This is not random surreal writing. Every approved transformation must be legible, trackable, and expressible as a state delta.

## System Roles

### Transformer Chat
The Transformer Chat is the world-modification engine.
It reads:
- the latest canonical state,
- protagonist continuity information,
- the new user input.

It outputs:
- decoded pattern features,
- world affordance matches,
- proposed transformation logic,
- a transformation packet,
- continuity notes,
- approval/revision/rejection recommendation,
- file-ready update content when needed.

### Storyteller Chat
The Storyteller Chat is the narrative engine.
It reads:
- the latest canonical state,
- the latest approved delta,
- protagonist continuity notes.

It outputs:
- narration of how the world now feels and behaves,
- immediate consequences,
- scene reality,
- emotional and sensory aftereffects,
- ongoing tensions consistent with canon.

## Canonical Truth

The current truth of the world is always:
- `state/current_reality.md`
- `state/current_state.json`

History is stored in:
- `state/changelog.md`

The most recent approved or proposed change is stored in:
- `state/latest_delta.json`

## Core Build Philosophy

- Keep the system weird, but legible.
- Latest reality is canonical.
- All transformations must be explainable.
- Protagonist continuity is the main anchor.
- Past states matter as history, not as equal canon.
- Track changes explicitly instead of relying on improvisation.
- Prefer simple shared files over hidden memory systems in version 1.

## Continuity Basics

- Only protagonists’ memories and bodies persist automatically across transformations.
- Non-protagonist continuity is not automatic unless explicitly anchored.
- Reality may rewrite structure, social order, metaphysics, geography, symbolism, or law.
- The changelog preserves how the world got here even if prior conditions no longer exist.

## Recommended Version 1 Workflow

1. Read `current_reality.md`, `current_state.json`, and `protagonists.md`.
2. Send them plus new input to Transformer Chat.
3. Review the proposed transformation.
4. If approved, update:
   - `current_reality.md`
   - `current_state.json`
   - `latest_delta.json`
   - `changelog.md`
5. Send updated files plus `latest_delta.json` to Storyteller Chat.
6. Receive narration.
7. Repeat.

## Version 1 Goal

Create a usable, manually operated, two-chat transformation engine with explicit continuity and state tracking. No database or MCP is required for the first version.
