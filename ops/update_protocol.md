# Update Protocol

## Version 1 Operating Model
Version 1 is manual, file-based, and chat-assisted.

The operator is responsible for:
- supplying the latest state to the Transformer Chat
- approving or rejecting proposed transformations
- updating files after approval
- feeding updated state to the Storyteller Chat

## Required Read Set Before Any Transformation
Always provide the Transformer Chat with:
- `state/current_reality.md`
- `state/current_state.json`
- `state/protagonists.md`
- the new input

Optionally provide:
- relevant recent changelog entries
- `TRANSFORMATION_GRAMMAR.md`
- `CONTINUITY_RULES.md`

Always provide the Storyteller Chat with:
- `state/current_reality.md`
- `state/current_state.json`
- `state/protagonists.md`
- `state/latest_delta.json`

## Order of Operations

### Step 1: Read Canon
Read the latest canonical files.

### Step 2: Submit Input
Give the new input plus current state to Transformer Chat.

### Step 3: Review Output
Check whether the Transformer Chat output includes:
- pattern decode
- affordance match
- operator choice
- resonance depth
- continuity check
- decision status
- transformation packet

### Step 4: Validate
Run the validation checklist.

### Step 5: Decide
Choose one:
- approve
- revise
- reject

### Step 6: If Approved, Update Files
Update:
- `state/latest_delta.json`
- `state/current_reality.md`
- `state/current_state.json`
- `state/changelog.md`

### Step 7: Narrate
Send updated state plus latest delta to Storyteller Chat.

### Step 8: Archive and Repeat
Keep the updated files as the new canon.

## File Update Rules

### `latest_delta.json`
Overwrite this file with the newest approved delta.

### `current_reality.md`
Rewrite this file so it describes the new present truth cleanly.
Do not make it a patch file. It should read like the world as it now is.

### `current_state.json`
Overwrite with the structured new state.

### `changelog.md`
Append a new entry. Never delete prior entries.

## Rollback Rule
If an approved transformation proves unusable:
1. create a new changelog entry documenting rollback or corrective transformation
2. restore the previous canonical files from version control or manual copy
3. do not silently erase the failed step from history

Rollback should be recorded as a new event, not hidden.

## Approval Standard
Approve only if:
- the change is legible
- the delta is bounded
- protagonist continuity is intact or explicitly handled
- major remaps are declared
- contradictions are resolved or tracked
- the new state can be used immediately by Storyteller Chat

## Rejection Standard
Reject if:
- the proposal is arbitrary
- the change is too vague
- the resonance depth is mismatched
- canon drift is present
- continuity is broken
- the output cannot be converted into state files

## Naming Convention
Use:
`tx_###_<short_slug>`

Examples:
- `tx_001_mercy_fog_inversion`
- `tx_002_harbor_choir_bind`
- `tx_003_glass_rain_reveal`

## Recommended Versioning Practice
Use ordinary file versioning or git commits after each approved transformation.
One approved transformation = one commit.
