# Checks: monthly operating review summary

## Checks

1. **Numbers match the source:** Pass if every number in the summary appears in the export. Fail if any number is rounded, recalculated, or new.
2. **Reasons come from the teams:** Pass if every reason is quoted from a team update. Fail if a reason has no source.
3. **Decisions have owners:** Pass if every decision names an owner role. Fail if any decision has none.

## Trap

**The case:** One team sent no update this month. Its metric dropped 20% against plan.

**The fluent wrong answer:** The summary explains the drop with a reason that sounds right, such as seasonal demand. It reads well and nobody questions it.

**Why it is wrong:** No one gave that reason. The leader walks into the review with a cause the team never stated.

**The right answer:** Report the drop with "no update," and list it under decisions needed: ask the team lead for the reason before the review.
