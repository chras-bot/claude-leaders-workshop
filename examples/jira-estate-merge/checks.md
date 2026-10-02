# Checks: mapping two Jira estates before a merge

## Checks

1. **Every field accounted for:** Pass if the field count in the map equals the sum of both exports. Fail if any field is missing.
2. **No orphan statuses:** Pass if every source status has a target or sits on the open decisions list. Fail if any status is dropped.
3. **Read only:** Pass if the plan contains no step that changes either site. Fail if it does.

## Trap

**The case:** Both sites have a field called "Team." On one site it is a single select list. On the other it is a user picker.

**The fluent wrong answer:** The map marks "Team" as "same" because the names match. The table looks complete.

**Why it is wrong:** A merge on name alone puts user values into a select list, or drops them. Reports and automation that read the field break after the move.

**The right answer:** Mark the pair "keep both" or "merge with mapping," name the type difference, and add it to the open decisions list.
