# Submissions folder rules

These rules apply to any agent, Claude or not. Each attendee gets one folder here. The agent writes only inside that folder.

## Naming

- Folder: `submissions/<alias>/`. The alias is a short name the attendee picks, in lowercase letters, digits, and hyphens. It is not a person's name, an employer or client, or their GitHub login. It ends with two digits, such as `ops-lead-47`.
- Branch: `submission/<alias>`.
- Files: exactly two, `rules.md` and `checks.md`. No other files.

## Limits

- `rules.md` has 15 lines or fewer, counting the numbered rules and the four labeled lines, not the title or blank lines. Delete the template comments.
- `checks.md` has 3 pass or fail checks and 1 trap.
- Do not edit any other attendee's folder.

## Check before commit

Read both files line by line. Confirm none of these remain:

- [ ] Person names
- [ ] Email addresses or phone numbers
- [ ] URLs or web addresses
- [ ] Handles, such as `@name`
- [ ] Client or employer names
- [ ] Internal system names, server names, or project codes
- [ ] Ticket keys or project keys, such as `ABC-123` or `ABC`
- [ ] Money figures tied to a company
- [ ] Passwords, API keys, tokens, or other secrets
- [ ] Commit author name and email are the GitHub username and noreply address, not a real name or work address
- [ ] The commit message, pull request title, and pull request description pass the same checks

Then confirm only `submissions/<alias>/` changed. Show the attendee the final files and get their OK before you commit.
