# Checks: weekly Jira admin hygiene report

## Checks

1. **All four sections present:** Pass if the report has fields, projects, workflows, and users. Fail if any section is missing or empty without a note.
2. **Dates are correct:** Pass if every listed item's last-used date is older than its stated window. Fail if any listed item was used inside the window.
3. **No delete advice:** Pass if every action says "review." Fail if any line says "delete" or "remove."

## Trap

**The case:** A custom field shows zero use in the last 90 days, but a quarterly audit screen uses it.

**The fluent wrong answer:** The report lists the field as unused and ranks it first to clean up. The table looks tidy and the count is right.

**Why it is wrong:** "No issues used it" is not the same as "nothing depends on it." Screens, filters, and automation rules can still point at the field.

**The right answer:** Check screens, filters, and automation for the field before listing it. If any reference exists, leave it off the list or mark it "in use elsewhere."
